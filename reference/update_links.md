# Update document to unit links Saves or updates the links between observation units and documents

Update document to unit links Saves or updates the links between
observation units and documents

## Usage

``` r
update_links(
  checked = "",
  docs_df_path = "",
  this_doc_path = "",
  units_docs_path = ""
)
```

## Arguments

- checked:

  vector of new or updated links

- docs_df_path:

  full path to document dataset

- this_doc_path:

  value of doc_path for the document

- units_docs_path:

  full path of the data frame of unit to docs links

## Examples

``` r

unlink("./_my_qcoder_project", recursive=TRUE)
```
