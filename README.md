# @diotoborg/fugit-at-porro <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

A helper to optimistically set Symbol.toStringTag, when possible.

Most common usage:
```js
var assert = require('assert');
var setToStringTag = require('@diotoborg/fugit-at-porro');

var obj = {};

assert.equal(Object.prototype.toString.call(obj), '[object Object]');

setToStringTag(obj, 'tagged!');

assert.equal(Object.prototype.toString.call(obj), '[object tagged!]');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@diotoborg/fugit-at-porro
[npm-version-svg]: https://versionbadg.es/es-shims/@diotoborg/fugit-at-porro.svg
[deps-svg]: https://david-dm.org/es-shims/@diotoborg/fugit-at-porro.svg
[deps-url]: https://david-dm.org/es-shims/@diotoborg/fugit-at-porro
[dev-deps-svg]: https://david-dm.org/es-shims/@diotoborg/fugit-at-porro/dev-status.svg
[dev-deps-url]: https://david-dm.org/es-shims/@diotoborg/fugit-at-porro#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@diotoborg/fugit-at-porro.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@diotoborg/fugit-at-porro.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@diotoborg/fugit-at-porro.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@diotoborg/fugit-at-porro
[codecov-image]: https://codecov.io/gh/es-shims/@diotoborg/fugit-at-porro/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/es-shims/@diotoborg/fugit-at-porro/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/es-shims/@diotoborg/fugit-at-porro
[actions-url]: https://github.com/diotoborg/fugit-at-porro/actions
