# Create fake credit card data

Create fake credit card data

## Usage

``` r
ch_credit_card_provider(n = 1)

ch_credit_card_number(n = 1)

ch_credit_card_security_code(n = 1)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

## See also

[CreditCardProvider](https://docs.ropensci.org/charlatan/reference/CreditCardProvider.md)

## Examples

``` r
ch_credit_card_provider()
#> [1] "VISA 16 digit"
ch_credit_card_provider(n = 4)
#> [1] "JCB 15 digit"                "Diners Club / Carte Blanche"
#> [3] "Discover"                    "Mastercard"                 

ch_credit_card_number()
#> [1] "4578098147398248"
ch_credit_card_number(n = 10)
#>  [1] "4292927380462"       "675949584223470"     "4217020959413995"   
#>  [4] "55924315472483093"   "4316420166043"       "4734700194552"      
#>  [7] "6011643471500429416" "3402000298770080"    "3088656282559777710"
#> [10] "639036126207681"    
# or even ch_credit_card_number(n = 500)

ch_credit_card_security_code()
#> [1] "722"
ch_credit_card_security_code(n = 10)
#>  [1] "808"  "873"  "609"  "9644" "386"  "480"  "287"  "101"  "693"  "2707"
# or even ch_credit_card_security_code(n = 500)
```
