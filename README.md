# arr-flatten [![NPM version](https://img.shields.io/npm/v/arr-flatten.svg?style=flat)](https://www.npmjs.com/package/arr-flatten) [![NPM monthly downloads](https://img.shields.io/npm/dm/arr-flatten.svg?style=flat)](https://npmjs.org/package/arr-flatten) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/arr-flatten.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/arr-flatten) [![Windows Build Status](https://img.shields.io/appveyor/ci/jonschlinkert/arr-flatten.svg?style=flat&label=AppVeyor)](https://ci.appveyor.com/project/jonschlinkert/arr-flatten)

> Recursively flatten an array or arrays.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save arr-flatten
```

Install with [yarn](https://yarnpkg.com):

```sh
$ yarn add arr-flatten
```

## Install

Install with [bower](https://bower.io/)

```sh
$ bower install arr-flatten --save
```

## Usage

```js
var flatten = require('arr-flatten');

flatten(['a', ['b', ['c']], 'd', ['e']]);
//=> ['a', 'b', 'c', 'd', 'e']
```

## Benchmarks

This library versus [array-flatten](https://github.com/blakeembrey/array-flatten), on April 14, 2017:

```
#1: large.js
  arr-flatten.js x 487,030 ops/sec ±0.67% (92 runs sampled)
  array-flatten.js x 347,020 ops/sec ±0.57% (98 runs sampled)

#2: medium.js
  arr-flatten.js x 1,914,516 ops/sec ±0.76% (94 runs sampled)
  array-flatten.js x 1,391,661 ops/sec ±0.63% (96 runs sampled)

#3: small.js
  arr-flatten.js x 5,158,980 ops/sec ±0.85% (94 runs sampled)
  array-flatten.js x 3,683,173 ops/sec ±0.79% (97 runs sampled)

```

**Run the benchmarks**

```bash
$ npm run benchmarks
```

## Why another flatten utility?

I wanted the fastest implementation I could find, with implementation choices that should work for 95% of use cases, but no cruft to cover the other 5%.

## About

### Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

### Building docs

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

### Running tests

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

### Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](https://twitter.com/jonschlinkert)

### License

Copyright © 2017, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.5.0, on April 14, 2017._