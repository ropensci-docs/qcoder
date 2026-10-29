# Define an empty units data frame

Define an empty units data frame

## Usage

``` r
create_empty_units_file(path)
```

## Arguments

- path:

  Full path to data frame to be created.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project")
path <- file.path(getwd(),
  "_my_qcoder_project/data_frames/qcoder_units__my_qcoder_project")
create_empty_docs_file(path)
unlink("./_my_qcoder_project", recursive=TRUE)
```
