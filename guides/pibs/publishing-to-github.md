# Publishing To GitHub

One day this will be done automatically. Until then, it'll need to be done manually.

## Initializing A Repo

To initialize a repo run the following in the root of your project:

```text
$ git init
```

## Creating A Repo on GitHub

Go to [GitHub](https://github.com/new) and create a new repo.

You should name the repo `interactive_YOUR-PROJECT-NAME-HERE`.

After you create it you should see a GitHub URL that looks like this:

```text
git@github.com:The-Politico/interactive_YOUR-PROJECT-NAME-HERE.git
```

Connect this repo to your folder by running the following \(providing that GitHub URL\):

```text
$ git remote add origin <GITHUB_URL_HERE>
```

## Using Git

Once you've done this, you can use all the usual `git` commands to publish to Github, including `git add`, `git commit`, and `git push`. See [the docs](https://git-scm.com/doc) for more on those.

