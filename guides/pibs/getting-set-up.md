---
description: >-
  Before you can start using PIBS, you'll need to make sure a few things are set
  up on your computer first.
---

# Getting Set Up

## Before You Start

Even before starting the setup process, you'll need the following information:

| Name | Description | Key |
| :--- | :--- | :--- |
| AWS Access Key | One of two keys needed to authenticate into AWS. | `AWS_ACCESS_KEY_ID` |
| AWS Secret Access Key | One of two keys needed to authenticate into AWS. | `AWS_SECRET_ACCESS_KEY` |
| AWS CloudFront Distribution | The ID needed to pass invalidations to CloudFront. | `AWS_CLOUDFRONT_DISTRIBUTION` |
| Google API Key | A key used to authenticate into Google. | `GAPI_PRIVATE_KEY` |

These four keys should be in the credentials package you received when you first started at POLITICO. If you're missing one, see Jon McClure.

You'll also need this information too, but it's not sensitive so we can publish it on the web:

| Name | Description | Key | Value |
| :--- | :--- | :--- | :--- |
| Bucket Name \(default\) | The default bucket used if no environment is specified \(we default to staging to be safe\). | `DEFAULT AWS_BUCKET_NAME` | `staging.interactives.com` |
| Base URL \(default\) | The URL to that default bucket. | `DEFAULT AWS_BASE_URL` | `https://s3.amazonaws.com/staging.interactives.politico.com` |
| Bucket Name \(staging\) | The name of our staging bucket. | `STAGING AWS_BUCKET_NAME` | `staging.interactives.com` |
| Base URL \(staging\) | The URL to the staging bucket. | `STAGING AWS_BASE_URL` | `https://s3.amazonaws.com/staging.interactives.politico.com` |
| Bucket Name \(production\) | The name of our production bucket. | `PRODUCTION AWS_BUCKET_NAME` | `interactives.politico.com` |
| Base URL \(production\) | The URL to the production bucket. | `PRODUCTION AWS_BASE_URL` | `https://politico.com/` |
| Google Client Email | The email account name of our team's Google service account | `GAPI_CLIENT_EMAIL` | `politico-interactives@politico-interactives-228617.iam.gserviceaccount.com` |

## Setting Up PIB

Now that you have all the credentials you need, you can set up PIB. PIB is a toolkit with a lot of functionality for making interactive pages. It'll handle all the building, previewing, data management, and publishing for you. But before you can use all that, you'll need to give it all the necessary keys.

Make sure you have Node installed on your computer by typing `node --version` into a terminal. If you don't see a version number, you can get Node [here](https://nodejs.org/en/download/).

Then, install PIB by typing the following into a terminal window:

```text
$ npm install -g @politico/interactive-bin
```

Then run:

```text
$ pib setup
```

You'll be asked to provide a number of values based on key prompts. You can look up those keys in the tables above. Then, you can say no to adding any new or editing any values.

## Setting Up PIT

Unlike PIB, PIT is focussed on one thing: making it easy for you to find the template you need to get started. Out of the box it has no templates though, so you'll need to supply those.

Install PIT by typing the following into a terminal window:

```text
$ npm install -g @politico/interactive-templates
```

Once it's installed you can register new templates. We'll start with a basic one that'll be used throughout this guide:

```text
$ pit register https://github.com/The-Politico/template_pib-interactive
```

One of the advantages of using PIT is that you don't have to worry about keeping your templates up to date. Every time you start a new project, it'll use the latest version of the template from GitHub.

You can see all the templates we have to offer on the [templates page](templates.md), or learn how to make your own by reading the [PIT Docs](https://github.com/The-Politico/politico-interactive-templates/blob/master/docs/templates.md).

## Setting Up Your Linter

As part of this suite, POLITICO also has a custom `eslint` configuration to be used on all projects. The linter configuration will be set up for you if you start a project from a template, but you'll need to make sure your Atom has the right plugins to take full advantage.

In Atom, hit `Cmnd + ,` to open up your settings. Go to `Packages`. Search for and install a package called `linter-eslint`. Scroll down and check the box that says `Autofix Fix on Save`. Once you have this package installed, linting in your template-generated projects should happen by default. Try forgetting a semi-colon on a line of JavaScript and saving the file. It should be added for you automatically.

## Setting Up Snippets

Snippets in Atom are a powerful way to save yourself on repeated code. As a team we share snippets in a GitHub repo to make it easier for anyone to edit. To add these snippets to your Atom, go to [the repo](https://github.com/The-Politico/politico-interactive-code-snippets). Then, in your Atom, go to `Atom` in the top menu, and click `Snippets...`. This will open a file in your editor. Replace the contents with what you see in the README of the snippets repo.

## Setting Up Google Docs

All Google Docs for interactive projects go in [this folder](https://drive.google.com/drive/folders/1LwuTm5ueV-gvIma0Up5opkbUqK0WTbmV). Make sure you have full read/write access to it. If you need access, contact Andrew Briz.

We'll cover making new new docs later in this guide.

