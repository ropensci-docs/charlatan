# AddressProvider for The Netherlands

Object to create addresses for a locale. Makes use of
[PersonProvider](https://docs.ropensci.org/charlatan/reference/PersonProvider.md)
for creating street names.

## Value

Returns an AddressProvider object.

## Details

When there is no PersonProvider for this locale, we default back to
en_US.

## See also

Other nl:
[`ElementProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/ElementProvider_nl_NL.md),
[`JobProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/JobProvider_nl_NL.md),
[`PersonProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/PersonProvider_nl_NL.md),
[`PhoneNumberProvider_nl_BE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_nl_BE.md),
[`PhoneNumberProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_nl_NL.md),
[`SSNProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/SSNProvider_nl_NL.md),
[`dutch-language`](https://docs.ropensci.org/charlatan/reference/dutch-language.md)

Other NL:
[`ElementProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/ElementProvider_nl_NL.md),
[`JobProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/JobProvider_nl_NL.md),
[`PersonProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/PersonProvider_nl_NL.md),
[`PhoneNumberProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_nl_NL.md),
[`SSNProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/SSNProvider_nl_NL.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md)
-\> `AddressProvider_nl_NL`

## Methods

### Public methods

- [`AddressProvider_nl_NL$address()`](#method-AddressProvider_nl_NL-address)

- [`AddressProvider_nl_NL$city()`](#method-AddressProvider_nl_NL-city)

- [`AddressProvider_nl_NL$street_name()`](#method-AddressProvider_nl_NL-street_name)

- [`AddressProvider_nl_NL$street_address()`](#method-AddressProvider_nl_NL-street_address)

- [`AddressProvider_nl_NL$postcode()`](#method-AddressProvider_nl_NL-postcode)

- [`AddressProvider_nl_NL$building_number()`](#method-AddressProvider_nl_NL-building_number)

- [`AddressProvider_nl_NL$province()`](#method-AddressProvider_nl_NL-province)

- [`AddressProvider_nl_NL$clone()`](#method-AddressProvider_nl_NL-clone)

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

Create an address, a combination of street, postal code and city. The
three components street, postal code and city are generated
independently, so they are not related.

#### Usage

    AddressProvider_nl_NL$address()

------------------------------------------------------------------------

### Method `city()`

Create a city

#### Usage

    AddressProvider_nl_NL$city()

------------------------------------------------------------------------

### Method `street_name()`

Create a street name

#### Usage

    AddressProvider_nl_NL$street_name()

------------------------------------------------------------------------

### Method `street_address()`

Create a street address, a combination of streetname and house
indicator.

#### Usage

    AddressProvider_nl_NL$street_address()

------------------------------------------------------------------------

### Method `postcode()`

Create a postal code, does not exclude impossible postcodes in The
Netherlands (leading zero for examples) but looks good enough for most
purposes.

#### Usage

    AddressProvider_nl_NL$postcode()

------------------------------------------------------------------------

### Method `building_number()`

building number.

#### Usage

    AddressProvider_nl_NL$building_number()

------------------------------------------------------------------------

### Method `province()`

Create a province.

#### Usage

    AddressProvider_nl_NL$province()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    AddressProvider_nl_NL$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
(z <- AddressProvider_nl_NL$new())
#> < AddressProvider >
#> locale: nl_NL
z$locale
#> [1] "nl_NL"
z$postcode()
#> [1] "3088 JQ"
z$street_name()
#> [1] "Kayleestraat"
z$address()
#> [1] "Arienshof 199\n2077 DV Sepptrecht"
z$city()
#> [1] "Masonmeren"
z$province()
#> [1] "Zuid-Holland"
```
