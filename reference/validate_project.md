# Check for a valid qcoder project

Check for a valid qcoder project

## Usage

``` r
validate_project(path_to_test)
```

## Arguments

- path_to_test:

  Path to possible project folder

## Value

NULL for valid project, Error otherwise.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project")
validate_project("_my_qcoder_project")
unlink("./_my_qcoder_project", recursive=TRUE)
```
