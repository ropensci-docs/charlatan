# Person Provider for Dutch (Netherlands)

Person Provider for Dutch (Netherlands)

Person Provider for Dutch (Netherlands)

## Value

A PersonProvider object that can create names.

## Details

Note for female and male components that we fall back on generic
versions if the locale doesn't provide a male/female version. e.g., if
no female first name we use first name

## See also

Other nl:
[`AddressProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/AddressProvider_nl_NL.md),
[`ElementProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/ElementProvider_nl_NL.md),
[`JobProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/JobProvider_nl_NL.md),
[`PhoneNumberProvider_nl_BE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_nl_BE.md),
[`PhoneNumberProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_nl_NL.md),
[`SSNProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/SSNProvider_nl_NL.md),
[`dutch-language`](https://docs.ropensci.org/charlatan/reference/dutch-language.md)

Other NL:
[`AddressProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/AddressProvider_nl_NL.md),
[`ElementProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/ElementProvider_nl_NL.md),
[`JobProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/JobProvider_nl_NL.md),
[`PhoneNumberProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_nl_NL.md),
[`SSNProvider_nl_NL`](https://docs.ropensci.org/charlatan/reference/SSNProvider_nl_NL.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md)
-\> `PersonProvider_nl_NL`

## Methods

### Public methods

- [`PersonProvider_nl_NL$clone()`](#method-PersonProvider_nl_NL-clone)

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

    PersonProvider_nl_NL$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- PersonProvider_nl_NL$new()
x$locale
#> [1] "nl_NL"
x$render()
#> [1] "Jamie de Graaf"
x$first_name()
#> [1] "Thom"
x$first_name_female()
#> [1] "Mette"
x$first_name_male()
#> [1] "Muhammed"
x$last_name()
#> [1] "van Maaren"
x$last_name_female()
#> [1] "Ellis"
x$last_name_male()
#> [1] "Huel"
```
