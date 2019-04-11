# Working Within Your Interactive Project

PIB relies on strict naming conventions to keep you organized. The most important file that uses these conventions here:  `src/components/index/page.js`

This file will contain the React code that makes up your page. You should see some basic React code in there now. Go ahead and add some to see your preview page change.

## Non-React Client Code

You should also see a file in `src/components/index/client.js`. This file can contain JavaScript code that will run after your `Page` is component is done [mounting](https://stackoverflow.com/questions/31556450/what-is-mounting-in-react-js). You may be used to writing `DOMContentLoaded` listeners or using `$.ready()` to wait for the page to load. You don't have to worry about for the code in this file. It will only run after your page is done loading.

You can use this file to initialize D3 graphics, add event listeners, or run any other JavaScript.

## Making A Second Page

The `page.js` file located within `src/components/index` will appear at the root of your publish path. You can also add more pages by making new folders in `src/components` and placing `page.js` files inside of them.

For example, if you make the file `src/components/about/page.js`, then its content will appear on `https://politico.com/<YOUR_PUBLISH_PATH>/about/`.

**Making new `page.js` files will require you to restart your development server in order to see them.**
