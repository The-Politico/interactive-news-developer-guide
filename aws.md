# AWS

We use Amazon Web Services to host most of our interactives infrastructure.

### Keep it tidy!

##### Lambda

- Always prefix lambda distributions `interactives_*`.

##### S3

- All interactive projects **must** go into folders by year, e.g., `2017/your-project`. (If publishing through the [interactives generator](https://github.com/The-Politico/generator-politico-interactives), this is done for you.)
- Use common slug conventions for naming your projects and avoid underscores. Wherever possible, call your projects something meaningful, never something generic like `new-project`.
- Use the interactives generator to bundle Javascript and CSS assets and to create responsive image sets.
- **Very rarely** there is a file that is common to many interactives. You may place this in a `common/` folder at the root of the bucket. In general, though, don't do this. Bundle assets with individual projects.