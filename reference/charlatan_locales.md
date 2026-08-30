# Available locales

Available locales

## Usage

``` r
charlatan_locales()
```

## Value

a data.frame of the available locales in this package. See
[available_locales_df](https://docs.ropensci.org/charlatan/reference/available_locales_df.md)
for structure.

Not all functions support all locales. Check the docs for each one to
see what locales they support.

You can find out more about each locale by running your locale though
[`stringi::stri_locale_info()`](https://rdrr.io/pkg/stringi/man/stri_locale_info.html)

## Examples

``` r
charlatan_locales()
#>    Language Country Variant  Name
#> 1        ar      AA         ar_AA
#> 2        bg      BG         bg_BG
#> 3        bs      BA         bs_BA
#> 4        cs      CZ         cs_CZ
#> 5        da      DK         da_DK
#> 6        dk      DK         dk_DK
#> 7        de      AT         de_AT
#> 8        de      DE         de_DE
#> 9        el      GR         el_GR
#> 10       en                    en
#> 11       en      AU         en_AU
#> 12       en      CA         en_CA
#> 13       en      GB         en_GB
#> 14       en      US         en_US
#> 15       en      NZ         en_NZ
#> 16       es                    es
#> 17       es      ES         es_ES
#> 18       es      MX         es_MX
#> 19       es      PE         es_PE
#> 20       fa      IR         fa_IR
#> 21       fi      FI         fi_FI
#> 22       fr      CH         fr_CH
#> 23       fr      FR         fr_FR
#> 24       he      IL         he_IL
#> 25       hi      IN         hi_IN
#> 26       hr      HR         hr_HR
#> 27       hu      HU         hu_HU
#> 28       id      ID         id_ID
#> 29       it      IT         it_IT
#> 30       ja      JP         ja_JP
#> 31       ko      KR         ko_KR
#> 32       la                    la
#> 33       lt      LT         lt_LT
#> 34       lv      LV         lv_LV
#> 35       ne      NP         ne_NP
#> 36       nl      BE         nl_BE
#> 37       nl      NL         nl_NL
#> 38       no      NO         no_NO
#> 39       nn      NO         nn_NO
#> 40       pl      PL         pl_PL
#> 41       pt      BR         pt_BR
#> 42       pt      PT         pt_PT
#> 43       ru      RU         ru_RU
#> 44       sk      SK         sk_SK
#> 45       sl      SL         sl_SL
#> 46       sv      SE         sv_SE
#> 47       th      TH         th_TH
#> 48       tr      TR         tr_TR
#> 49       tw      GH         tw_GH
#> 50       uk      UA         uk_UA
#> 51       zh      CN         zh_CN
#> 52       zh      TW         zh_TW
```
