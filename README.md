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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Positive Opinion Words

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> A [list][sentiment-lexicon] of positive opinion words.



<section class="usage">

## Usage

```javascript
import words from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-liu-positive-opinion-words-en@esm/index.mjs';
```

#### words()

Returns a [list][sentiment-lexicon] of positive opinion words.

```javascript
var list = words();
/* returns
    [
        'a+',
        'abound',
        'abounds',
        'abundance',
        'abundant',
        'accessable',
        'accessible',
        'acclaim',
        'acclaimed',
        'acclamation',
        'accolade',
        'accolades',
        ...
    ]
*/
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   A word's appearance in a sentence does **not** necessarily imply a positive or negative opinion. See [Liu (2010)](#references).
-   The list includes misspelled words. Their presence is intentional, as such misspellings frequently occur in social media content.

</section>

<!-- /.notes -->

<section class="examples">

<!-- TODO: more creative example; possibly counting the number of positive words per sentence in two pieces of text. -->

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import floor from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-floor@esm/index.mjs';
import randu from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@esm/index.mjs';
import words from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-liu-positive-opinion-words-en@esm/index.mjs';

var list = words();
var len = list.length;
var idx;
var i;

// Select random words from the list...
for ( i = 0; i < 100; i++ ) {
    idx = floor( randu()*len );
    console.log( list[ idx ] );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->



* * *

<section class="references">

## References

-   Hu, Minqing, and Bing Liu. 2004. "Mining and Summarizing Customer Reviews." In _Proceedings of the Tenth Acm Sigkdd International Conference on Knowledge Discovery and Data Mining_, 168–77. KDD '04. New York, NY, USA: ACM. doi:[10.1145/1014052.1014073][@hu:2004a].
-   Liu, Bing, Minqing Hu, and Junsheng Cheng. 2005. "Opinion Observer: Analyzing and Comparing Opinions on the Web." In _Proceedings of the 14th International Conference on World Wide Web_, 342–51. WWW '05. New York, NY, USA: ACM. doi:[10.1145/1060745.1060797][@liu:2005a].
-   Liu, Bing. 2010. "Sentiment Analysis and Subjectivity." In _Handbook of Natural Language Processing_, edited by Nitin Indurkhya and Fred J. Damerau, 2nd ed., 627–66. Chapman & Hall/CRC. <https://www.crcpress.com/Handbook-of-Natural-Language-Processing-Second-Edition/Indurkhya-Damerau/p/book/9781420085921>.

</section>

<!-- /.references -->

<!-- <license> -->

## License

The data files (databases) are licensed under an [Open Data Commons Attribution 1.0 License][odc-by-1.0] and their contents are licensed under a [Creative Commons Attribution 4.0 International Public License][cc-by-4.0]. The original dataset is attributed to Bing Liu and Minqing Hu and can be found [here][sentiment-lexicon]. The software is licensed under [Apache License, Version 2.0][apache-license].

<!-- </license> -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/datasets-liu-negative-opinion-words-en`][@stdlib/datasets/liu-negative-opinion-words-en]</span><span class="delimiter">: </span><span class="description">A list of negative opinion words.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## Copyright

Copyright &copy; 2016-2025. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-liu-positive-opinion-words-en.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-liu-positive-opinion-words-en

[test-image]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-liu-positive-opinion-words-en/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-liu-positive-opinion-words-en?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-liu-positive-opinion-words-en.svg
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-liu-positive-opinion-words-en/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[cli-section]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en#cli
[cli-url]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/tree/cli
[@stdlib/datasets-liu-positive-opinion-words-en]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/tree/main

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/tree/deno
[deno-readme]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/tree/umd
[umd-readme]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/tree/esm
[esm-readme]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/datasets-liu-positive-opinion-words-en/blob/main/branches.md

[sentiment-lexicon]: http://www.cs.uic.edu/~liub/FBS/sentiment-analysis.html#lexicon

[odc-by-1.0]: http://opendatacommons.org/licenses/by/1.0/

[cc-by-4.0]: http://creativecommons.org/licenses/by/4.0/

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

[@hu:2004a]: https://doi.org/10.1145/1014052.1014073

[@liu:2005a]: https://doi.org/10.1145/1060745.1060797

<!-- <related-links> -->

[@stdlib/datasets/liu-negative-opinion-words-en]: https://github.com/stdlib-js/datasets-liu-negative-opinion-words-en/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
