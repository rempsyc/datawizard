# datawizard 0.2.3.9000

- New functions to find or remove empty rows and columns in a data frame:
  `empty_rows()`, `empty_columns()`, `remove_empty_rows()` and 
  `remove_empty_columns()`.

- Arguments `cols`, `before` and `after` in `data_relocate()` can now also be
  numeric values, indicating the position of the destination column.

# datawizard 0.2.3

- New functions:

  + to work with lists: `is_empty_object()` and `compact_list()`
  + to work with strings: `compact_character()`

# datawizard 0.2.2

- New function `data_extract()` (or its alias `extract()`) to pull single 
  variables from a data frame, possibly naming each value by the row names
  of that data frame.

- `reshape_ci()` gains a `ci_type` argument, to reshape data frames where 
  CI-columns have prefixes other than `"CI"`.

- `standardize()` and `center()` gain arguments `center` and `scale`, to define
  references for centrality and deviation that are used when centering or
  standardizing variables.

- `center()` gains the arguments `force` and `reference`, similar to
  `standardize()`.

- The functionality of the `append` argument in `center()` and `standardize()` 
  was revised. This made the `suffix` argument redundant, and thus it was 
  removed.

- Fixed issue in `standardize()`.

- Fixed issue in `data_findcols()`.

# datawizard 0.2.1

- Exports `plot` method for `visualisation_recipe()` objects from `{see}`
  package.

- `centre()`, `standardise()`, `unstandardise()` are exported as aliases for
  `center()`, `standardize()`, `unstandardize()`, respectively.

# datawizard 0.2.0.1

- This is mainly a maintenance release that addresses some issues with
  conflicting namespaces.

# datawizard 0.2.0

- New function: `visualisation_recipe()`.

- The following function has now moved to *performance* package:
  `check_multimodal()`.

- Minor updates to documentation, including a new vignette about `demean()`.

# datawizard 0.1.0

* First release.
