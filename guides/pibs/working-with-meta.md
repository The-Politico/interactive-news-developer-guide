# Working With Metadata

Metadata is always found is in your `package.json`. There should be a `pib` key with some information pre-filled.

### `template`

`template` determines the routine PIB uses to build your interactive. It should only ever be one of two values: `static` or `dynamic`.

`static` means that any code written in your `page.js` files will be run once to create your page, and then discarded. So things like click handlers in your JSX will no longer work.

`dynamic` means that any code written in your `page.js` files will be used to create your page, and then your page will be [hydrated](https://reactjs.org/docs/react-dom.html#hydrate) on-load to keep that functionality around. So things like click handlers and state management will continue to work after loading.

### `id`

`id` is a random value generated each time you make a new project. It's used to uniquely identify your project.

### `pageName`

`pageName` is the title of your page (both in the `<title>` and for Chartbeat).


### `siteSection`, `pageType`, `adUnitSection` & `freePaidContent`

These are values used for UTag. They should mostly be left as is unless you know what you're doing.

### `publishPath`

`publishPath` is the URL of your story after `https://politico.com/`. It should almost always start with `interactives`.

### `published` & `updated`
These values will be set automatically when you publish (or update) your interactive. You can manually set this to an ISO string in Zulu time which looks like this: `2019-04-09T19:43:35.259Z`. They can also each be set to `null` to not be displayed.

If you need help converting to an ISO string, you can use [this demo](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toISOString). Type your string in line one (take note of the timezone you're using), and click `Run >`. You should see your ISO string as the second output in the console.

### `authors`
`authors` should be an array of objects with two keys: `link` and `name`. This array will be used for UTag data and will also be rendered with their links in your page's header.
