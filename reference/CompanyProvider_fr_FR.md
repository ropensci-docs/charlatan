# CompanyProvider for France (French)

company name/etc. methods

Note that you cannot instantiate this class, you can only use the
localized versions such as
[CompanyProvider_en_US](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md).

## Value

A CompanyProvider object that can create companies.

## See also

Other FR:
[`InternetProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/InternetProvider_fr_FR.md),
[`JobProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_FR.md),
[`PersonProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_FR.md),
[`PhoneNumberProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_FR.md)

Other fr:
[`InternetProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/InternetProvider_fr_FR.md),
[`JobProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_CH.md),
[`JobProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_FR.md),
[`PersonProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_CH.md),
[`PersonProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_FR.md),
[`PhoneNumberProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_CH.md),
[`PhoneNumberProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_FR.md),
[`french-language`](https://docs.ropensci.org/charlatan/reference/french-language.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
-\> `CompanyProvider_fr_FR`

## Methods

### Public methods

- [`CompanyProvider_fr_FR$catch_phrase()`](#method-CompanyProvider_fr_FR-catch_phrase)

- [`CompanyProvider_fr_FR$clone()`](#method-CompanyProvider_fr_FR-clone)

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
- [`charlatan::CompanyProvider$company()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-company)
- [`charlatan::CompanyProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-initialize)

------------------------------------------------------------------------

### Method `catch_phrase()`

generate a catch phrase for a company.

#### Usage

    CompanyProvider_fr_FR$catch_phrase()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CompanyProvider_fr_FR$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- CompanyProvider_fr_FR$new()
x$locale
#> [1] "fr_FR"
x$company()
#> [1] "Boucher Boucher et Fils"
x$catch_phrase()
#> [1] "le droit de louer plus facilement"
```
