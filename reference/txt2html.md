# Format text as HTML Minimal conversion of a text to html

Format text as HTML Minimal conversion of a text to html

## Usage

``` r
txt2html(text)
```

## Arguments

- text:

  text to be converted

## Examples

``` r
txt2html("The quick brown (QCODE)fox(/QCODE){#animal} jumped over ")
#> [1] "<p>The quick brown <mark>fox</mark>{#animal} jumped over </p>"
```
