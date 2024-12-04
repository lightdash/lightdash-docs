[![Netlify Status](https://api.netlify.com/api/v1/badges/0ed2850c-dbab-4c76-8bfe-c3706712fe34/deploy-status)](https://app.netlify.com/sites/peaceful-bassi-cbf284/deploys)



# Website

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

## Installation

```console
yarn install
```

## Local Development

```console
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build

```console
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

```console
GIT_USER=<Your GitHub username> USE_SSH=true yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.

## API docs

API docs are automatically generated from the [Lightdash API](https://github.com/lightdash/lightdash/tree/main/packages/backend) and hosted on this site. They are publicly available [here](https://docs.lightdash.com/api/v1)

The source of truth for the API docs is the [OpenAPI spec](https://github.com/lightdash/lightdash/blob/main/packages/backend/src/generated/swagger.json) which is used to generate the docs.

The [update-swagger.yml](.github/workflows/update-swagger.yml) GitHub Action runs on a schedule and updates the docs site with the latest API docs. You can also manually trigger a build by going to the [Github actions](https://github.com/lightdash/lightdash-docs/actions/workflows/update-swagger.yml) and clicking the "Run workflow" button.
