<img alt='overnightjs' src='https://github.com/seanpmaxwell/express-generator-typescript/raw/master/express-typescript.png' border='0'>

[Express](https://www.npmjs.com/package/express) with [TypeScript's](https://www.npmjs.com/package/typescript) application generator.

<a href="https://www.npmjs.com/package/express-generator-typescript" target="_blank"><img src="https://img.shields.io/npm/v/express-generator-typescript.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/package/express-generator-typescript" target="_blank"><img src="https://img.shields.io/npm/l/express-generator-typescript.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/package/express-generator-typescript" target="_blank"><img src="https://img.shields.io/npm/dm/express-generator-typescript.svg" alt="NPM Downloads" /></a>


## What is it?

Creates a new express application similar to the _express-generator_ module. Except this new
application is configured to use TypeScript instead of plain JavaScript. 



## Why express-generator-typescript?

NodeJS is great for the rapid development of web-projects, but is often neglected because of the lack of
type-safety. TypeScript solves this issue and (along with its linter file) can even make your code
more robust than some other static languages like Java.

There are some other tools out there to generate express apps with TypeScript such as 
_express-generator-ts_, but these either haven't been updated in a while, install a lot of junk 
in your project (such as an ORM), or don't take full advantage of TypeScript. 

Due to the heavy use of single-page-applications, no view-engine is configured by default. Express is 
only setup with the minimal settings for calling APIs and serving an index.html file. All the tools you 
need to run for development (while restarting on changes), build, test, and run for production are packaged 
with this library.

One huge advantage of _express-generator-typescript_ is it installs [OvernightJS](https://www.npmjs.com/package/@overnightjs/core). 
OvernightJS is a small library to add decorators to express routes and initialize them in the server file. It is not
a separate framework or an abstraction layer on top of express. It's just a simple library to add
decorators and do some basic logging. With Overnight you can build your server in a more structured,
object-oriented way instead of have to use `express.Router` objects and callbacks.



## Installation

```sh
$ Just use 'npx'
  Or
$ npm install -g express-generator-typescript
```


## Quick Start

The quickest way to get started is use npx and pass in the name of the project you want to create.
If you don't specify a project name, the default _express-gen-project_ will be used instead.

Create the app:

```bash
$ npx express-generator-typescript "project name"
```

Start your express-generator-typescript app in development mode at `http://localhost:3000/`:

```bash
$ cd "project name" && npm run start-dev
```


## Available commands for the server.

- Run the server in development mode: `npm run start-dev`.
- Run all unit-tests: `npm test`.
- Run a single unit-test: `npm test -- "name of test file (i.e. Users)"`.
- Build the project for production: `npm run build`.
- Run the production build: `npm start`.



## License

[MIT](LICENSE)
