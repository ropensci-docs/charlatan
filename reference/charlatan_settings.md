# charlatan settings

charlatan settings

## Usage

``` r
charlatan_settings(messy = NULL)
```

## Arguments

- messy:

  (logical) make some messy data. Default: `NULL`

## More deets

- `messy` - When `FALSE`, nothing is different from normal. When `TRUE`,
  we select incorrect/wrong values with probability X. Messy mode is
  only available for **en-US** for now, and only for some data types.
  The default setting is `NULL`, meaning it is ignored.

## Examples

``` r
charlatan_settings()
#> $global_messy
#> NULL
#> 
charlatan_settings(messy = TRUE)
#> $global_messy
#> [1] TRUE
#> 
charlatan_settings(messy = FALSE)
#> $global_messy
#> [1] FALSE
#> 

# with PersonProvider - overrides local messy param in all cases
x <- PersonProvider_en_US$new()
x$messy
#> [1] FALSE
charlatan_settings(messy = TRUE)
#> $global_messy
#> [1] TRUE
#> 
x <- PersonProvider_en_US$new()
#> Warning: Global setting for messy is TRUE
x$messy
#> [1] TRUE
```
