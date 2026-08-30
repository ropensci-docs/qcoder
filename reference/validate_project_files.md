# Check for required imported data frames.

Check for required imported data frames.

## Usage

``` r
validate_project_files(path_to_test)
```

## Arguments

- path_to_test:

  Path to possible project folder

## Value

NULL for valid project, Error otherwise.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project", sample = TRUE)
import_project_data("_my_qcoder_project")
validate_project_files("_my_qcoder_project")
unlink("./_my_qcoder_project", recursive=TRUE)
```
