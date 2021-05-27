# tinkr dev

* xml and yaml objects are now stored in an R6 class called `yarn`.
* testthat edition 3 is now being used with snapshot testing.
* Tables are now pretty after a full loop `to_xml()` + `to_md()` (@pdaengeli, #9)
* 2021-05-04: yarn objects remember the `sourcepos` and `encoding` options 
  when using the `$reset()` method.
* 2021-05-06: `protect_math()` function and method protects LaTeX math (dollar 
  notation) from escaping by commonmark (@zkamvar, #39).
* 2021-05-06: GitHub-flavored markdown ticks/checkboxes are now protected by
  default (@zkamvar, #39).
* 2021-05-11: `md_ns()` is a new convenience function to provide the `md` 
  namespace prefix for commonmark xml documents (@zkamvar, #39).
* 2021-05-11: `stylesheet()` returns the path to the internal {tinkr} stylesheet
  so that it can easily be discovered by other packages
* 2021-05-11: yarn methods `show()`, `head()`, and `tail()` all gain 
  `stylesheet_path` arguments so the modified stylesheets can be used.
* 2021-05-24: reference style links (i.e. `[text][link-ref]` with `[link-ref]: 
  <link>` on another place in the document will be preserved and the anchor will
  sink to the bottom of the document.

# tinkr 0.0.0.9000

* Added a `NEWS.md` file to track changes to the package.
