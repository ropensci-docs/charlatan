# BaseProvider

BaseProvider

BaseProvider

## Note

You cannot instantiate the Parent providers. You must use one of the
localized one.

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `BaseProvider`

## Active bindings

- `locale`:

  (character) locale of this Provider.

## Methods

### Public methods

- [`BaseProvider$check_locale()`](#method-BaseProvider-check_locale)

- [`BaseProvider$allowed_locales()`](#method-BaseProvider-allowed_locales)

- [`BaseProvider$new()`](#method-BaseProvider-new)

- [`BaseProvider$print()`](#method-BaseProvider-print)

- [`BaseProvider$clone()`](#method-BaseProvider-clone)

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

------------------------------------------------------------------------

### Method `check_locale()`

check a locale to see if it exists, if not, stop with error message

#### Usage

    BaseProvider$check_locale(x)

#### Arguments

- `x`:

  a locale name, e.g, 'bg_BG'

#### Returns

returns nothing if locale is supported; stops w/ message if not

------------------------------------------------------------------------

### Method `allowed_locales()`

fetch the allowed locales for this provider

#### Usage

    BaseProvider$allowed_locales()

------------------------------------------------------------------------

### Method `new()`

Create a new Provider object

#### Usage

    BaseProvider$new()

#### Returns

A new object

------------------------------------------------------------------------

### Method [`print()`](https://rdrr.io/r/base/print.html)

Print method for provider

#### Usage

    BaseProvider$print(...)

#### Arguments

- `...`:

  ignored by this method

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    BaseProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
(x <- BaseProvider$new())
#> < BaseProvider >
#> locale: 

x$numerify("#%%asdf221?")
#> [1] "775asdf221?"
x$lexify("#%%asdf221?")
#> [1] "#%%asdf221h"
x$bothify("#%%asdf221?")
#> [1] "173asdf221E"
```
