# lucas-lehmer-test

[Lucas-Lehmer primality test](https://en.wikipedia.org/wiki/Lucas%E2%80%93Lehmer_primality_test)
in JavaScript. This is the primality test that is used by the
[Great Internet Mersenne Prime Search](http://www.mersenne.org/) to locate large
primes, and has done a pretty good job of finding some of the largest primes to
date.

## Example

Is the 31st Mersenne number a prime number?

``` javascript
var lucasLehmerTest = require('lucas-lehmer-test');

lucasLehmerTest(31);
// => true
```

## Installation

``` bash
$ npm install lucas-lehmer-test
```

## API

``` javascript
var lucasLehmerTest = require('lucas-lehmer-test');
```

### `lucasLehmerTest(value)`

Uses the Lucas-Lehmer primality test to determine if the `value`th Mersenne
number is a prime number. Returns `true` if it is; otherwise returns `false`.
`value` can be a _Number_ (it most cases it probably will be), a _String_ (for
really large numbers that JavaScript has a hard time with), or an instance of
[big-integer](https://www.npmjs.org/package/big-integer).
