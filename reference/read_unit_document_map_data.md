# Create a data frame of unit to document links from csv file Use this is you have a spreadsheet already created.

Create a data frame of unit to document links from csv file Use this is
you have a spreadsheet already created.

## Usage

``` r
read_unit_document_map_data(
  project_name,
  data_path = "units/unit_document_map.csv",
  data_frame_name = "qcoder_unit_document_map",
  project_path = "",
  df_path = "data_frames"
)
```

## Arguments

- project_name:

  Name of project

- data_path:

  path to a file containing unit document map data in csv.

- data_frame_name:

  The name of the RDS file that the data frame will be stored in.

- project_path:

  Full path to the project folder

- df_path:

  Full path to the documents data frame.

## Examples

``` r
create_qcoder_project(project_name = "_my_qcoder_project", sample = TRUE)
project_name = "_my_qcoder_project"
read_unit_document_map_data( project_name = "_my_qcoder_project")
unlink("./_my_qcoder_project", recursive=TRUE)
```
