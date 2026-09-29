# ColorProvider

methods for colors create color names, hex values, rgb values or css
values.

## Value

A ColorProvider object that can generate colors.

## See also

Other ParentProviders:
[`AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
[`InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md),
[`JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md),
[`LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md),
[`PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md),
[`PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md),
[`TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md),
[`UserAgentProvider`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `ColorProvider`

## Active bindings

- `all_colors`:

  (character) xxx

- `safe_colors`:

  (character) xxx

## Methods

### Public methods

- [`ColorProvider$color_name()`](#method-ColorProvider-color_name)

- [`ColorProvider$hex_from_name()`](#method-ColorProvider-hex_from_name)

- [`ColorProvider$safe_color_name()`](#method-ColorProvider-safe_color_name)

- [`ColorProvider$hex_color()`](#method-ColorProvider-hex_color)

- [`ColorProvider$safe_hex_color()`](#method-ColorProvider-safe_hex_color)

- [`ColorProvider$rgb_color()`](#method-ColorProvider-rgb_color)

- [`ColorProvider$rgb_css_color()`](#method-ColorProvider-rgb_css_color)

- [`ColorProvider$clone()`](#method-ColorProvider-clone)

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

------------------------------------------------------------------------

### Method `color_name()`

color name

#### Usage

    ColorProvider$color_name()

------------------------------------------------------------------------

### Method `hex_from_name()`

get color by name

#### Usage

    ColorProvider$hex_from_name(name)

#### Arguments

- `name`:

  color name

#### Returns

hex value

------------------------------------------------------------------------

### Method `safe_color_name()`

safe color name

#### Usage

    ColorProvider$safe_color_name()

------------------------------------------------------------------------

### Method `hex_color()`

hex color

#### Usage

    ColorProvider$hex_color()

------------------------------------------------------------------------

### Method `safe_hex_color()`

safe hex color

#### Usage

    ColorProvider$safe_hex_color()

------------------------------------------------------------------------

### Method `rgb_color()`

RGB color

#### Usage

    ColorProvider$rgb_color()

------------------------------------------------------------------------

### Method `rgb_css_color()`

RGB CSS color

#### Usage

    ColorProvider$rgb_css_color()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    ColorProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
