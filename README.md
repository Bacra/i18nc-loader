I18NC-LOADER
============

[![NPM Version][npm-image]][npm-url]
[![NPM Downloads][downloads-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Coveralls][coveralls-image]][coveralls-url]
[![NPM License][license-image]][npm-url]
[![License Status][license-status-image]][license-status-url]


# Install

```
npm install i18nc-loader webpack --save-dev
```

# Useage

```javascript
module.exports = {
  entry: {'input': 'input.js'},
  output: {
    path: 'dist',
    filename: '[name].js',
  },
  module: {
    rules: [{
      test: /\.js$/,
      use: [{
        loader: 'i18nc-loader',
        options: {
          I18NHandlerName: 'weLANG'
        }
      }]
    }]
  }
};
```

# OPTIONS

You can pass [i18nc options](https://bacra.github.io/node-i18nc-core/?p=options)
using standard webpack [loader options](https://webpack.js.org/configuration/module/#useentry).



[npm-image]: http://img.shields.io/npm/v/i18nc-loader.svg
[downloads-image]: http://img.shields.io/npm/dm/i18nc-loader.svg
[npm-url]: https://www.npmjs.org/package/i18nc-loader
[travis-image]: http://img.shields.io/travis/Bacra/i18nc-loader/master.svg?label=linux
[travis-url]: https://travis-ci.org/Bacra/i18nc-loader
[coveralls-image]: https://img.shields.io/coveralls/Bacra/i18nc-loader.svg
[coveralls-url]: https://coveralls.io/github/Bacra/i18nc-loader
[license-image]: http://img.shields.io/npm/l/i18nc-loader.svg
[license-status-url]: https://app.fossa.io/projects/git%2Bgithub.com%2FBacra%2Fi18nc-loader?ref=badge_shield
[license-status-image]: https://app.fossa.io/api/projects/git%2Bgithub.com%2FBacra%2Fi18nc-loader.svg?type=shield
