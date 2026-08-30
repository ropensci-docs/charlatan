# AddressProvider

Object to create addresses for a locale. Makes use of
[PersonProvider](https://docs.ropensci.org/charlatan/reference/PersonProvider.md)
for creating street names.

## Value

Returns an AddressProvider object.

## Details

When there is no PersonProvider for this locale, we default back to
en_US.

## Note

You cannot instantiate the Parent providers. You must use one of the
localized one.

## See also

Other ParentProviders:
[`ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
[`InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md),
[`JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md),
[`LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md),
[`PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md),
[`PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md),
[`TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md),
[`UserAgentProvider`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `AddressProvider`

## Methods

### Public methods

- [`AddressProvider$new()`](#method-AddressProvider-new)

- [`AddressProvider$address()`](#method-AddressProvider-address)

- [`AddressProvider$city()`](#method-AddressProvider-city)

- [`AddressProvider$street_name()`](#method-AddressProvider-street_name)

- [`AddressProvider$street_address()`](#method-AddressProvider-street_address)

- [`AddressProvider$postcode()`](#method-AddressProvider-postcode)

- [`AddressProvider$init_person_provider()`](#method-AddressProvider-init_person_provider)

- [`AddressProvider$clone()`](#method-AddressProvider-clone)

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

------------------------------------------------------------------------

### Method `new()`

Create a new `AddressProvider` object

#### Usage

    AddressProvider$new()

#### Returns

A new `AddressProvider` object

------------------------------------------------------------------------

### Method `address()`

Create an address, a combination of street, postal code and city.

#### Usage

    AddressProvider$address()

------------------------------------------------------------------------

### Method `city()`

Create a city

#### Usage

    AddressProvider$city()

------------------------------------------------------------------------

### Method `street_name()`

Create a street name.

#### Usage

    AddressProvider$street_name()

------------------------------------------------------------------------

### Method `street_address()`

Create a street address, a combination of streetname and house
indicator.

#### Usage

    AddressProvider$street_address()

------------------------------------------------------------------------

### Method `postcode()`

Create a postal code

#### Usage

    AddressProvider$postcode()

------------------------------------------------------------------------

### Method `init_person_provider()`

initialize the person provider (for use in addresses based on names)

#### Usage

    AddressProvider$init_person_provider(locale)

#### Arguments

- `locale`:

  locale

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    AddressProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
