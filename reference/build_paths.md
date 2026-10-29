# Build the paths for file creation

Builds the paths to the data to be imported and to the data frame where
the imported data is to be stored. The project name is required, all
other parameters may be set. These each represent a segment of the path
to a file. If a project path is not set or set to "" it will be set to
the current working directory via getwd(). The Shiny qcode application
assumes that the data frame folder will be "data_frames" and that any
new documents to be imported will be in a folder called "documents".

## Usage

``` r
build_paths(
  project_name,
  data_path = "",
  data_frame_name = "",
  df_path = "data_frames",
  project_path = ""
)
```

## Arguments

- project_name:

  Name of the project

- data_path:

  Path segment to the data. The format for this may depend on the
  function using the paths.

- data_frame_name:

  Name of the data frame that will contain the data

- df_path:

  path segment(s) to the created data frame file from the project path

- project_path:

  Path to the project (not including project_name). This will be set to
  getwd() if a value of "" is passed in.

## Value

A named list of paths. "data_frame_path" is the path to the data frame
and "data" is the path to the data.
