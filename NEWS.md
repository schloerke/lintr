# lintr 1.0.0.9000 #

* Fixed lint_package bug where cache was not caching (#146, @schloerke)
* Commas linter handles missing arguments calls properly (#145)

# lintr 1.0.0 #
* bugfix to work with testthat 1.0.0

# lintr 0.3.3 #
* infix_spaces_linter now properly checks `=` in named arguments. (#130, @saurfang).
* commas_linter now properly recognizes lints when preceded by a blank line and points to the missing space rather than the comma (#111, #129, @saurfang).
* Make spaces_left_parentheses_linter more robust when determining `(` type (#128, @saurfang)
* commented_code_linter (#83, @jackwasey)
* Now trims long comments (#55, reported by @paulstaab)
* Automatic commenting of Github commits and pull requests when linting on Travis-CI
* expect_lint_free expectation can be added to testthat unit tests.
* Robust configuration system and exclusion logic
* Emacs and Sublime Text 3 plugins now available from their respective package repositories.
* add `names.lints`, `split.lints` (#49, @ttriche)
* Fixed bug that caused vim syntatic plugin not to work properly in windows (#46, @abossenbroek)
* allow lintr customization per project using `.lintr` config files.
* use `globalenv()` instead of `baseenv()` for default parent environment so
  that `methods` will be included.
* do not check object usage if eval fails.  Fixes (#24, reported by @fabian-s)
* `trailing_whitespace_linter` was reporting the incorrect line number
* Use RStudio source marker API to display lints (#37, @jjallaire)
* Permit single quotes if they quote literal double quotes (#28, @jackwasey)
* # nolint comments are respected with caching (#68, @krlmlr)
* Properly handle all knitr document formats

# lintr 0.2.0 #

* Initial release
