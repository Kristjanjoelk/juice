1.3.2 / 2014-11-24
==================

 * Add option preserveImportant [jrit]

1.3.1 / 2014-11-24
==================

 * Add option applyLinksToStyleTags [jrit]

1.3.0 / 2014-07-22
==================

 * Update dependencies and code cleanup
 * heads up, xhtml might be handled differently
 * extract LICENSE from README
 * rename History.md to CHANGELOG.md

1.2.0 / 2014-05-22
==================

 * Add option applyWidthAttributes to API [jrit]

1.1.0 / 2014-05-22
==================

 * preserve single quotes for values [jrit]

1.0.0 / 2014-05-07
==================

 * order styles alphabetically to preserve expected style priority [jrit]
 * major version bumped in case people expected styles to not be sorted alphabetically

0.7.0 / 2014-05-06
==================

 * add preserveMediaQueries API [jrit]

0.6.0 / 2014-04-25
==================

 * update dependencies [jonkemp]

0.5.1 / 2014-03-12
==================

 * fix not including all stylesheets [andxyz]

0.5.0 / 2013-04-15
==================

 * update dependencies to latest
 * fix not preserving DOCTYPE [jgannonjr]
 * fix decoding local file paths [alexluke]

0.4.0 / 2013-04-15
==================

 * update jsdom dependency to 0.6.0

0.3.3 / 2013-04-08
==================

 * fix resolving file:// paths on windows (thanks Mirco Zeiss)
 * fix crash during cleanup. (thanks Ger Hobbelt)
 * update superagent to 0.14.0

0.3.2 / 2013-03-26
==================

 * fix regression: not ignoring pseudos

0.3.1 / 2013-03-26
==================

 * do not crash on ::selectors (covered by normalize.css test case)

0.3.0 / 2013-03-26
==================

 * update jsdom dependency to 0.5.4
 * support node v0.10
 * switch dependency to slick instead of mootools which was rudely unpublished

0.2.0 / 2013-02-13
==================

 * update jsdom dependency to 0.5.0

0.1.3 / 2013-02-12
==================

 * fix specificity test. all test cases passed now.
 * add a command line `juice` program

0.1.2 / 2013-02-11
==================

 * fix incorrectly lowercasing <link> href

0.1.1 / 2013-02-11
==================

 * explicitly document which node versions are supported
   with `engines` and travis-ci.
 * expose `juice.inlineDocument` and `juice.inlineContent`

0.1.0 / 2013-02-07
==================

 * fix / test case for @media queries
 * merge [boost](https://github.com/andrewrk/boost) into juice
 * legacy `juice` function still works as is
 * add `juice(filePath, [options], callback)`
 * add `juice.juiceDocument(document, options, callback)`
 * add `juice.juiceContent(html, options, callback)`
 * remove `juice.juiceDom`

0.0.9 / 2013-02-07
==================

 * update jsdom dependency to 0.4.0
 * update cssom dependency to 0.2.5

0.0.8 / 2013-02-06
==================

  * expose a lower level export so you can operate on a jsdom document [andrewrk]
  * fix exports not working [andrewrk]
  * fix jshint problems [andrewrk]

0.0.7 / 2013-02-06
==================

  * fixed test case expected outputs to have starting and ending <html> and <body> tags as jsdom appends them in its html() function if they do not exist
  * regression test for previous fix for media queries. note i had to wrap my test .out content in <html><body> tags in order to pass tests, it looks like they are appended at some point for partial html content which just guessing is new behavior from when these tests were written
  * make sure the css rule has selectorText to prevent parsing exception. hit this on @media rules which do not have selector text. afaik this means media queries will not be inlined. however everything else is.
  * bump jsdom
  * Added note regarding node-email-templates to README

0.0.6 / 2011-12-20
==================

  * Corrected juice unit tests for latest cssom.
  * Fixed presence of \n in selectors.
  * Fixed unneeded removal of inline event handlers in html.
  * Bumped jsdom.

0.0.5 / 2011-10-10
==================

  * Added whitelist of pseudos to ignore (fixes `:first-child` etc)
  * Fine-tuned jsdom for speed (disabled unneded features).
  * Added caching of parsed selectors.

0.0.4 / 2011-10-10
==================

  * Fixed `:hover`.

0.0.3 / 2011-10-09
==================

  * Fixed specificity :not recursion.

0.0.2 / 2011-10-09
==================

  * Fixed specificity calculation for `not()` and pseudos. [arian]

0.0.1 / 2011-10-09
==================

  * Initial release.
