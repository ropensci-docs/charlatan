# Person Provider for Spanish (Mexico)

Person Provider for Spanish (Mexico)

Person Provider for Spanish (Mexico)

## Value

A PersonProvider object that can create names.

## Details

Note for female and male components that we fall back on generic
versions if the locale doesn't provide a male/female version. e.g., if
no female first name we use first name

## See also

Other es:
[`CompanyProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_es_MX.md),
[`PersonProvider_es_ES`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_ES.md),
[`PhoneNumberProvider_es_ES`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_ES.md),
[`PhoneNumberProvider_es_PE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_PE.md),
[`spanish-language`](https://docs.ropensci.org/charlatan/reference/spanish-language.md)

Other MX:
[`CompanyProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_es_MX.md),
[`PhoneNumberProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_MX.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md)
-\> `PersonProvider_es_MX`

## Methods

### Public methods

- [`PersonProvider_es_MX$clone()`](#method-PersonProvider_es_MX-clone)

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
- [`charlatan::PersonProvider$change_messy()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-change_messy)
- [`charlatan::PersonProvider$first_name()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-first_name)
- [`charlatan::PersonProvider$first_name_female()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-first_name_female)
- [`charlatan::PersonProvider$first_name_male()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-first_name_male)
- [`charlatan::PersonProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-initialize)
- [`charlatan::PersonProvider$last_name()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-last_name)
- [`charlatan::PersonProvider$last_name_female()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-last_name_female)
- [`charlatan::PersonProvider$last_name_male()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-last_name_male)
- [`charlatan::PersonProvider$messy_is_possible()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-messy_is_possible)
- [`charlatan::PersonProvider$messy_switch()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-messy_switch)
- [`charlatan::PersonProvider$prefix()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-prefix)
- [`charlatan::PersonProvider$prefix_female()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-prefix_female)
- [`charlatan::PersonProvider$prefix_male()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-prefix_male)
- [`charlatan::PersonProvider$render()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-render)
- [`charlatan::PersonProvider$suffix()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-suffix)
- [`charlatan::PersonProvider$suffix_female()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-suffix_female)
- [`charlatan::PersonProvider$suffix_male()`](https://docs.ropensci.org/charlatan/reference/PersonProvider.html#method-suffix_male)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    PersonProvider_es_MX$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- PersonProvider_de_AT$new()
x$locale
#> [1] "de_AT"
x$render()
#> [1] "Ing. Anton Gruber"
x$first_name()
#> [1] "Paul"
x$first_name_female()
#> [1] "Alexander"
x$first_name_male()
#> [1] "Matthias"
x$last_name()
#> [1] "Brunner"
x$last_name_female()
#> [1] "Müllner"
x$last_name_male()
#> [1] "Baumgartner"
```
