# Create a file of codes from csv file Use this if you have a spreadsheet of codes already created.

Create a file of codes from csv file Use this if you have a spreadsheet
of codes already created.

## Usage

``` r
read_code_data(
  project_name,
  data_path = "codes/codes.csv",
  df_path = "data_frames",
  data_frame_name = "qcoder_codes",
  project_path = ""
)
```

## Arguments

- project_name:

  Name of the project, which matches folder name

- data_path:

  Path to a file containing code data in csv.

- df_path:

  Full path to the codes data frame.

- data_frame_name:

  The name of the RDS file that the data frame will be stored in.

- project_path:

  Full path to the project folder

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project", sample = TRUE)
read_code_data(project_name = "_my_qcoder_project")
unlink("./_my_qcoder_project", recursive=TRUE)
```
