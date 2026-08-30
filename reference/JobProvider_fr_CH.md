# Job provider for Zwitserland

generate jobs

## Value

A JobProvider object with methods for jobs

## See also

Other fr:
[`CompanyProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_fr_FR.md),
[`InternetProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/InternetProvider_fr_FR.md),
[`JobProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_FR.md),
[`PersonProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_CH.md),
[`PersonProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_FR.md),
[`PhoneNumberProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_CH.md),
[`PhoneNumberProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_FR.md),
[`french-language`](https://docs.ropensci.org/charlatan/reference/french-language.md)

Other CH:
[`PersonProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_CH.md),
[`PhoneNumberProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_CH.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md)
-\> `JobProvider_fr_CH`

## Methods

### Public methods

- [`JobProvider_fr_CH$clone()`](#method-JobProvider_fr_CH-clone)

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
- [`charlatan::BaseProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-initialize)
- [`charlatan::BaseProvider$print()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-print)
- [`charlatan::JobProvider$render()`](https://docs.ropensci.org/charlatan/reference/JobProvider.html#method-render)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    JobProvider_fr_CH$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- JobProvider_fr_CH$new()
x$render()
#> [1] "Ecobiologiste de la construction diplômé"
```
