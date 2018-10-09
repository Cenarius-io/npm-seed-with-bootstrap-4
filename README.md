# Basic NPM seed project with Bootstrap 4
This is a basic seed project for web-development with bootstrap 4 and SASS. Furthermore this contains a live server and
basic build-process which is handle the scss linting and compiling, the minifying, and image compressing.

## Install
```console
$ git clone https://github.com/Kenariosz/npm-seed-with-bootstrap-4.git npmSeed
$ cd npmSeed
$ npm install
```

## Usage

### Development
```console
$ npm run start
```
This script does the following tasks:
- Copy bootstrap.js, popper.js and jquery.slim.min.js and their map files under the builds/development/js folder from
node modules.
- Run scss/css watcher
- Run scss/css linting
- Compile the bootstrap scss and custom scss
- Run postcss-autoprefixer
- Run a live server 

### Production
```console
$ npm run build
```
This script responsible for the production creation. It has the following tasks:
- Copy jquery.slim.min.js under the builds/production/js folder from node modules. 
- Compile scss files for production
- Run html-minifier
- Run image compression
- Run uglify-js
- Run a live server for production
