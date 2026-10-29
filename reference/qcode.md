# This launches the coder Shiny app

This launches the coder Shiny app

## Usage

``` r
qcode(use_wd = TRUE)
```

## Arguments

- use_wd:

  Whether or not the current working directory when launching qcoder
  should be used as the base from which the project file is selected.

## Examples

``` r
if (interactive()) {
 qcode()
}
```
