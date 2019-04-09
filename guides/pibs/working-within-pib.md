# Working Within Your Interactive Project

PIB relies on a set of conventions on file and folder names in order to balance being both flexible and all-encompassing. These conventions are true of any PIB-powered interactive project, not just this template we're using as an example. The specifics can get somewhat complicated, so they'll be included elsewhere but for now what you need to know is where the pages are.

Inside the root of your codebase is a file at the location of `src/components/index/page.js`. This folder will contain the React code that makes up your page. You should see some basic React code in there now. Go ahead and add some to see your preview page change.

## Non-React Client Code

You should also see a file in `src/components/index/client.js`. This file can contain JavaScript code that will run after your `Page` is component is done mounting. You don't need to worry about waiting for page loads in your code.

You can use this file to initialize D3 graphics for add event listeners among other things.

## Making A Second Page

The `page.js` file located within `src/components/index` will appear at the root of your publish path. Put you can also make multiple pages if your project requires it by making new folders in `src/components` and placing `page.js` files inside of them.

For example, if you make the file `src/components/about/page.js`, then its content will appear on `https://politico.com/<YOUR_PUBLISH_PATH>/about/`.
