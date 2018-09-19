---
description: Style guide for front-end application architecture
---

# JS apps

## The Stack

* React/Preact
* Redux
* redux-orm

And on the backend, usually...

* Django
* Django Rest Framework
* PostgreSQL

#### How we got here

We've been building apps at scale in React/Redux for over 3 years. React introduced a more sustainable component architecture to our front-end work and Redux paired with redux-orm created a data model we were comfortable relying on.

Most of our backend code is written in Python and in large part we chose React/Redux because it makes our front-end code feel _more Pythonic_. React components are composable in a way we're used to working with Python's object-oriented model. Redux creates a data control layer that smacks of Django's ORM and redux-orm is just to drive the point all the way home.

You may have other opinions. That's great! We've just got deadlines...

We've found this stack is highly reliable, composable and **most importantly** easy to reason about and read. React and Redux are also well-documented, supported, optimized and **most importantly** come with fantastic development tools that help us discover and isolate issues quickly.

In terms of performance benchmarks, this stack has supported the fastest election night results pages on internet™. That's good enough for us.

## Folder structure

### Top-level directories

```text
js/
  components/
  stores/
  theme/
  content/
```

#### Components all the way down

We prefer not to distinguish between containers/components, dumb/smart, fat/skinny in our top-level directory structure. Instead, all JSX components should go into a `components/` directory at the root of your app.

#### Separate app state

We prefer app state, e.g., Redux actions, reducers and stores, be kept separately under a `stores/` directory.

#### Styles

A `theme/` directory should contain universal style rules for your app including colors, fonts, mixins, etc. We prefer styles that apply to markup be colocated with the components they style and loaded as [CSS modules](https://github.com/css-modules/css-modules).

#### Content

Any text content should be loaded from a top-level directory. We do this so any content that needs copy-editing is more easily accessible. This includes meta data.

## Components

#### Hierarchy

We use a combination of hierarchy by **type/function** and **feature/domain**.

At the top level, we nest strictly by **type** under any routes or views, respectively.

```text
components/
  chat/     << Routes
  results/  << Routes
    senate/ << Views
    house/  << Views
    gov/    << Views
    
```

Thereafter, we encourage organizing components by **feature/domain**. The goal is to keep directories as shallow as possible below views but also to **collocate** related files so no one directory gets too large or unwieldy. Use your discretion.

#### No useless folders

If a directory is simply a pass-through, we prefer to shorten the directory path instead of maintaining strict hierarchy.

```text
components/
  app/       << PASS-THROUGH representing a single route
    senate/
    house/
    gov/
```

```text
components/  << REMOVE IT!
  senate/
  house/
  gov/
```

#### Make component modules

Organizing components as modules is encouraged. Use an `index.js` file to create a public entry for your component and write your base-level component directly in that file \(rather than just importing it from a separate file\).

```text
card/
  Description.jsx
  index.js
  styles.scss
  Title.jsx
```

```javascript
import React from 'react';
import Card from './card';

const Stack = (props) => {
  return (
    <div>
      {props.data.map(d =>
        <Card data={d} />
      )}
    </div>
  );
}

```

#### Hoist common components

Common components should be hoisted to the highest level that they are shared in your component directory. Use a `common/` directory to contain them.

```text
components/
  chat/
  results/
    common/
      CountyMap.jsx    << COMMON COMPONENT
    senate/            << USED HERE
    house/
    gov/               << USED HERE
```

#### Separate layout components

Layout components are either containers that simply pass through `props.children` or they compose components in a specific configuration. Generally, they **should not** __create any new props for their children, merely pass through props from a parent component.

```text
components/
  results/
    layout/
      Desktop.jsx << SEPERATE LAYOUT
      Mobile.jsx  << SEPARATE LAYOUT
    table/
    map/
```

##  Stores

Our structure for stores is [ducks](https://github.com/erikras/ducks-modular-redux)-ish in that we don't split Redux folders by type. Group them instead by branch of the app state, with one notable exception for redux-orm models.

```text
stores/
  orm/
    api.js
    actions.js
    constants.js
    fixtures.js
    reducers.js << Reducers (default export) + Selectors (named exports)
    utils/
      distributions.js
  filters/
    actions.js
    constants.js
    reducers.js
  models/
    Race.js
    Result.js
    Candidate.js
  index.js
```

#### Keep actions and constants separated

They can be more easily imported that way.

#### Write selectors

Always write [selectors](https://redux.js.org/recipes/computingderiveddata). Don't denormalize or query your app state in your components.

Wherever possible memoize selectors with [reselect](https://github.com/reduxjs/reselect) or even just lodash's [memoize](https://lodash.com/docs/4.17.10#memoize) to improve performance.

#### Write reducers and selectors in the same file

Export the reducer by default and the selectors by name. Break this rule if your selectors become too large or, better yet, write more [composable](https://github.com/reduxjs/reselect#composing-selectors) selectors.

Selectors should operate on the same state shape as is defined in the reducer. Prune the state in another place, if the reducer state is only a piece of the app state.

```javascript
// stores/orm/reducers.js
import * as actions from './constants';

export default (currentState, action) => {
  const initialState = {
    races: {},
  };
  // ...
  return newState;
}

export const getActiveRaces = state =>
  state.races.filter(r => r.active);
```

```javascript
// stores/index.js
import races, * as fromRaces from './races';

// ...

export const getActiveRaces = (state) =>
  fromRaces.getActiveRaces(state.races);
```

#### Keep models separate

Write these together as a close copy of the models directory in your API \(usually Django\). 

Keep the data in your models normalized. \(Use selectors to denormalize!\)

Always use camelCase field names in your redux-orm models.

#### Connect multiple components

If you can, [connect](https://redux.js.org/basics/usagewithreact#implementing-container-components) parts of your app state to [multiple components](https://redux.js.org/faq/reactredux#should-i-only-connect-my-top-component-or-can-i-connect-multiple-components-in-my-tree). This will limit the number of pass-through props you have and can increase performance.

## Theme

Define universal styles here, including fonts and default typography rules, color variables and classes, etc.

Don't define component styles here.

#### On using CSS modules for component styles

CSS module spec makes sure styles are prefixed and scoped just to the component they apply to.



## Content

Keep all copy-editable content external to your code in simple Markdown or txt files.

Use our [Webpack Markdown loader](https://github.com/The-Politico/markdown-react-loader) to load paragraph text from Markdown files as React components.

```javascript
import Content from 'Content/intro.md';

const Intro () => (
    <div className='top'>
        <Intro />
    </div>
);
```

Use the [raw-loader](https://github.com/webpack-contrib/raw-loader) to load strings from txt files for small textual.

```javascript
import Description from 'Content/meta/decsription.txt';

const Head = () => (
    <Helmet>
        <meta name="description" content={Description} />
    </Helmet>
);
```

You're encouraged to use modules to group like content.

```text
content/
  about/
    Description.md
    index.js
    Contact.md
```

```javascript
import React from 'react';
import Content from 'Content/about'; // << CONTENT MODULE

const AboutPage = () => (
  <div className='about-page'>
    <Content.Description />
    <hr />
    <Content.Contact />
  </div>
);
```



