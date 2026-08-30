# Add new documents Adds new document or documents to an existing documents data frame.

Add new documents Adds new document or documents to an existing
documents data frame.

## Usage

``` r
add_new_documents(files, docs_df_path = "", file_path = "")
```

## Arguments

- files:

  Vector of new files to be added

- docs_df_path:

  Path to existing data frame of text documents

- file_path:

  Full path to the data set of documents including trailing slash

## Examples

``` r
create_qcoder_project(project_name = "my_qcoder_project", sample = TRUE)

unlink("./my_qcoder_project", recursive=TRUE)
```
