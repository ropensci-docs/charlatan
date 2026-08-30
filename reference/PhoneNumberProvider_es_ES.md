# PhoneNumberProvider for Spain

methods for generating phone numbers

## Value

A PhoneNumberProvider object that can create phonenumbers.

## See also

Other es:
[`CompanyProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_es_MX.md),
[`PersonProvider_es_ES`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_ES.md),
[`PersonProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_MX.md),
[`PhoneNumberProvider_es_PE`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_PE.md),
[`spanish-language`](https://docs.ropensci.org/charlatan/reference/spanish-language.md)

Other ES:
[`PersonProvider_es_ES`](https://docs.ropensci.org/charlatan/reference/PersonProvider_es_ES.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md)
-\> `PhoneNumberProvider_es_ES`

## Methods

### Public methods

- [`PhoneNumberProvider_es_ES$clone()`](#method-PhoneNumberProvider_es_ES-clone)

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
- [`charlatan::PhoneNumberProvider$render()`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.html#method-render)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    PhoneNumberProvider_es_ES$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- PhoneNumberProvider_es_ES$new()
z$render()
#> [1] "+34 492 840 464"
```
