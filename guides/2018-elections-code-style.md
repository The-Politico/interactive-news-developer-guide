---
description: Essential conventions for keeping your coworkers sane.
---

# 2018 elections code style

### Repository naming conventions

Generally, back-end projects use existing naming conventions. Front-end projects use the namespace `elections-2018`.

#### Lambda front-ends

* `lambda-elections-2018-results`
* `lambda-elections-2018-slackchat`

#### Dataviz modules

Should always be scaffolded using the [graphics generator](https://github.com/The-Politico/generator-politico-graphics).

Should always follow the pattern of `module_elections-2018-*`. For example:

* `module_elections-2018-county-choropleth`
* `module_elections-2018-census-scatterplot`

#### Civic

Continues to be `politico-civic-*`.

### Linting

Is required. Use [ESLint](https://eslint.org/) in the editor of your choice for JavaScript. Use [Black](https://black.readthedocs.io/en/stable/) for Python.

### READMEs

**Write them** with any essential notes.

For **dataviz modules**, be sure to always update the README with the public API of your module.

### Project management

Will happen in [CodeTree](https://codetree.com/projects/jwX2/), based on issues in GitHub.

