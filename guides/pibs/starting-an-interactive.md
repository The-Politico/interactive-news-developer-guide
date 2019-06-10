# Starting An Interactive Page

Once you have everything set up with at least one template registered, you can get started.

In your terminal, make a new folder and enter it:

```text
$ mkdir MY_PROJECT_NAME
$ cd MY_PROJECT_NAME
```

Then run PIT's new project command:

```text
$ pit new
```

Here you'll see three different ways of finding your registered templates. For simplicity, select `Show me all my templates` and then select `Interactive Story` \(if you don't see it make sure you've completed the [Set Up Guide](getting-set-up.md).\) Give the project a name, and you should then see some files in your folder.

With most templates \(including this one\) you'll have to install dependencies by running:

```text
$ yarn
```

Then you can open up your new codebase in atom:

```text
$ atom .
```

And you can start your development server by running:

```text
$ yarn start
```

