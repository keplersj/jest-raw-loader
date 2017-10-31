# jest-raw-loader

[![npm](https://img.shields.io/npm/v/jest-raw-loader.svg)](https://www.npmjs.com/package/jest-raw-loader)
[![Build Status](https://travis-ci.org/keplersj/jest-raw-loader.svg?branch=master)](https://travis-ci.org/keplersj/jest-raw-loader)
[![Code Coverage](https://codecov.io/gh/keplersj/jest-raw-loader/branch/master/graph/badge.svg)](https://codecov.io/gh/keplersj/jest-raw-loader)
[![Code Style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)


[Jest](https://facebook.github.io/jest/) transformer mimicking [webpack-contrib/raw-loader](https://github.com/webpack-contrib/raw-loader)'s functionality

## Install

```
$ npm install --save-dev jest-raw-loader
```

## Usage

Use jest's `transform` configuration options to use this package in your unit tests. For example use the following to raw load `.md` and `.graphql` files:

```js
"jest": {
  "transform": {
    "\\.graphql$": "<rootDir>/node_modules/jest-raw-loader/index.js",
    "\\.md$": "<rootDir>/node_modules/jest-raw-loader/index.js"
  }
}
```

## License

MIT © [Kepler Sticka-Jones](https://github.com/keplersj)