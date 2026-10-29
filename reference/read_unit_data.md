# Create a data frame of units from csv file Use this is you have a spreadsheet of units already created.

Create a data frame of units from csv file Use this is you have a
spreadsheet of units already created.

## Usage

``` r
read_unit_data(
  data_path = "units/units.csv",
  data_frame_name = "qcoder_units",
  project_name,
  project_path = "",
  df_path = "data_frames"
)
```

## Arguments

- data_path:

  path to a file containing unit data in csv.

- data_frame_name:

  The name of the RDS file that the data frame will be stored in.

- project_name:

  Name of project if available

- project_path:

  Full path to the project folder.

- df_path:

  Full path to the units data frame.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project", sample = TRUE)
read_unit_data(project_name = "_my_qcoder_project")
unlink("./_my_qcoder_project", recursive=TRUE)
```
