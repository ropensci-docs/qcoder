# Read data into a project Convenience method to read raw data from standard locations and using standard names in a project folder structure.

Read data into a project Convenience method to read raw data from
standard locations and using standard names in a project folder
structure.

## Usage

``` r
import_project_data(project_name)
```

## Arguments

- project_name:

  The project name. This should represent the folder holding the
  project.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project", sample = TRUE)
import_project_data("_my_qcoder_project")
unlink("./_my_qcoder_project", recursive=TRUE)
```
