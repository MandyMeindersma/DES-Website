[![Netlify Status](https://api.netlify.com/api/v1/badges/5f9bdcfb-7b48-46e8-a58d-dfd2b32d8ccc/deploy-status)](https://app.netlify.com/sites/dev-edmonton/deploys)

# Dev Edmonton Society

New home for the [devedmonton.com](https://devedmonton.com) website

> Fostering a stronger software development community in Edmonton.

## Questions and Discussion

If you'd like to discuss anything about the website we have a channel on the [DES Slack (join here)](https://devedmonton.com/#about-our-slack) called #des-website-contributing that is welcome to anyone. Feel free to ask questions, get clarification, and request/discuss features.

## Development Setup

Note that all of these commands have been tested and used on Mac/unix machines, if you are on windows and these do not work for you look in the contributing guidelines for help.

```bash
# switch to project node version
$ nvm use

# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build production bundle and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate

# run the linter
$ npm run lint # check for linting errors
$ npm run lint:fix # fix linting errors

# run pr checks
$ npm run pr-checks
```

For detailed explanation on how things work, check out [Nuxt docs](https://nuxt.com).

## Import Calendar Events Function local testing.

1. You'll need the netlify cli install globally if you don't have it already.

```bash
$ npm install -g netlify-cli
```

2. In one terminal, run the netlify dev server.

```bash
$ netlify dev
```

3. In another terminal, run the import script.

```bash
$ npm run daily-calendar-import
```

Notes:

- cron job in `netlify/scheduled-functions.json`
- function located at `netlify/functions/daily-calendar-import.js` (all it does is hit the import api endpoint)

# Resources

Icons sourced from [Iconify](https://iconify.design/icon-sets/ph/)
