# Add code Append a new unit record to the existing data frame

Add code Append a new unit record to the existing data frame

## Usage

``` r
add_code(codes_df, new_code, new_code_desc, codes_df_path)
```

## Arguments

- codes_df:

  Existing codes data frame

- new_code:

  text name of a new code (single name only)

- new_code_desc:

  text description of the code

- codes_df_path:

  full path to the codes data frame

## Examples

``` r
unlink("./_my_qcoder_project", recursive=TRUE)
```
