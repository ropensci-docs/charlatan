# Internet provider for France

methods for internet related data, like email addresses, usernames, and
websites.

## See also

Other fr:
[`CompanyProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_fr_FR.md),
[`JobProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_CH.md),
[`JobProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_FR.md),
[`PersonProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_CH.md),
[`PersonProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_FR.md),
[`PhoneNumberProvider_fr_CH`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_CH.md),
[`PhoneNumberProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_FR.md),
[`french-language`](https://docs.ropensci.org/charlatan/reference/french-language.md)

Other FR:
[`CompanyProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/CompanyProvider_fr_FR.md),
[`JobProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/JobProvider_fr_FR.md),
[`PersonProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PersonProvider_fr_FR.md),
[`PhoneNumberProvider_fr_FR`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_fr_FR.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md)
-\> `InternetProvider_fr_FR`

## Methods

### Public methods

- [`InternetProvider_fr_FR$clone()`](#method-InternetProvider_fr_FR-clone)

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
- [`charlatan::InternetProvider$ascii_company_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-ascii_company_email)
- [`charlatan::InternetProvider$ascii_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-ascii_email)
- [`charlatan::InternetProvider$ascii_free_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-ascii_free_email)
- [`charlatan::InternetProvider$ascii_safe_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-ascii_safe_email)
- [`charlatan::InternetProvider$company_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-company_email)
- [`charlatan::InternetProvider$domain_name()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-domain_name)
- [`charlatan::InternetProvider$domain_word()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-domain_word)
- [`charlatan::InternetProvider$email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-email)
- [`charlatan::InternetProvider$free_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-free_email)
- [`charlatan::InternetProvider$free_email_domain()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-free_email_domain)
- [`charlatan::InternetProvider$image_url()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-image_url)
- [`charlatan::InternetProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-initialize)
- [`charlatan::InternetProvider$ipv4()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-ipv4)
- [`charlatan::InternetProvider$ipv6()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-ipv6)
- [`charlatan::InternetProvider$mac_address()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-mac_address)
- [`charlatan::InternetProvider$safe_email()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-safe_email)
- [`charlatan::InternetProvider$slug()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-slug)
- [`charlatan::InternetProvider$tld()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-tld)
- [`charlatan::InternetProvider$to_ascii()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-to_ascii)
- [`charlatan::InternetProvider$uri()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-uri)
- [`charlatan::InternetProvider$uri_extension()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-uri_extension)
- [`charlatan::InternetProvider$uri_page()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-uri_page)
- [`charlatan::InternetProvider$uri_path()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-uri_path)
- [`charlatan::InternetProvider$url()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-url)
- [`charlatan::InternetProvider$user_name()`](https://docs.ropensci.org/charlatan/reference/InternetProvider.html#method-user_name)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    InternetProvider_fr_FR$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- InternetProvider_fr_FR$new()
#> Warning:  LoremProvider does not have locale fr_FR, defaulting to en_US locale.
x$email()
#> [1] "durand.camille@sarl.fr"
x$free_email()
#> [1] "wgarnier@tiscali.fr"
x$mac_address()
#> [1] "cd:ce:7f:7b:4b:f1:f8"
x$company_email()
#> [1] "odelorme@na.com"
```
