# ElementProvider

chemical elements methods

## Details

Data from Wikipedia at <https://en.wikipedia.org/wiki/Chemical_element>

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `ElementProvider`

## Methods

### Public methods

- [`ElementProvider$elements()`](#method-ElementProvider-elements)

- [`ElementProvider$symbol()`](#method-ElementProvider-symbol)

- [`ElementProvider$element()`](#method-ElementProvider-element)

- [`ElementProvider$symbol_by_number()`](#method-ElementProvider-symbol_by_number)

- [`ElementProvider$element_by_number()`](#method-ElementProvider-element_by_number)

- [`ElementProvider$clone()`](#method-ElementProvider-clone)

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

### Method [`elements()`](https://docs.ropensci.org/charlatan/reference/elements.md)

dataframe of symbols and elements

#### Usage

    ElementProvider$elements()

------------------------------------------------------------------------

### Method `symbol()`

Get a symbol

#### Usage

    ElementProvider$symbol()

------------------------------------------------------------------------

### Method `element()`

Get an element

#### Usage

    ElementProvider$element()

------------------------------------------------------------------------

### Method `symbol_by_number()`

symbol by number

#### Usage

    ElementProvider$symbol_by_number(number)

#### Arguments

- `number`:

  retrieve symbol of element by atomic number.

------------------------------------------------------------------------

### Method `element_by_number()`

element by number

#### Usage

    ElementProvider$element_by_number(number)

#### Arguments

- `number`:

  retrieve element by atomic number.

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    ElementProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
