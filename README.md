# jest-raw-loader

[Jest](https://facebook.github.io/jest/) transformer mimicking [webpack-contrib/raw-loader](https://github.com/webpack-contrib/raw-loader)'s functionality

## Install

```
$ npm install --save-dev @glen/jest-raw-loader
```

## Usage

Use [jest's `transform` configuration options](https://facebook.github.io/jest/docs/en/configuration.html#transform-object-string-string) to use this package in your unit tests.

For example use the following to raw load `.md` and `.graphql` files:

```json
"jest": {
  "transform": {
    "\\.graphql$": "@glen/jest-raw-loader",
    "\\.md$": "@glen/jest-raw-loader"
  }
}
```

This is for jest >= 28, if you are using older version use `jest-raw-loader` package:
- https://github.com/keplersj/jest-raw-loader

## License

Copyright 2017-2020 [Kepler Sticka-Jones](https://keplersj.com/). Licensed MIT.
