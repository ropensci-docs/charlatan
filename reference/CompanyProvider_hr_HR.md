# CompanyProvider Croatian (Croatia)

company name/etc. methods

Note that you cannot instantiate this class, you can only use the
localized versions such as
[CompanyProvider_en_US](https://docs.ropensci.org/charlatan/reference/CompanyProvider_en_US.md).

## Value

A CompanyProvider object that can create companies.

## See also

Other hr:
[`InternetProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/InternetProvider_hr_HR.md),
[`JobProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/JobProvider_hr_HR.md),
[`PersonProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_hr_HR.md),
[`PhoneNumberProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_hr_HR.md),
[`croatian-language`](https://docs.ropensci.org/charlatan/reference/croatian-language.md)

Other HR:
[`InternetProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/InternetProvider_hr_HR.md),
[`JobProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/JobProvider_hr_HR.md),
[`PersonProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_hr_HR.md),
[`PhoneNumberProvider_hr_HR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_hr_HR.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
-\> `CompanyProvider_hr_HR`

## Methods

### Public methods

- [`CompanyProvider_hr_HR$clone()`](#method-CompanyProvider_hr_HR-clone)

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
- [`charlatan::CompanyProvider$company()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-company)
- [`charlatan::CompanyProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.html#method-initialize)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CompanyProvider_hr_HR$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- CompanyProvider_hr_HR$new()
x$locale
#> [1] "hr_HR"
x$company()
#> [1] "Peroš Bolčević j.d.o.o."
x$catch_phrase()
#> [1] ""
x$bs()
#> [1] ""
```
