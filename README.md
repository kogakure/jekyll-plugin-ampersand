![Maintenance](https://img.shields.io/maintenance/no/2012.svg)

Jekyll plugin Ampersand
=======================

A simple plugin for Jekyll (or Octopress) that replaces all occurrences of
`&` or `&amp;` surrounded by spaces with a `<span>`. It will add
`&thinsp;` (Thinspace) before and after the ampersand to prevent the words
before and after to be broken into different lines.

It will replace 'Peter & Paul', but not 'Peter&Paul' and it will not replace any
`&` or `&amp;` in attributes.

Usage
-----

    <div class="entry-content">{{ content | ampersand }}</div>

Output
------

It will output a string like this:

    Peter&thinsp;<span class="amp">&amp;</span>&thinsp;Paul

The MIT License
---------------

Copyright (c) 2012 Stefan Imhoff

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
