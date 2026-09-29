# A NonLocalized Provider that contains all the selection and creation elements, but not the locales. That way we can still inherit an do useful stuff for providers that have no locale.

A NonLocalized Provider that contains all the selection and creation
elements, but not the locales. That way we can still inherit an do
useful stuff for providers that have no locale.

A NonLocalized Provider that contains all the selection and creation
elements, but not the locales. That way we can still inherit an do
useful stuff for providers that have no locale.

## Active bindings

- `provider`:

  Display the provider name.

## Methods

### Public methods

- [`BareProvider$random_element()`](#method-BareProvider-random_element)

- [`BareProvider$random_element_prob()`](#method-BareProvider-random_element_prob)

- [`BareProvider$random_int()`](#method-BareProvider-random_int)

- [`BareProvider$random_digit()`](#method-BareProvider-random_digit)

- [`BareProvider$random_digit_not_zero()`](#method-BareProvider-random_digit_not_zero)

- [`BareProvider$random_digit_or_empty()`](#method-BareProvider-random_digit_or_empty)

- [`BareProvider$random_digit_not_zero_or_empty()`](#method-BareProvider-random_digit_not_zero_or_empty)

- [`BareProvider$random_letter()`](#method-BareProvider-random_letter)

- [`BareProvider$numerify()`](#method-BareProvider-numerify)

- [`BareProvider$lexify()`](#method-BareProvider-lexify)

- [`BareProvider$bothify()`](#method-BareProvider-bothify)

- [`BareProvider$randomize_nb_elements()`](#method-BareProvider-randomize_nb_elements)

- [`BareProvider$print()`](#method-BareProvider-print)

- [`BareProvider$clone()`](#method-BareProvider-clone)

------------------------------------------------------------------------

### Method `random_element()`

pick a random element from vector/list

#### Usage

    BareProvider$random_element(x)

#### Arguments

- `x`:

  vector or list

#### Returns

a single element from x

------------------------------------------------------------------------

### Method `random_element_prob()`

pick a random element with probability from vector/list

#### Usage

    BareProvider$random_element_prob(x)

#### Arguments

- `x`:

  vector or list

------------------------------------------------------------------------

### Method `random_int()`

any number of random integers from a min, max

#### Usage

    BareProvider$random_int(min = 0, max = 9999, size = 1)

#### Arguments

- `min`:

  the minimum value. default: 0

- `max`:

  the maximum value. default: 9999

- `size`:

  number of values to return. default: 1

#### Returns

random integer

------------------------------------------------------------------------

### Method `random_digit()`

random integer between 0 and 9

#### Usage

    BareProvider$random_digit()

------------------------------------------------------------------------

### Method `random_digit_not_zero()`

random integer between 1 and 9

#### Usage

    BareProvider$random_digit_not_zero()

------------------------------------------------------------------------

### Method `random_digit_or_empty()`

random integer between 0 and 9 or empty character string

#### Usage

    BareProvider$random_digit_or_empty()

------------------------------------------------------------------------

### Method `random_digit_not_zero_or_empty()`

random integer between 1 and 9 or empty character string

#### Usage

    BareProvider$random_digit_not_zero_or_empty()

------------------------------------------------------------------------

### Method `random_letter()`

random letter

#### Usage

    BareProvider$random_letter()

------------------------------------------------------------------------

### Method `numerify()`

replace a template with numbers

#### Usage

    BareProvider$numerify(text = "###")

#### Arguments

- `text`:

  (character) a string

------------------------------------------------------------------------

### Method `lexify()`

replace a template with letters

#### Usage

    BareProvider$lexify(text = "????")

#### Arguments

- `text`:

  (character) a string

------------------------------------------------------------------------

### Method `bothify()`

both numerify and lexify together

#### Usage

    BareProvider$bothify(text = "## ??")

#### Arguments

- `text`:

  (character) a string

------------------------------------------------------------------------

### Method `randomize_nb_elements()`

Returns a random value near number

#### Usage

    BareProvider$randomize_nb_elements(
      number = 10,
      le = FALSE,
      ge = FALSE,
      min = NULL,
      max = NULL
    )

#### Arguments

- `number`:

  value to which the result must be near

- `le`:

  result must be lower or equal to number

- `ge`:

  result must be greater or equal to number

- `min`:

  the minimum value. default: `NULL`

- `max`:

  the maximum value. default: `NULL`

#### Returns

a random int near number

------------------------------------------------------------------------

### Method [`print()`](https://rdrr.io/r/base/print.html)

Print method for provider

#### Usage

    BareProvider$print(...)

#### Arguments

- `...`:

  ignored by this method

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    BareProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
