# CompanyProvider for German (Germany)

company name/etc. methods

Note that you cannot instantiate this class, you can only use the
localized versions such as
[CompanyProvider_en_US](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md).

## Value

A CompanyProvider object that can create companies.

## See also

Other de:
[`InternetProvider_de_DE`](https://docs.ropensci.org/charlatan/reference/InternetProvider_de_DE.md),
[`PersonProvider_de_AT`](https://docs.ropensci.org/charlatan/reference/PersonProvider_de_AT.md),
[`PersonProvider_de_DE`](https://docs.ropensci.org/charlatan/reference/PersonProvider_de_DE.md),
[`PhoneNumberProvider_de_DE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_de_DE.md),
[`german-language`](https://docs.ropensci.org/charlatan/reference/german-language.md)

Other DE:
[`InternetProvider_de_DE`](https://docs.ropensci.org/charlatan/reference/InternetProvider_de_DE.md),
[`PersonProvider_de_DE`](https://docs.ropensci.org/charlatan/reference/PersonProvider_de_DE.md),
[`PhoneNumberProvider_de_DE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_de_DE.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
-\> `CompanyProvider_de_DE`

## Methods

### Public methods

- [`CompanyProvider_de_DE$clone()`](#method-CompanyProvider_de_DE-clone)

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

    CompanyProvider_de_DE$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- CompanyProvider_de_DE$new()
x$locale
#> [1] "de_DE"
x$company()
#> [1] "Süßebier"
```
