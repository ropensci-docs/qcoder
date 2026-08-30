# Parse one document

Parse one document

## Usage

``` r
parse_one_document(doc, df, qcoder_documents, dots = NULL)
```

## Arguments

- doc:

  A single document from qcoder_data

- df:

  The data frame that will contain the parsed data

- qcoder_documents:

  The full documents data frame

- dots:

  Other parameters that may be passed in.

## Examples

``` r
unlink("./my_qcoder_project", recursive=TRUE)
```
