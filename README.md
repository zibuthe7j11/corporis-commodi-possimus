# @zibuthe7j11/corporis-commodi-possimus <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.

## Example

```js
var getSymbolDescription = require('@zibuthe7j11/corporis-commodi-possimus');
var assert = require('assert');

assert(getSymbolDescription(Symbol()) === undefined);
assert(getSymbolDescription(Symbol('')) === ''); // or `undefined`, if in an engine that lacks name inference from concise method
assert(getSymbolDescription(Symbol('foo')) === 'foo');
assert(getSymbolDescription(Symbol.iterator) === 'Symbol.iterator');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@zibuthe7j11/corporis-commodi-possimus
[2]: https://versionbadg.es/inspect-js/@zibuthe7j11/corporis-commodi-possimus.svg
[5]: https://david-dm.org/inspect-js/@zibuthe7j11/corporis-commodi-possimus.svg
[6]: https://david-dm.org/inspect-js/@zibuthe7j11/corporis-commodi-possimus
[7]: https://david-dm.org/inspect-js/@zibuthe7j11/corporis-commodi-possimus/dev-status.svg
[8]: https://david-dm.org/inspect-js/@zibuthe7j11/corporis-commodi-possimus#info=devDependencies
[11]: https://nodei.co/npm/@zibuthe7j11/corporis-commodi-possimus.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@zibuthe7j11/corporis-commodi-possimus.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@zibuthe7j11/corporis-commodi-possimus.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@zibuthe7j11/corporis-commodi-possimus
[codecov-image]: https://codecov.io/gh/inspect-js/@zibuthe7j11/corporis-commodi-possimus/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@zibuthe7j11/corporis-commodi-possimus/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@zibuthe7j11/corporis-commodi-possimus
[actions-url]: https://github.com/zibuthe7j11/corporis-commodi-possimus/actions
