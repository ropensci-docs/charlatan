# MiscProvider

miscellaneous methods

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `MiscProvider`

## Active bindings

- `language_locale_codes`:

  (list) locale codes by locale family

## Methods

### Public methods

- [`MiscProvider$boolean()`](#method-MiscProvider-boolean)

- [`MiscProvider$null_boolean()`](#method-MiscProvider-null_boolean)

- [`MiscProvider$locale()`](#method-MiscProvider-locale)

- [`MiscProvider$language_code()`](#method-MiscProvider-language_code)

- [`MiscProvider$clone()`](#method-MiscProvider-clone)

Inherited methods

- [`charlatan::BareProvider$bothify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-bothify)
- [`charlatan::BareProvider$lexify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-lexify)
- [`charlatan::BareProvider$numerify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-numerify)
- [`charlatan::BareProvider$print()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-print)
- [`charlatan::BareProvider$random_digit()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit)
- [`charlatan::BareProvider$random_digit_not_zero()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero)
- [`charlatan::BareProvider$random_digit_not_zero_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero_or_empty)
- [`charlatan::BareProvider$random_digit_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_or_empty)
- [`charlatan::BareProvider$random_element()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element)
- [`charlatan::BareProvider$random_element_prob()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element_prob)
- [`charlatan::BareProvider$random_int()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_int)
- [`charlatan::BareProvider$random_letter()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_letter)
- [`charlatan::BareProvider$randomize_nb_elements()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-randomize_nb_elements)

------------------------------------------------------------------------

### Method `boolean()`

get a random boolean, `TRUE` or `FALSE`

#### Usage

    MiscProvider$boolean(chance_of_getting_true = 50)

#### Arguments

- `chance_of_getting_true`:

  (integer) an integer, default: 50

------------------------------------------------------------------------

### Method `null_boolean()`

get a random boolean, `TRUE` or `FALSE`, or NULL

#### Usage

    MiscProvider$null_boolean()

------------------------------------------------------------------------

### Method `locale()`

get a random locale

#### Usage

    MiscProvider$locale()

------------------------------------------------------------------------

### Method `language_code()`

random language code

#### Usage

    MiscProvider$language_code()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    MiscProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
(x <- MiscProvider$new())
#> < MiscProvider >
x$language_locale_codes
#> $aa
#> [1] "DJ" "ER" "ET"
#> 
#> $af
#> [1] "ZA"
#> 
#> $ak
#> [1] "GH"
#> 
#> $am
#> [1] "ET"
#> 
#> $an
#> [1] "ES"
#> 
#> $apn
#> [1] "IN"
#> 
#> $ar
#>  [1] "AE" "BH" "DJ" "DZ" "EG" "EH" "ER" "IL" "IN" "IQ" "JO" "KM" "KW" "LB" "LY"
#> [16] "MA" "MR" "OM" "PS" "QA" "SA" "SD" "SO" "SS" "SY" "TD" "TN" "YE"
#> 
#> $as
#> [1] "IN"
#> 
#> $ast
#> [1] "ES"
#> 
#> $ayc
#> [1] "PE"
#> 
#> $az
#> [1] "AZ" "IN"
#> 
#> $be
#> [1] "BY"
#> 
#> $bem
#> [1] "ZM"
#> 
#> $ber
#> [1] "DZ" "MA"
#> 
#> $bg
#> [1] "BG"
#> 
#> $bhb
#> [1] "IN"
#> 
#> $bho
#> [1] "IN"
#> 
#> $bn
#> [1] "BD" "IN"
#> 
#> $bo
#> [1] "CN" "IN"
#> 
#> $br
#> [1] "FR"
#> 
#> $brx
#> [1] "IN"
#> 
#> $bs
#> [1] "BA"
#> 
#> $byn
#> [1] "ER"
#> 
#> $ca
#> [1] "AD" "ES" "FR" "IT"
#> 
#> $ce
#> [1] "RU"
#> 
#> $ckb
#> [1] "IQ"
#> 
#> $cmn
#> [1] "TW"
#> 
#> $crh
#> [1] "UA"
#> 
#> $cs
#> [1] "CZ"
#> 
#> $csb
#> [1] "PL"
#> 
#> $cv
#> [1] "RU"
#> 
#> $cy
#> [1] "GB"
#> 
#> $da
#> [1] "DK"
#> 
#> $de
#> [1] "AT" "BE" "CH" "DE" "LI" "LU"
#> 
#> $doi
#> [1] "IN"
#> 
#> $dv
#> [1] "MV"
#> 
#> $dz
#> [1] "BT"
#> 
#> $el
#> [1] "GR" "CY"
#> 
#> $en
#>  [1] "AG" "AU" "BW" "CA" "DK" "GB" "HK" "IE" "IN" "NG" "NZ" "PH" "SG" "US" "ZA"
#> [16] "ZM" "ZW"
#> 
#> $eo
#> [1] "US"
#> 
#> $es
#>  [1] "AR" "BO" "CL" "CO" "CR" "CU" "DO" "EC" "ES" "GT" "HN" "MX" "NI" "PA" "PE"
#> [16] "PR" "PY" "SV" "US" "UY" "VE"
#> 
#> $et
#> [1] "EE"
#> 
#> $eu
#> [1] "ES" "FR"
#> 
#> $fa
#> [1] "IR"
#> 
#> $ff
#> [1] "SN"
#> 
#> $fi
#> [1] "FI"
#> 
#> $fil
#> [1] "PH"
#> 
#> $fo
#> [1] "FO"
#> 
#> $fr
#> [1] "CA" "CH" "FR" "LU"
#> 
#> $fur
#> [1] "IT"
#> 
#> $fy
#> [1] "NL" "DE"
#> 
#> $ga
#> [1] "IE"
#> 
#> $gd
#> [1] "GB"
#> 
#> $gez
#> [1] "ER" "ET"
#> 
#> $gl
#> [1] "ES"
#> 
#> $gu
#> [1] "IN"
#> 
#> $gv
#> [1] "GB"
#> 
#> $ha
#> [1] "NG"
#> 
#> $hak
#> [1] "TW"
#> 
#> $he
#> [1] "IL"
#> 
#> $hi
#> [1] "IN"
#> 
#> $hne
#> [1] "IN"
#> 
#> $hr
#> [1] "HR"
#> 
#> $hsb
#> [1] "DE"
#> 
#> $ht
#> [1] "HT"
#> 
#> $hu
#> [1] "HU"
#> 
#> $hy
#> [1] "AM"
#> 
#> $ia
#> [1] "FR"
#> 
#> $id
#> [1] "ID"
#> 
#> $ig
#> [1] "NG"
#> 
#> $ik
#> [1] "CA"
#> 
#> $is
#> [1] "IS"
#> 
#> $it
#> [1] "CH" "IT"
#> 
#> $iu
#> [1] "CA"
#> 
#> $iw
#> [1] "IL"
#> 
#> $ja
#> [1] "JP"
#> 
#> $ka
#> [1] "GE"
#> 
#> $kk
#> [1] "KZ"
#> 
#> $kl
#> [1] "GL"
#> 
#> $km
#> [1] "KH"
#> 
#> $kn
#> [1] "IN"
#> 
#> $ko
#> [1] "KR"
#> 
#> $kok
#> [1] "IN"
#> 
#> $ks
#> [1] "IN"
#> 
#> $ku
#> [1] "TR"
#> 
#> $kw
#> [1] "GB"
#> 
#> $ky
#> [1] "KG"
#> 
#> $lb
#> [1] "LU"
#> 
#> $lg
#> [1] "UG"
#> 
#> $li
#> [1] "BE" "NL"
#> 
#> $lij
#> [1] "IT"
#> 
#> $ln
#> [1] "CD"
#> 
#> $lo
#> [1] "LA"
#> 
#> $lt
#> [1] "LT"
#> 
#> $lv
#> [1] "LV"
#> 
#> $lzh
#> [1] "TW"
#> 
#> $mag
#> [1] "IN"
#> 
#> $mai
#> [1] "IN"
#> 
#> $mg
#> [1] "MG"
#> 
#> $mhr
#> [1] "RU"
#> 
#> $mi
#> [1] "NZ"
#> 
#> $mk
#> [1] "MK"
#> 
#> $ml
#> [1] "IN"
#> 
#> $mn
#> [1] "MN"
#> 
#> $mni
#> [1] "IN"
#> 
#> $mr
#> [1] "IN"
#> 
#> $ms
#> [1] "MY"
#> 
#> $mt
#> [1] "MT"
#> 
#> $my
#> [1] "MM"
#> 
#> $nan
#> [1] "TW"
#> 
#> $nb
#> [1] "NO"
#> 
#> $nds
#> [1] "DE" "NL"
#> 
#> $ne
#> [1] "NP"
#> 
#> $nhn
#> [1] "MX"
#> 
#> $niu
#> [1] "NU" "NZ"
#> 
#> $nl
#> [1] "AW" "BE" "NL"
#> 
#> $nn
#> [1] "NO"
#> 
#> $nr
#> [1] "ZA"
#> 
#> $nso
#> [1] "ZA"
#> 
#> $oc
#> [1] "FR"
#> 
#> $om
#> [1] "ET" "KE"
#> 
#> $or
#> [1] "IN"
#> 
#> $os
#> [1] "RU"
#> 
#> $pa
#> [1] "IN" "PK"
#> 
#> $pap
#> [1] "AN" "AW" "CW"
#> 
#> $pl
#> [1] "PL"
#> 
#> $ps
#> [1] "AF"
#> 
#> $pt
#> [1] "BR" "PT"
#> 
#> $quz
#> [1] "PE"
#> 
#> $raj
#> [1] "IN"
#> 
#> $ro
#> [1] "RO"
#> 
#> $ru
#> [1] "RU" "UA"
#> 
#> $rw
#> [1] "RW"
#> 
#> $sa
#> [1] "IN"
#> 
#> $sat
#> [1] "IN"
#> 
#> $sc
#> [1] "IT"
#> 
#> $sd
#> [1] "IN" "PK"
#> 
#> $se
#> [1] "NO"
#> 
#> $shs
#> [1] "CA"
#> 
#> $si
#> [1] "LK"
#> 
#> $sid
#> [1] "ET"
#> 
#> $sk
#> [1] "SK"
#> 
#> $sl
#> [1] "SI"
#> 
#> $so
#> [1] "DJ" "ET" "KE" "SO"
#> 
#> $sq
#> [1] "AL" "ML"
#> 
#> $sr
#> [1] "ME" "RS"
#> 
#> $ss
#> [1] "ZA"
#> 
#> $st
#> [1] "ZA"
#> 
#> $sv
#> [1] "FI" "SE"
#> 
#> $sw
#> [1] "KE" "TZ"
#> 
#> $szl
#> [1] "PL"
#> 
#> $ta
#> [1] "IN" "LK"
#> 
#> $tcy
#> [1] "IN"
#> 
#> $te
#> [1] "IN"
#> 
#> $tg
#> [1] "TJ"
#> 
#> $th
#> [1] "TH"
#> 
#> $the
#> [1] "NP"
#> 
#> $ti
#> [1] "ER" "ET"
#> 
#> $tig
#> [1] "ER"
#> 
#> $tk
#> [1] "TM"
#> 
#> $tl
#> [1] "PH"
#> 
#> $tn
#> [1] "ZA"
#> 
#> $tr
#> [1] "CY" "TR"
#> 
#> $ts
#> [1] "ZA"
#> 
#> $tt
#> [1] "RU"
#> 
#> $ug
#> [1] "CN"
#> 
#> $uk
#> [1] "UA"
#> 
#> $unm
#> [1] "US"
#> 
#> $ur
#> [1] "IN" "PK"
#> 
#> $uz
#> [1] "UZ"
#> 
#> $ve
#> [1] "ZA"
#> 
#> $vi
#> [1] "VN"
#> 
#> $wa
#> [1] "BE"
#> 
#> $wae
#> [1] "CH"
#> 
#> $wal
#> [1] "ET"
#> 
#> $wo
#> [1] "SN"
#> 
#> $xh
#> [1] "ZA"
#> 
#> $yi
#> [1] "US"
#> 
#> $yo
#> [1] "NG"
#> 
#> $yue
#> [1] "HK"
#> 
#> $zh
#> [1] "CN" "HK" "SG" "TW"
#> 
#> $zu
#> [1] "ZA"
#> 
x$language_code()
#> [1] "mhr"
x$locale()
#> [1] "es_PA"
x$boolean()
#> [1] TRUE
x$null_boolean()
#> [1] TRUE
```
