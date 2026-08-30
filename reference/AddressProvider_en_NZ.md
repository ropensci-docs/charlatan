# AddressProvider for New-Zealand

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
[`AddressProvider_en_US`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_US.md),
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

Other NZ:
[`PersonProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_NZ.md),
[`PhoneNumberProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_NZ.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md)
-\> `AddressProvider_en_NZ`

## Methods

### Public methods

- [`AddressProvider_en_NZ$address()`](#method-AddressProvider_en_NZ-address)

- [`AddressProvider_en_NZ$city()`](#method-AddressProvider_en_NZ-city)

- [`AddressProvider_en_NZ$street_name()`](#method-AddressProvider_en_NZ-street_name)

- [`AddressProvider_en_NZ$street_address()`](#method-AddressProvider_en_NZ-street_address)

- [`AddressProvider_en_NZ$postcode()`](#method-AddressProvider_en_NZ-postcode)

- [`AddressProvider_en_NZ$clone()`](#method-AddressProvider_en_NZ-clone)

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

Create an address, a combination of street, postal code and city.

#### Usage

    AddressProvider_en_NZ$address()

------------------------------------------------------------------------

### Method `city()`

Create a city

#### Usage

    AddressProvider_en_NZ$city()

------------------------------------------------------------------------

### Method `street_name()`

Create a street name

#### Usage

    AddressProvider_en_NZ$street_name()

------------------------------------------------------------------------

### Method `street_address()`

Create a street address , a combination of streetname and house
indicator.

#### Usage

    AddressProvider_en_NZ$street_address()

------------------------------------------------------------------------

### Method `postcode()`

Create a postal code

#### Usage

    AddressProvider_en_NZ$postcode()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    AddressProvider_en_NZ$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
(z <- AddressProvider_en_NZ$new())
#> < AddressProvider >
#> locale: en_NZ
z$postcode()
#> [1] "4921"
z$street_name()
#> [1] "Kawanuku Road"
z$address()
#> [1] "PO Box 88\nNewRange Road 5750"
z$city()
#> [1] "UpperDrive"
```
