# Job provider for Taiwan

generate jobs

## Value

A JobProvider object with methods for jobs

## See also

Other zh:
[`LoremProvider_zh_CN`](https://docs.ropensci.org/charlatan/reference/LoremProvider_zh_CN.md),
[`LoremProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/LoremProvider_zh_TW.md),
[`PhoneNumberProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_zh_TW.md),
[`chinese-language`](https://docs.ropensci.org/charlatan/reference/chinese-language.md)

Other TW:
[`LoremProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/LoremProvider_zh_TW.md),
[`PhoneNumberProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_zh_TW.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md)
-\> `JobProvider_zh_TW`

## Methods

### Public methods

- [`JobProvider_zh_TW$clone()`](#method-JobProvider_zh_TW-clone)

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

    JobProvider_zh_TW$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- JobProvider_zh_TW$new()
x$render()
#> [1] "稽核人員"
```
