# Define an empty many to many unit to document map

Define an empty many to many unit to document map

## Usage

``` r
create_empty_unit_doc_file(path)
```

## Arguments

- path:

  Full path to data frame to be created.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project")
path <- file.path(getwd(),
  "_my_qcoder_project/data_frames/qcoder_units_document_map__my_qcoder_project")
create_empty_docs_file(path)
unlink("./_my_qcoder_project", recursive=TRUE)
```
