# Reduxor
__A React Router ready, Redux & React Isomorphic starting template for mortals.__

Isomorphic React starting package cause the rest of them suck and I wanted to make my own with the latest packages.

### Technology
* Redux v2.0
* React v0.13.0
* React Router v1.0.0-rc1
* Express v4.13.3
* Webpack v1.12.1
* Babel v5.8.23

### Primary Goals
* Get the latest packages on npm playing nicely.
* Pay careful attention to create a clearly defined easy to follow file structure.
* Isomorphicize as much as practical.
* Plays nicely as a 12 Factor app. http://12factor.net/
* Avoid unnecessary global dependencies especially for deployment. _(ie. favour using local .bin, avoid gulp)_
* Should be low volume production ready launchable via npm start for upstart.
* Everything should be the same version of ES$#%@.

### TODO
- [x] Refactor to Redux
- [x] Isomorphic Rendering with a service
- [x] Encapsulate Hydration using [Drator](https://www.npmjs.com/package/drator)
- [x] Implement [Redux actions](https://github.com/acdlite/redux-actions)
- [x] Implement [Redux promise](https://github.com/acdlite/redux-promise)
- [x] Service Proxying with [Nector](http://github.com/ryardley/nector)
- [ ] Service Authentication with [Passport](https://github.com/jaredhanson/passport) and [Nector](http://github.com/ryardley/nector)
- [ ] React Zurb Foundation or Bootstrap
- [ ] Login Page with Authenticated resources.
- [ ] Seed data script.
- [ ] React Hot Loading.
- [ ] Redux Dev Tools.
- [ ] Minification.
- [ ] Assets / Gzip.
- [ ] Cache server rendered pages in memory.

### Future goals
- [ ] CSS Modules.
- [ ] Upgrade to React v0.14
- [ ] Unit tests
- [ ] Feature tests
- [ ] Simple basic deployment script to SSH into a server and run a git pull.

## To setup

Install dependencies
```bash
$ npm i
```

## To run
The start in development mode

```bash
$ npm start
```

Then shoot over to [http://localhost:3000/](http://localhost:3000/) to be amazed at the awesomeness.

## To run in production
The start in production mode

```bash
# First build the source
$ npm run build

# Then start with NODE_ENV set to production
$ NODE_ENV=production npm start
```

## Environment vars

To customise your environment create a .env file to provide some simple environment information.

```bash
# .env
PORT=3181
ASSET_HOST=http://localhost:8080
```

Here we are setting the development port to run on 3181 and the location of the transpiled assets to be http://localhost:8080 (webpack-dev-server defaults)
