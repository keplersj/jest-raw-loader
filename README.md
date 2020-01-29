# jest-raw-loader

[Jest](https://facebook.github.io/jest/) transformer mimicking [webpack-contrib/raw-loader](https://github.com/webpack-contrib/raw-loader)'s functionality

## Install

```
$ npm install --save-dev jest-raw-loader
```

## Usage

Use [jest's `transform` configuration options](https://facebook.github.io/jest/docs/en/configuration.html#transform-object-string-string) to use this package in your unit tests.

For example use the following to raw load `.md` and `.graphql` files:

```json
"jest": {
  "transform": {
    "\\.graphql$": "jest-raw-loader",
    "\\.md$": "jest-raw-loader"
  }
}
```

## License

MIT © [Kepler Sticka-Jones](https://github.com/keplersj)
