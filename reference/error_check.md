# Check for coding errors

Checks the current document for coding errors.

## Usage

``` r
error_check(document)
```

## Arguments

- document:

  A string to be scanned for errors.

## Value

A `warning` message as a character string.

## Details

This function takes a string (such as the contents of a document), and
conducts some basic linting. It returns a warning if there aren't a
matching number of `(QCODE)` tags, or if text has been marked to be
captured but the capture is missing a tag (missing `{#my_tag}`).

## Examples

``` r
error_check("An (QCODE)unmatched set of (QCODE) gives (/QCODE){#tag} a warning.")
#> Warning: WARNING: number of (QCODE) and (/QCODE) tags do not match
#>             in document ; erroneous output is likely.
error_check("A (QCODE) qcode with a missing tag gives a warning.")
#> Warning: WARNING: number of (QCODE) and (/QCODE) tags do not match
#>             in document ; erroneous output is likely.
```
