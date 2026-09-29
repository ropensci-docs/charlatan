# Fraudster - catch all client to make all types of fake data

Fraudster - catch all client to make all types of fake data

## Usage

``` r
fraudster(locale = NULL)
```

## Arguments

- locale:

  (character) the locale to use. options: en_US (default), fr_FR, fr_CH,
  hr_FR, fa_IR, pl_PL, ru_RU, uk_UA, zh_TW.

## Examples

``` r
# English - the default locale
(x <- fraudster())
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> <fraudster>
#>   locale: en_US
x$job()
#> [1] "Community pharmacist"
x$name()
#> [1] "Mr. Benson Crona PhD"
x$color_name()
#> [1] "DarkBlue"
x$safe_color_name()
#> [1] "olive"
x$hex_color()
#> [1] "#307F6D"
x$safe_hex_color()
#> [1] "#ffcc33"
x$rgb_color()
#> [[1]]
#> [1]  97   9 212
#> 
x$rgb_css_color()
#> [1] "rgb(233, 13, 3)"

# different locales
## French
(y <- fraudster(locale = "fr_FR"))
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning:  LoremProvider does not have locale fr_FR, defaulting to en_US locale.
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> <fraudster>
#>   locale: fr_FR
y$job()
#> [1] "Ethnologue"

## Croatian
(z <- fraudster(locale = "hr_HR"))
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning:  LoremProvider does not have locale hr_HR, defaulting to en_US locale.
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> <fraudster>
#>   locale: hr_HR
z$job()
#> [1] "Hidrograđevinski  inspektor"

## Ukranian
(w <- fraudster(locale = "uk_UA"))
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> <fraudster>
#>   locale: uk_UA
w$job()
#> [1] "Музикант"
w$color_name()
#> [1] "Аквамариновий"

# geospatial
x$lat()
#> [1] 66.21565
x$lon()
#> [1] 33.72385
x$position()
#>           [,1]
#> [1,] -27.67296
#> [2,]  78.83574

# DOIs (Digital Object Identifier)
x$doi()
#> [1] "10.77043/ydsf.14494714"
```
