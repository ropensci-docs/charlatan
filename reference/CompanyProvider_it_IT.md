# CompanyProvider Italian (Italy)

company name/etc. methods

Note that you cannot instantiate this class, you can only use the
localized versions such as
[CompanyProvider_en_US](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md).

## Value

A CompanyProvider object that can create companies.

## See also

Other it:
[`PersonProvider_it_IT`](https://docs.ropensci.org/charlatan/reference/PersonProvider_it_IT.md),
[`PhoneNumberProvider_it_IT`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_it_IT.md),
[`italian-language`](https://docs.ropensci.org/charlatan/reference/italian-language.md)

Other IT:
[`PersonProvider_it_IT`](https://docs.ropensci.org/charlatan/reference/PersonProvider_it_IT.md),
[`PhoneNumberProvider_it_IT`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_it_IT.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
-\> `CompanyProvider_it_IT`

## Methods

### Public methods

- [`CompanyProvider_it_IT$company()`](#method-CompanyProvider_it_IT-company)

- [`CompanyProvider_it_IT$clone()`](#method-CompanyProvider_it_IT-clone)

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
- [`charlatan::CompanyProvider$bs()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-bs)
- [`charlatan::CompanyProvider$catch_phrase()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-catch_phrase)
- [`charlatan::CompanyProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-initialize)

------------------------------------------------------------------------

### Method `company()`

a company name

#### Usage

    CompanyProvider_it_IT$company()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CompanyProvider_it_IT$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- CompanyProvider_it_IT$new()
x$locale
#> [1] "it_IT"
x$company()
#> [1] "Villa-Benedetti s.r.l."
x$catch_phrase()
#> [1] "Iniziativa distribuita globale"
x$bs()
#> [1] "sistemi estensioni efficienti"
```
