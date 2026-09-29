# TaxonomyProvider en_US

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

Other en:
[`AddressProvider_en_GB`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_GB.md),
[`AddressProvider_en_NZ`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_NZ.md),
[`AddressProvider_en_US`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_US.md),
[`ColorProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ColorProvider_en_US.md),
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
[`UserAgentProvider_en_US`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider_en_US.md),
[`english-language`](https://docs.ropensci.org/charlatan/reference/english-language.md)

Other US:
[`AddressProvider_en_US`](https://docs.ropensci.org/charlatan/reference/AddressProvider_en_US.md),
[`ColorProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ColorProvider_en_US.md),
[`CompanyProvider_en_US`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md),
[`ElementProvider_en_US`](https://docs.ropensci.org/charlatan/reference/ElementProvider_en_US.md),
[`FileProvider_en_US`](https://docs.ropensci.org/charlatan/reference/FileProvider_en_US.md),
[`InternetProvider_en_US`](https://docs.ropensci.org/charlatan/reference/InternetProvider_en_US.md),
[`JobProvider_en_US`](https://docs.ropensci.org/charlatan/reference/JobProvider_en_US.md),
[`LoremProvider_en_US`](https://docs.ropensci.org/charlatan/reference/LoremProvider_en_US.md),
[`PersonProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_US.md),
[`PhoneNumberProvider_en_US`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_en_US.md),
[`SSNProvider_en_US`](https://docs.ropensci.org/charlatan/reference/SSNProvider_en_US.md),
[`UserAgentProvider_en_US`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider_en_US.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md)
-\> `TaxonomyProvider_en_US`

## Methods

### Public methods

- [`TaxonomyProvider_en_US$clone()`](#method-TaxonomyProvider_en_US-clone)

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
- [`charlatan::TaxonomyProvider$epithet()`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.html#method-epithet)
- [`charlatan::TaxonomyProvider$genus()`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.html#method-genus)
- [`charlatan::TaxonomyProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.html#method-initialize)
- [`charlatan::TaxonomyProvider$species()`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.html#method-species)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    TaxonomyProvider_en_US$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
(z <- TaxonomyProvider_en_US$new())
#> < TaxonomyProvider >
#> locale: en_US
z$genus()
#> [1] "Elettariopsis"
z$epithet()
#> [1] "gerardii"
z$species()
#> [1] "Spiesia flaccidum"
z$species(authority = TRUE)
#> [1] "Bethencourtia areitiana Kunde"
## FIXME - datetimeprovider slow - may be related to unix time problem
# z$species(authority = TRUE, date = TRUE)
```
