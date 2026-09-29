# Create fake Social Security Numbers

Create fake Social Security Numbers

## Usage

``` r
ch_ssn(n = 1, locale = NULL)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. See
  `SSNProvider$new()$allowed_locales()` for locales supported (default:
  en_US)

## See also

[SSNProvider](https://docs.ropensci.org/charlatan/reference/SSNProvider.md)

## Examples

``` r
ch_ssn()
#> [1] "669-09-4259"
ch_ssn(10)
#>  [1] "590-05-8975" "684-52-4862" "885-96-4191" "722-20-0226" "779-91-7411"
#>  [6] "481-72-5579" "248-43-8548" "250-86-5084" "730-20-4009" "349-03-9591"
```
