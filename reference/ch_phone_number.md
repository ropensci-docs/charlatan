# Create fake phone numbers

Create fake phone numbers

## Usage

``` r
ch_phone_number(n = 1, locale = NULL)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. See
  `PhoneNumberProvider$new()$allowed_locales()` for locales supported
  (default: en_US)

## See also

[PhoneNumberProvider](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md)

## Examples

``` r
ch_phone_number()
#> [1] "1-433-163-3748"
ch_phone_number(10)
#>  [1] "918-025-9081x273"   "(001)882-4982"      "449.113.1432x709"  
#>  [4] "08869721900"        "1-901-592-4465"     "191.082.6414x11943"
#>  [7] "744.094.5364x1767"  "852.176.6450"       "02076422743"       
#> [10] "+25(8)1549965053"  
# or even ch_phone_number(500)

# locales
ch_phone_number(locale = "fr_FR")
#> [1] "+33 2 47 55 49 18"
ch_phone_number(locale = "uk_UA")
#> [1] "069 313 63 16"
ch_phone_number(locale = "en_CA")
#> [1] "(264) 680-9195"
ch_phone_number(locale = "lv_LV")
#> [1] "+371 62320909"
```
