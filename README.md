# @swenkerorg/vitae-ut <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Is this value a JS regex?
This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isRegex = require('@swenkerorg/vitae-ut');
var assert = require('assert');

assert.notOk(isRegex(undefined));
assert.notOk(isRegex(null));
assert.notOk(isRegex(false));
assert.notOk(isRegex(true));
assert.notOk(isRegex(42));
assert.notOk(isRegex('foo'));
assert.notOk(isRegex(function () {}));
assert.notOk(isRegex([]));
assert.notOk(isRegex({}));

assert.ok(isRegex(/a/g));
assert.ok(isRegex(new RegExp('a', 'g')));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@swenkerorg/vitae-ut
[2]: https://versionbadg.es/inspect-js/@swenkerorg/vitae-ut.svg
[5]: https://david-dm.org/inspect-js/@swenkerorg/vitae-ut.svg
[6]: https://david-dm.org/inspect-js/@swenkerorg/vitae-ut
[7]: https://david-dm.org/inspect-js/@swenkerorg/vitae-ut/dev-status.svg
[8]: https://david-dm.org/inspect-js/@swenkerorg/vitae-ut#info=devDependencies
[11]: https://nodei.co/npm/@swenkerorg/vitae-ut.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@swenkerorg/vitae-ut.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@swenkerorg/vitae-ut.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@swenkerorg/vitae-ut
[codecov-image]: https://codecov.io/gh/inspect-js/@swenkerorg/vitae-ut/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@swenkerorg/vitae-ut/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@swenkerorg/vitae-ut
[actions-url]: https://github.com/swenkerorg/vitae-ut/actions
