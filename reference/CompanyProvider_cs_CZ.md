# CompanyProvider for Czech

company name/etc. methods

Note that you cannot instantiate this class, you can only use the
localized versions such as
[CompanyProvider_en_US](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md).

## Value

A CompanyProvider object that can create companies.

## See also

Other cs:
[`InternetProvider_cs_CZ`](https://docs.ropensci.org/charlatan/reference/InternetProvider_cs_CZ.md),
[`PersonProvider_cs_CZ`](https://docs.ropensci.org/charlatan/reference/PersonProvider_cs_CZ.md),
[`PhoneNumberProvider_cs_CZ`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_cs_CZ.md),
[`czech-language`](https://docs.ropensci.org/charlatan/reference/czech-language.md)

Other CZ:
[`InternetProvider_cs_CZ`](https://docs.ropensci.org/charlatan/reference/InternetProvider_cs_CZ.md),
[`PersonProvider_cs_CZ`](https://docs.ropensci.org/charlatan/reference/PersonProvider_cs_CZ.md),
[`PhoneNumberProvider_cs_CZ`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_cs_CZ.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
-\> `CompanyProvider_cs_CZ`

## Methods

### Public methods

- [`CompanyProvider_cs_CZ$clone()`](#method-CompanyProvider_cs_CZ-clone)

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
- [`charlatan::CompanyProvider$bs()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-bs)
- [`charlatan::CompanyProvider$catch_phrase()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-catch_phrase)
- [`charlatan::CompanyProvider$company()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-company)
- [`charlatan::CompanyProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-initialize)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CompanyProvider_cs_CZ$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- CompanyProvider_cs_CZ$new()
x$locale
#> [1] "cs_CZ"
x$company()
#> [1] "Dušek Doležal a.s."
```
