# Create an empty codes data set

Used to create a codes data frame with no data but that can have data
added. File is placed in the data_frames folder.

## Usage

``` r
create_empty_code_file(path)
```

## Arguments

- path:

  Full path to data frame to be created.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project")
path <- file.path(getwd(),
  "_my_qcoder_project/data_frames/qcoder_codes__my_qcoder_project")
create_empty_docs_file(path)
unlink("./_my_qcoder_project", recursive=TRUE)
```
