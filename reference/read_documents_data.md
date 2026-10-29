# Create a data frame of documents

Create a data frame of documents

## Usage

``` r
read_documents_data(
  project_name,
  data_path = "documents/",
  df_path = "data_frames",
  data_frame_name = "qcoder_documents",
  project_path = ""
)
```

## Arguments

- project_name:

  Name of the Qcoder project

- data_path:

  path to a folder contain text files to be analyzed.

- df_path:

  Full path to the docs data frame.

- data_frame_name:

  The name of the RDS file that the data frame will be stored in.

- project_path:

  Full path to the project folder.

## Examples

``` r
 if (FALSE) { # \dontrun{
read_documents_data("_my_qcoder_project")
} # }
```
