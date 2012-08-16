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
