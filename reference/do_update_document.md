# Update document Updates the text field of the documents data frame, typically after pressing Save button in the Shiny App. May also be used in the console.

Update document Updates the text field of the documents data frame,
typically after pressing Save button in the Shiny App. May also be used
in the console.

## Usage

``` r
do_update_document(updated, docs_df_path, this_doc_path)
```

## Arguments

- updated:

  The updated text as a character string

- docs_df_path:

  Location of the documents rds file.

- this_doc_path:

  Name of record to be updated, as recorded in "doc_path" field of data
  frame.

## Examples

``` r
unlink("./_my_qcoder_project", recursive=TRUE)
```
