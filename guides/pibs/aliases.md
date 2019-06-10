# Using Aliases

PIB comes with a number of built-in aliases to make importing easier.

Without aliases, if you want to import a file from your `src/content` directory in your `src/components/index/page.js` your import statement would look like this:

```javascript
import headline from '../../content/headline.txt'
```

And those `..` would only increase as your project became more complicated. However, because PIB already has aliases, you can instead import it from anywhere in your codebase like this:

```javascript
import headline from 'Content/headline.txt'
```

The aliases included in PIB are:

* `Data` → `YourProject/src/data`
* `Common` → `YourProject/src/components/common`
* `Content` → `YourProject/src/content`
* `Theme` → `YourProject/src/theme`
* `Utils` → `YourProject/src/utils`
* `package.json` → `YourProject/package.json`
* `politico-components` → `YourProject/node_modules/politico-style/js/lib/components/base`

