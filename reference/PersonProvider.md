# PersonProvider

PersonProvider

PersonProvider

## Value

A PersonProvider object that can create names.

## Details

Methods for Persons, methods for generating names.

## Note

You cannot instantiate the Parent providers. You must use one of the
localized one.

## See also

Other ParentProviders:
[`AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md),
[`ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
[`InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md),
[`JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md),
[`LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md),
[`PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md),
[`TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md),
[`UserAgentProvider`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `PersonProvider`

## Active bindings

- `messy`:

  show current setting for messy. Either TRUE or FALSE depending on
  configuration and if this is even possible for the locale.

## Methods

### Public methods

- [`PersonProvider$new()`](#method-PersonProvider-new)

- [`PersonProvider$messy_is_possible()`](#method-PersonProvider-messy_is_possible)

- [`PersonProvider$change_messy()`](#method-PersonProvider-change_messy)

- [`PersonProvider$render()`](#method-PersonProvider-render)

- [`PersonProvider$messy_switch()`](#method-PersonProvider-messy_switch)

- [`PersonProvider$first_name()`](#method-PersonProvider-first_name)

- [`PersonProvider$first_name_female()`](#method-PersonProvider-first_name_female)

- [`PersonProvider$first_name_male()`](#method-PersonProvider-first_name_male)

- [`PersonProvider$last_name()`](#method-PersonProvider-last_name)

- [`PersonProvider$last_name_female()`](#method-PersonProvider-last_name_female)

- [`PersonProvider$last_name_male()`](#method-PersonProvider-last_name_male)

- [`PersonProvider$prefix()`](#method-PersonProvider-prefix)

- [`PersonProvider$prefix_female()`](#method-PersonProvider-prefix_female)

- [`PersonProvider$prefix_male()`](#method-PersonProvider-prefix_male)

- [`PersonProvider$suffix()`](#method-PersonProvider-suffix)

- [`PersonProvider$suffix_female()`](#method-PersonProvider-suffix_female)

- [`PersonProvider$suffix_male()`](#method-PersonProvider-suffix_male)

- [`PersonProvider$clone()`](#method-PersonProvider-clone)

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

------------------------------------------------------------------------

### Method `new()`

Create a new `PersonProvider` object

#### Usage

    PersonProvider$new(messy = FALSE)

#### Arguments

- `messy`:

  make it messy

------------------------------------------------------------------------

### Method `messy_is_possible()`

internal function to figure out if messy is a valid option for this
locale.

#### Usage

    PersonProvider$messy_is_possible()

------------------------------------------------------------------------

### Method `change_messy()`

Change messy (if possible)

#### Usage

    PersonProvider$change_messy(messy)

#### Arguments

- `messy`:

  TRUE or FALSE

------------------------------------------------------------------------

### Method `render()`

Make a person's name

#### Usage

    PersonProvider$render(fmt = NULL)

#### Arguments

- `fmt`:

  (character) a name format, default: `NULL`

------------------------------------------------------------------------

### Method `messy_switch()`

messy switch (internal). Always return a text, when messy is allowed
return a messy version, but otherwise return a clean version.

#### Usage

    PersonProvider$messy_switch(clean_choice, messy_choice)

#### Arguments

- `clean_choice`:

  the clean version

- `messy_choice`:

  the messy version

------------------------------------------------------------------------

### Method `first_name()`

make a first name

#### Usage

    PersonProvider$first_name()

------------------------------------------------------------------------

### Method `first_name_female()`

make a female first name

#### Usage

    PersonProvider$first_name_female()

------------------------------------------------------------------------

### Method `first_name_male()`

make a male first name

#### Usage

    PersonProvider$first_name_male()

------------------------------------------------------------------------

### Method `last_name()`

make a last name

#### Usage

    PersonProvider$last_name()

------------------------------------------------------------------------

### Method `last_name_female()`

make a female last name

#### Usage

    PersonProvider$last_name_female()

------------------------------------------------------------------------

### Method `last_name_male()`

make a male last name

#### Usage

    PersonProvider$last_name_male()

------------------------------------------------------------------------

### Method `prefix()`

make a name prefix

#### Usage

    PersonProvider$prefix()

------------------------------------------------------------------------

### Method `prefix_female()`

make a female name prefix

#### Usage

    PersonProvider$prefix_female()

------------------------------------------------------------------------

### Method `prefix_male()`

make a male name prefix

#### Usage

    PersonProvider$prefix_male()

------------------------------------------------------------------------

### Method `suffix()`

make a name suffix

#### Usage

    PersonProvider$suffix()

------------------------------------------------------------------------

### Method `suffix_female()`

make a female name suffix

#### Usage

    PersonProvider$suffix_female()

------------------------------------------------------------------------

### Method `suffix_male()`

make a male name suffix

#### Usage

    PersonProvider$suffix_male()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    PersonProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
