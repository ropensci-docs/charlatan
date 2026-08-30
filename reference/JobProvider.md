# JobProvider

generate jobs

## Value

A JobProvider object with methods for jobs

## See also

Other ParentProviders:
[`AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md),
[`ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
[`InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md),
[`LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md),
[`PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md),
[`PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md),
[`TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md),
[`UserAgentProvider`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `JobProvider`

## Methods

### Public methods

- [`JobProvider$render()`](#method-JobProvider-render)

- [`JobProvider$clone()`](#method-JobProvider-clone)

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

### Method `render()`

Make a job

#### Usage

    JobProvider$render()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    JobProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
