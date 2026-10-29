# Parse coded text

Take a data frame of coded text documents and return a data frame of the
codes captured within.

## Usage

``` r
parse_qcodes(x, ...)
```

## Arguments

- x:

  A data frame containing the text to be coded; requires columns
  "doc_id" and "document_text"

- ...:

  Other parameters optionally passed in

## Value

If the data frame contains coded text in the `document_text` column,
output will be a data frame with three columns: "doc", "qcode", and
"text".

        The "doc" column is the corresponding "doc_id" value from the input
        data frame.

        "qcode" is the code that the captured text was marked up with.

        "text" is the text that was captured.

## Details

This function takes a text document containing coded text of the form:

    "stuff to ignore (QCODE) coded text we care about (/QCODE){#my_code}
    more stuff to ignore"

and turns it into a data frame with one row per coded item, of the form:
`docid,qcode,text`

`parse_qcodes` assumes that it is being passed a data frame, the
[`parse_one_document`](https://docs.ropensci.org/qcoder/reference/parse_one_document.md)
function is called to do the heavy lifting extracting the coded text
from the `document_text` column.

Newline characters are replaced with an HTML `<br>` in the captured
text.

If no valid qcodes are found, `parse_qcodes` returns an empty data frame
(no rows).

## Examples

``` r
my_documents <- data.frame("doc_id" = 1, "document_text" =
"(QCODE)Parts of above text is licensed {CC BY-SA 4.0}.(/QCODE){#license} Credit to SRCCON.
","doc_path" = "mypath.txt")
parse_qcodes(my_documents)
#>   doc   qcode                                            text
#> 1   1 license Parts of above text is licensed {CC BY-SA 4.0}.
```
