# Publishing An Interactive
Once your code is ready to publish, there's a quick checklist you should make sure you run through:

- [ ] Social Info Filled Out In `src/content/social.js`
- [ ] Social Image Created And Put In `dist/images/share.jpg`
- [ ] [Metadata](working-with-meta.md) Filled Out
  - [ ] `pageName`
  - [ ] `publishPath`
  - [ ] `authors`

Then you can run the following (which will publish to staging):
```
$ yarn pub
```

You'll be prompted to update the publish time. If you don't want to set it to the current date, just say so and it will ask you again next time you try to publish.

If the preview looks good, you can then publish to production:
```
$ yarn pub --production
```

## Updating An Interactive
If you need to make changes to an interactive, you can do so in the codebase and then publish it again. This time you'll be prompted to add an updated time which you can do if you wish. You should also pass an invalidation to break the server cache:

```
$ yarn pub --production --invalidate
```
