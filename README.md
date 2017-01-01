# Blockstack Tutorials

## Building a Hello World App

In this first Blockstack app tutorial, we'll take you through the process of building the simplest Blockstack app where users login and are shown a welcome message with their name and avatar. You'll learn how to (1) create a simple frontend web app with HTML, JS and CSS (2) integrate blockstack.js for identity and authentication (3) register a domain name for the app, listing it in the app directory.

### Getting Started

To get started, first clone this repo to your local machine by running:

```bash
$ git clone git@github.com:blockstack/blockstack-tutorialsblockstack-tutorials.git
$ cd blockstack-tutorials/hello-world/
```

Once you have cloned this repo, download all the dependencies by running:

```bash
$ npm install
```

Next, `browserify` is used to connect the node_modules in `requires.js` to the browser code found in the `/public` folder.

Browserify was already downloaded as a dependency, so simply run:

```bash
$ browserify requires.js > public/bundle.js
```

This will create a `bundle.js` file in the public folder to immediately invoke blockstack.js for use in `app.js`. Note, you do not have to include `bundle.js` in the header of your html file, this has already been done for you.
