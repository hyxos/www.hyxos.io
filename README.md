# www.hyxos.io

## Deploy Status
[![Netlify Status](https://api.netlify.com/api/v1/badges/2d47f1e0-ee3e-445c-ae5c-019799b411e1/deploy-status)](https://app.netlify.com/sites/naughty-ritchie-2769b9/deploys)

## Features

* Simple content model and structure. Easy to adjust to your needs.
* Contentful integration using our [Sync API](https://www.contentful.com/developers/docs/references/content-delivery-api/#/reference/synchronization/initial-synchronization-of-entries-of-a-specific-content-type)
* Using our [Delivery API](https://www.contentful.com/developers/docs/references/content-delivery-api/).
* Responsive/adaptive images via [gatsby-image](https://www.gatsbyjs.org/packages/gatsby-image/)

## History

This project is fork of a repo from [contentful-userland](https://github.com/contentful-userland) which means that we’re always open to contributions **and you can be part of userland and shape the project yourself after your first merged pull request**. You can learn more about how contentful userland is organized by visiting [our about repository](https://github.com/contentful-userland/about).

## Requirements

To use this project you have to have a Contentful account. If you don't have one yet you can register at [www.contentful.com/sign-up](https://www.contentful.com/sign-up/).

## Getting started

Install [Yarn](https://yarnpkg.com/en/docs/install) (if you haven't already).

### Get the source code and install dependencies.

```
$ git clone git@github.com:hyxos/www.hyxos.io.git
$ yarn install
```

Or use the [Gatsby CLI](https://www.npmjs.com/package/gatsby-cli).

```
$ gatsby new contentful-starter https://github.com/hyxos/www.hyxos.io.git
```

### Set up of the needed content model and create a configuration file

This project comes with a Contentful setup command `yarn run setup`.

![Command line dialog of the yarn run setup command](https://rawgit.com/contentful-userland/gatsby-contentful-starter/master/setup.jpg "Command line dialog of the yarn run setup command")

This command will ask you for a space ID, and access tokens for the Contentful Management and Delivery API and then import the needed content model into the space you define and write a config file (`./contentful.json`).

`yarn run setup` automates that for you but if you want to do it yourself rename `.contentful.json.sample` to `.contentful.json` and add your configuration in this file.

## Crucial Commands

This project comes with a few handy commands for linting and code fixing. The most important ones are the ones to develop and ship code. You can find the most important commands below.

### `yarn run dev`

Run in the project locally.

### `yarn run build`

Run a production build into `./public`. The result is ready to be put on any static hosting you prefer.

### `yarn run deploy`

Run a production build into `./public` and publish the site to GitHub pages.

### `yarn run cleanup-repository`

Removes all dependencies, scripts and data from the installation script.

## Roadmap

- [x] [make the starter completely responsive](https://github.com/contentful-userland/gatsby-contentful-starter/issues/2)
- [ ] [include tags](https://github.com/contentful-userland/gatsby-contentful-starter/issues/3)
- [x] [support traced placeholders](https://github.com/contentful-userland/gatsby-contentful-starter/issues/4)
- [ ] [add i18n](https://github.com/contentful-userland/gatsby-contentful-starter/issues/6)

## Other resources

- Tutorial video series ["Building a blazing fast website with GatsbyJS and Contentful"](https://www.youtube.com/watch?v=Ek4o40w1tH4&list=PL8KiuH6vpACV-F7jXribe4YveGBhBeG9A) by @Khaledgarbaya
