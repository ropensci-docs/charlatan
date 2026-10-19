# ColorProvider

methods for colors create color names, hex values, rgb values or css
values.

## Value

A ColorProvider object that can generate colors.

## See also

Other en:
[`AddressProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_GB.md),
[`AddressProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_NZ.md),
[`AddressProvider_en_US`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_US.md),
[`CompanyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md),
[`ElementProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ElementProvider_en_US.md),
[`FileProvider_en_US`](https://docs.ropensci.org/charlatan/reference/FileProvider_en_US.md),
[`InternetProvider_en_AU`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_AU.md),
[`InternetProvider_en_US`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_US.md),
[`JobProvider_en_US`](https://docs.ropensci.org/charlatan/reference/JobProvider_en_US.md),
[`LoremProvider_en_US`](https://docs.ropensci.org/charlatan/reference/LoremProvider_en_US.md),
[`PersonProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_GB.md),
[`PersonProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_NZ.md),
[`PersonProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_US.md),
[`PhoneNumberProvider_en_AU`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_AU.md),
[`PhoneNumberProvider_en_CA`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_CA.md),
[`PhoneNumberProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_GB.md),
[`PhoneNumberProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_NZ.md),
[`PhoneNumberProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_US.md),
[`PhoneNumberProvider_es_MX`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_es_MX.md),
[`SSNProvider_en_US`](https://docs.ropensci.org/charlatan/reference/SSNProvider_en_US.md),
[`TaxonomyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider_en_US.md),
[`UserAgentProvider_en_US`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider_en_US.md),
[`english-language`](https://docs.ropensci.org/charlatan/reference/english-language.md)

Other US:
[`AddressProvider_en_US`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_US.md),
[`CompanyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md),
[`ElementProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ElementProvider_en_US.md),
[`FileProvider_en_US`](https://docs.ropensci.org/charlatan/reference/FileProvider_en_US.md),
[`InternetProvider_en_US`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_US.md),
[`JobProvider_en_US`](https://docs.ropensci.org/charlatan/reference/JobProvider_en_US.md),
[`LoremProvider_en_US`](https://docs.ropensci.org/charlatan/reference/LoremProvider_en_US.md),
[`PersonProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_US.md),
[`PhoneNumberProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_US.md),
[`SSNProvider_en_US`](https://docs.ropensci.org/charlatan/reference/SSNProvider_en_US.md),
[`TaxonomyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider_en_US.md),
[`UserAgentProvider_en_US`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider_en_US.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md)
-\> `ColorProvider_en_US`

## Methods

### Public methods

- [`ColorProvider_en_US$clone()`](#method-ColorProvider_en_US-clone)

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

    ColorProvider_en_US$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- ColorProvider_en_US$new()
x$locale
#> [1] "en_US"
x$color_name()
#> [1] "MidnightBlue"
x$safe_color_name()
#> [1] "lime"
x$hex_color()
#> [1] "#E1D344"
x$safe_hex_color()
#> [1] "#ff9999"
x$rgb_color()
#> [1]  22 236  51
x$rgb_css_color()
#> [1] "rgb(147, 3, 82)"
```
