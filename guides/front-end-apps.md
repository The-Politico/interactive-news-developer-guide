---
description: Style guide for front-end application architecture
---

# JS apps

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

Any text content should be loaded from a top-level directory. We do this so any content that needs copy-editing is more easily accessible.

This includes meta data.

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
components/ . << REMOVE IT!
  senate/
  house/
  gov/
```

#### Make component modules

Organizing components as modules is encouraged and helps collocate your code. Use an `index.js` file to create a public entry for your component.

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
      ResultsTable.jsx << COMMON COMPONENT
    senate/            << USED HERE
    house/             << USED HERE
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

#### Ducks-ish

Group 

```text
stores/
  orm/
    actions.js
    constants.js
    fixtures.js
    reducers.js << Reducers (default export) + Selectors (named exports)
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

## Content

Use our [Webpack Markdown loader](https://github.com/The-Politico/markdown-react-loader) to load paragraph text as React component.

Use the [raw-loader](https://github.com/webpack-contrib/raw-loader) to load strings from txt files for small textual.

You're encourage to form content groups using modules. For example:

```text
content/
  about/
    Description.md
    index.js
    Contact.md
```

```javascript
import React from 'react';
import Content from 'WebContent/about'; // << CONTENT MODULE

const AboutPage = () => (
  <div className='about-page'>
    <Content.Description />
    <hr />
    <Content.Contact />
  </div>
);
```



