# AddressProvider for United States of America

Object to create addresses for a locale. Makes use of
[PersonProvider](https://docs.ropensci.org/charlatan/reference/PersonProvider.md)
for creating street names.

## Value

Returns an AddressProvider object.

## Details

When there is no PersonProvider for this locale, we default back to
en_US.

## See also

Other en:
[`AddressProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_GB.md),
[`AddressProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_NZ.md),
[`ColorProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ColorProvider_en_US.md),
[`CompanyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md),
[`ElementProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ElementProvider_en_US.md),
[`FileProvider_en_US`](https://docs.ropensci.org/charlatan/reference/FileProvider_en_US.md),
[`InternetProvider_en_AU`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_AU.md),
[`InternetProvider_en_US`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_US.md),
[`JobProvider_en_US`](https://docs.ropensci.org/charlatan/reference/JobProvider_en_US.md),
[`LoremProvider_en_US`](https://docs.ropensci.org/charlatan/reference/LoremProvider_en_US.md),
[`PersonProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_GB.md),
[`PersonProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_NZ.md),
[`PersonProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_US.md),
[`PhoneNumberProvider_en_AU`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_AU.md),
[`PhoneNumberProvider_en_CA`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_CA.md),
[`PhoneNumberProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_GB.md),
[`PhoneNumberProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_NZ.md),
[`PhoneNumberProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_US.md),
[`PhoneNumberProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_MX.md),
[`SSNProvider_en_US`](https://docs.ropensci.org/charlatan/reference/SSNProvider_en_US.md),
[`TaxonomyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider_en_US.md),
[`UserAgentProvider_en_US`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider_en_US.md),
[`english-language`](https://docs.ropensci.org/charlatan/reference/english-language.md)

Other US:
[`ColorProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ColorProvider_en_US.md),
[`CompanyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md),
[`ElementProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ElementProvider_en_US.md),
[`FileProvider_en_US`](https://docs.ropensci.org/charlatan/reference/FileProvider_en_US.md),
[`InternetProvider_en_US`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_US.md),
[`JobProvider_en_US`](https://docs.ropensci.org/charlatan/reference/JobProvider_en_US.md),
[`LoremProvider_en_US`](https://docs.ropensci.org/charlatan/reference/LoremProvider_en_US.md),
[`PersonProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_US.md),
[`PhoneNumberProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_US.md),
[`SSNProvider_en_US`](https://docs.ropensci.org/charlatan/reference/SSNProvider_en_US.md),
[`TaxonomyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider_en_US.md),
[`UserAgentProvider_en_US`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider_en_US.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md)
-\> `AddressProvider_en_US`

## Methods

### Public methods

- [`AddressProvider_en_US$address()`](#method-AddressProvider_en_US-address)

- [`AddressProvider_en_US$civ_address()`](#method-AddressProvider_en_US-civ_address)

- [`AddressProvider_en_US$mil_address()`](#method-AddressProvider_en_US-mil_address)

- [`AddressProvider_en_US$city()`](#method-AddressProvider_en_US-city)

- [`AddressProvider_en_US$street_name()`](#method-AddressProvider_en_US-street_name)

- [`AddressProvider_en_US$street_address()`](#method-AddressProvider_en_US-street_address)

- [`AddressProvider_en_US$postcode()`](#method-AddressProvider_en_US-postcode)

- [`AddressProvider_en_US$building_number()`](#method-AddressProvider_en_US-building_number)

- [`AddressProvider_en_US$state()`](#method-AddressProvider_en_US-state)

- [`AddressProvider_en_US$clone()`](#method-AddressProvider_en_US-clone)

Inherited methods

- [`charlatan::BareProvider$bothify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-bothify)
- [`charlatan::BareProvider$lexify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-lexify)
- [`charlatan::BareProvider$numerify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-numerify)
- [`charlatan::BareProvider$random_digit()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit)
- [`charlatan::BareProvider$random_digit_not_zero()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero)
- [`charlatan::BareProvider$random_digit_not_zero_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero_or_empty)
- [`charlatan::BareProvider$random_digit_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_or_empty)
- [`charlatan::BareProvider$random_element()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element)
- [`charlatan::BareProvider$random_element_prob()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element_prob)
- [`charlatan::BareProvider$random_int()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_int)
- [`charlatan::BareProvider$random_letter()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_letter)
- [`charlatan::BareProvider$randomize_nb_elements()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-randomize_nb_elements)
- [`charlatan::BaseProvider$allowed_locales()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-allowed_locales)
- [`charlatan::BaseProvider$check_locale()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-check_locale)
- [`charlatan::BaseProvider$print()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-print)
- [`charlatan::AddressProvider$init_person_provider()`](https://docs.ropensci.org/charlatan/reference/AddressProvider.html#method-init_person_provider)
- [`charlatan::AddressProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/AddressProvider.html#method-initialize)

------------------------------------------------------------------------

### Method `address()`

address

#### Usage

    AddressProvider_en_US$address()

------------------------------------------------------------------------

### Method `civ_address()`

civilian address, the type of address you would expect. Not to be
confused with Military address which is also available for this locale.

#### Usage

    AddressProvider_en_US$civ_address()

------------------------------------------------------------------------

### Method `mil_address()`

Military address

#### Usage

    AddressProvider_en_US$mil_address()

------------------------------------------------------------------------

### Method `city()`

city

#### Usage

    AddressProvider_en_US$city()

------------------------------------------------------------------------

### Method `street_name()`

street name

#### Usage

    AddressProvider_en_US$street_name()

------------------------------------------------------------------------

### Method `street_address()`

street address

#### Usage

    AddressProvider_en_US$street_address()

------------------------------------------------------------------------

### Method `postcode()`

postal code

#### Usage

    AddressProvider_en_US$postcode()

------------------------------------------------------------------------

### Method `building_number()`

building number

#### Usage

    AddressProvider_en_US$building_number()

------------------------------------------------------------------------

### Method `state()`

state

#### Usage

    AddressProvider_en_US$state()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    AddressProvider_en_US$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
(z <- AddressProvider_en_US$new())
#> < AddressProvider >
#> locale: en_US
z$locale
#> [1] "en_US"
z$postcode()
#> [1] "28584"
z$street_name()
#> [1] "Vincenzo Shoal"
z$address()
#> [1] "8122 Kassulke Causeway Suite 643\nNorth Lolitaburgh, MI 69750-3154"
z$city()
#> [1] "West Zoe"
z$mil_address()
#> [1] "PSC 1842, Box 1493\nAPO AA 89828"
z$civ_address()
#> [1] "06483 Durrell Forest\nSporerton, CO 90491-8806"
```
