# TaxonomyProvider

Taxonomy provider for Generating Taxonomic names.

## Names

Names were taken from Theplantlist. 500 genera names and 500 epithets
were chosen at random from the set of 10,000 names in the dataset in the
`taxize` package. Theplantlist is, as it says on the tin, composed of
plant names - so these fake names are derived from plant names if that
matters to you. These may generate names that match those of real taxa,
but may not as well.

## Taxonomic authority

Randomly, the taxonomic authority is in parentheses - which represents
that the given authority was not the original authority.

## See also

Other ParentProviders:
[`AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md),
[`ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
[`InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md),
[`JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md),
[`LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md),
[`PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md),
[`PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md),
[`UserAgentProvider`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `TaxonomyProvider`

## Methods

### Public methods

- [`TaxonomyProvider$genus()`](#method-TaxonomyProvider-genus)

- [`TaxonomyProvider$epithet()`](#method-TaxonomyProvider-epithet)

- [`TaxonomyProvider$species()`](#method-TaxonomyProvider-species)

- [`TaxonomyProvider$new()`](#method-TaxonomyProvider-new)

- [`TaxonomyProvider$clone()`](#method-TaxonomyProvider-clone)

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

### Method `genus()`

Get a genus name

#### Usage

    TaxonomyProvider$genus()

------------------------------------------------------------------------

### Method `epithet()`

Get an epithet name

#### Usage

    TaxonomyProvider$epithet()

------------------------------------------------------------------------

### Method `species()`

Get a binomial name (genus + epithet)

#### Usage

    TaxonomyProvider$species(authority = FALSE, date = FALSE)

#### Arguments

- `authority`:

  Include authority. default: `FALSE`

- `date`:

  Include authority date. If `authority = FALSE`, this is ignored.
  default: `FALSE`

------------------------------------------------------------------------

### Method `new()`

Initialize new Taxonomy Provider.

#### Usage

    TaxonomyProvider$new()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    TaxonomyProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
