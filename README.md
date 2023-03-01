<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Median

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> [Degenerate][degenerate-distribution] distribution [median][median].

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

The [median][median] for a [degenerate][degenerate-distribution] random variable is

<!-- <equation class="equation" label="eq:degenerate_median" align="center" raw="\operatorname{Median}\left( X \right) = \mu" alt="Median for a degenerate distribution."> -->

<div class="equation" align="center" data-raw-text="\operatorname{Median}\left( X \right) = \mu" data-equation="eq:degenerate_median">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@e1fbdee688c5409e4cc6b0cd06d90b1cd2abd67c/lib/node_modules/@stdlib/stats/base/dists/degenerate/median/docs/img/equation_degenerate_median.svg" alt="Median for a degenerate distribution.">
    <br>
</div>

<!-- </equation> -->

where `μ` is the constant value of the distribution.

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

To use in Observable,

```javascript
median = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-degenerate-median@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var median = require( 'path/to/vendor/umd/stats-base-dists-degenerate-median/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-degenerate-median@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.median;
})();
</script>
```

#### median( mu )

Returns the [median][median] of a [degenerate][degenerate-distribution] distribution with constant value `mu`.

```javascript
var v = median( 10.0 );
// returns 10.0

v = median( -0.5 );
// returns -0.5
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-degenerate-median@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var mu;
var v;
var i;

for ( i = 0; i < 10; i++ ) {
    mu = randu();
    v = median( mu );
    console.log( 'µ: %d, Median(X;µ): %d', mu.toFixed( 4 ), v.toFixed( 4 ) );
}

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/stats-base-dists-degenerate-median.svg
[npm-url]: https://npmjs.org/package/@stdlib/stats-base-dists-degenerate-median

[test-image]: https://github.com/stdlib-js/stats-base-dists-degenerate-median/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-median/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/stats-base-dists-degenerate-median/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/stats-base-dists-degenerate-median?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/stats-base-dists-degenerate-median.svg
[dependencies-url]: https://david-dm.org/stdlib-js/stats-base-dists-degenerate-median/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-median/tree/deno
[umd-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-median/tree/umd
[esm-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-median/tree/esm
[branches-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-median/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/stats-base-dists-degenerate-median/main/LICENSE

[degenerate-distribution]: https://en.wikipedia.org/wiki/Degenerate_distribution

[median]: https://en.wikipedia.org/wiki/Median

</section>

<!-- /.links -->
