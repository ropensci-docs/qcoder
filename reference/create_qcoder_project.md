# Create a standard set of folders for a QCoder project

Create a standard set of folders for a QCoder project

## Usage

``` r
create_qcoder_project(project_name, sample = FALSE)
```

## Arguments

- project_name:

  A string project name to be located in the current working directory
  or a path to a project folder.

- sample:

  Logical that indicates that the sample data should be copied to the
  project.

## Examples

``` r
create_qcoder_project(project_name = "my_qcoder_project")
unlink("./my_qcoder_project", recursive=TRUE)
```
