# Making Components

You can create custom components to organize and maintain your code as well as share those components easily with the rest of the team.

Start by making a new file in `src/components/index` called `MyName.jsx` (generally component files should be capitalized). Then begin typing `comp-func`. If you have your snippets set up (see [Getting Set Up](getting-set-up.md)) you should see a snippet appear.

Hit enter to see the code appear. **Don't click anywhere**. Just begin typing `MyName` (generally the name of the component should match the name of the file). This should appear in two places in the file, which should now look like this:

```javascript
import React from 'react';

const MyName = (props) => (
  <div />
);

export default MyName;
```

Then replace the `<div />` with the following:

```html
<p>Hello! My name is {props.name}.</p>
```

The code `{props.name}` will display the `name` that is passed to the component once it's used (for more on React props check [the official docs](https://reactjs.org/docs/components-and-props.html)).

Now that it's created, you can use it in your `src/components/index/page.js` file.

First it must be imported with:

```javascript
import MyName from './MyName';
```

Then you can use it in the JSX for your `Page` component like this:

```javascript
<MyName name="Andrew" />
```

If you save this, you should see a paragraph on your page that reads:
```
Hello! My name is Andrew.
```

## Making Component Modules

Many times custom components have their own components inside them. They may also have separate style files used to style them. In either case, you should make not just a component but a **component module.**

POLITICO component modules are directories that look like this:
```
ComponentName
  ├── index.js
  ├── styles.scss
  └── ...OtherChildComponents
```

For example, you can make a component called `Greeting` which has some styles, and contains your original `MyName` component as a child.

Create a file in `src/components/index/Greeting/` called `index.js`. Then type: `comp-func-styles` and hit Enter to use your snippet. Without clicking away, type the word `Greeting` which should appear in three different places in your file.

Place `MyName.jsx` inside `src/components/index/Greeting` and then import it and use it `index.js` as described in the section above.

To add styles, create a file called `styles.scss` inside `src/components/index/Greeting`. Type `comp` and hit Enter to use your snippet. Any styles you put in this file will be mapped to only your `Greeting` component.

Now, you can use it in your `src/components/index/page.js` file.

Import it:

```javascript
import Greeting from './Greeting';
```

Then use it in the JSX for your `Page` component like this:

```javascript
<Greeting />
```

For more on the POLITICO component module style, check out [those docs](../front-end-apps).
