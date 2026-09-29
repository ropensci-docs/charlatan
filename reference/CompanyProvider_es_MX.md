# CompanyProvider Spanish (Mexico)

company name/etc. methods

Note that you cannot instantiate this class, you can only use the
localized versions such as
[CompanyProvider_en_US](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md).

## Value

A CompanyProvider object that can create companies.

## See also

Other es:
[`PersonProvider_es_ES`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_ES.md),
[`PersonProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_MX.md),
[`PhoneNumberProvider_es_ES`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_ES.md),
[`PhoneNumberProvider_es_PE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_PE.md),
[`spanish-language`](https://docs.ropensci.org/charlatan/reference/spanish-language.md)

Other MX:
[`PersonProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_MX.md),
[`PhoneNumberProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_MX.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
-\> `CompanyProvider_es_MX`

## Methods

### Public methods

- [`CompanyProvider_es_MX$company()`](#method-CompanyProvider_es_MX-company)

- [`CompanyProvider_es_MX$clone()`](#method-CompanyProvider_es_MX-clone)

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
- [`charlatan::CompanyProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-initialize)

------------------------------------------------------------------------

### Method `company()`

a company name

#### Usage

    CompanyProvider_es_MX$company()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CompanyProvider_es_MX$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- CompanyProvider_es_MX$new()
x$locale
#> [1] "es_MX"
x$company()
#> [1] "Cabrera y Asociados"
x$catch_phrase()
#> [1] "contingencia tiempo real multiplataforma"
x$bs()
#> [1] "compromete iniciativas escalables"
```
