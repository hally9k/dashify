# dashify [![NPM version](https://img.shields.io/npm/v/dashify.svg?style=flat)](https://www.npmjs.com/package/dashify) [![NPM monthly downloads](https://img.shields.io/npm/dm/dashify.svg?style=flat)](https://npmjs.org/package/dashify) [![NPM total downloads](https://img.shields.io/npm/dt/dashify.svg?style=flat)](https://npmjs.org/package/dashify) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/dashify.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/dashify)

> Convert a camelcase or space-separated string to a dash-separated string. ~12 sloc, fast, supports diacritics.

Please consider following this project's author, [Jon Schlinkert](https://github.com/jonschlinkert), and consider starring the project to show your :heart: and support.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save dashify
```

## Why another dashify lib?

Most slugify libs cover way too many corner cases and are bloated and slow as a result. I made this as a fast and light alternative (it even supports diacritics in ~12 sloc).

## Usage

```js
var dashify = require('dashify');

console.log(dashify('fooBar'));
//=> 'foo-bar'

console.log(dashify('fooBarBaz'));
//=> 'foo-bar-baz'

console.log(dashify('foo bar'));
//=> 'foo-bar'

console.log(dashify('foo barBaz'));
//=> 'foo-bar-baz'

console.log(dashify('foo barBaz quux'));
//=> 'foo-bar-baz-quux'

console.log(dashify('São Tomé and Príncipe'));
//=> 'são-tomé-and-príncipe'
```

## options.condense

**Type:** `boolean`

**Default**: `undefined`

Condense multiple consecutive dashes to one.

```js
console.log(dashify('Foo----Bar'));
//=> 'foo----bar'

console.log(dashify('Foo----Bar', {condense: true}));
//=> 'foo-bar'
```

## About

<details>
<summary><strong>Contributing</strong></summary>

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

</details>

<details>
<summary><strong>Running Tests</strong></summary>

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

</details>

<details>
<summary><strong>Building docs</strong></summary>

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

</details>

### Related projects

Other awesome string libs you might like:

* [pascalcase](https://www.npmjs.com/package/pascalcase): Convert a string to pascal-case. | [homepage](https://github.com/jonschlinkert/pascalcase "Convert a string to pascal-case.")
* [romanize](https://www.npmjs.com/package/romanize): Convert numbers to roman numerals (useful for books, outlines, documentation, slide decks, etc) | [homepage](https://github.com/jonschlinkert/romanize "Convert numbers to roman numerals (useful for books, outlines, documentation, slide decks, etc)")
* [word-wrap](https://www.npmjs.com/package/word-wrap): Wrap words to a specified length. | [homepage](https://github.com/jonschlinkert/word-wrap "Wrap words to a specified length.")
* [wordcount](https://www.npmjs.com/package/wordcount): Count the words in a string. Support for english, CJK and Cyrillic. | [homepage](https://github.com/jonschlinkert/wordcount "Count the words in a string. Support for english, CJK and Cyrillic.")

### Contributors

| **Commits** | **Contributor** | 
| --- | --- |
| 17 | [jonschlinkert](https://github.com/jonschlinkert) |
| 1 | [der-On](https://github.com/der-On) |
| 1 | [jeffreypriebe](https://github.com/jeffreypriebe) |

### Author

**Jon Schlinkert**

* [linkedin/in/jonschlinkert](https://linkedin.com/in/jonschlinkert)
* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](https://twitter.com/jonschlinkert)

### License

Copyright © 2017, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.6.0, on December 03, 2017._