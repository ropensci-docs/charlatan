# Create fake currencies

Create fake currencies

## Usage

``` r
ch_currency(n = 1)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

## See also

[CurrencyProvider](https://docs.ropensci.org/charlatan/reference/CurrencyProvider.md)

## Examples

``` r
ch_currency()
#> [1] "GHS"
ch_currency(10)
#>  [1] "DZD" "MZN" "MVR" "PGK" "CZK" "SOS" "TJS" "LYD" "ALL" "TJS"
# or even ch_currency(500)
```
