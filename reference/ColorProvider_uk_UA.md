# ColorProvider Ukrainian (Ukraine)

methods for colors create color names, hex values, rgb values or css
values.

## Value

A ColorProvider object that can generate colors.

## See also

Other uk:
[`JobProvider_uk_UA`](https://docs.ropensci.org/charlatan/reference/JobProvider_uk_UA.md),
[`PhoneNumberProvider_uk_UA`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_uk_UA.md),
[`ukrainian-language`](https://docs.ropensci.org/charlatan/reference/ukrainian-language.md)

Other UA:
[`JobProvider_uk_UA`](https://docs.ropensci.org/charlatan/reference/JobProvider_uk_UA.md),
[`PhoneNumberProvider_uk_UA`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_uk_UA.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md)
-\> `ColorProvider_uk_UA`

## Methods

### Public methods

- [`ColorProvider_uk_UA$clone()`](#method-ColorProvider_uk_UA-clone)

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
- [`charlatan::ColorProvider$color_name()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-color_name)
- [`charlatan::ColorProvider$hex_color()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-hex_color)
- [`charlatan::ColorProvider$hex_from_name()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-hex_from_name)
- [`charlatan::ColorProvider$rgb_color()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-rgb_color)
- [`charlatan::ColorProvider$rgb_css_color()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-rgb_css_color)
- [`charlatan::ColorProvider$safe_color_name()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-safe_color_name)
- [`charlatan::ColorProvider$safe_hex_color()`](https://docs.ropensci.org/charlatan/reference/ColorProvider.html#method-safe_hex_color)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    ColorProvider_uk_UA$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- ColorProvider_uk_UA$new()
x$locale
#> [1] "uk_UA"
x$color_name()
#> [1] "Червоно-буро-помаранчевий"
x$safe_color_name()
#> [1] "Білий"
x$hex_color()
#> [1] "#D49514"
x$safe_hex_color()
#> [1] "#6699ff"
x$rgb_color()
#> [1] 141  27  83
x$rgb_css_color()
#> [1] "rgb(152, 253, 148)"
```
