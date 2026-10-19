# InternetProvider

internet methods, e.g., email addresses, domain names

Note that if a locale you set doesn't have a locale specific set of data
for
[PersonProvider](https://docs.ropensci.org/charlatan/reference/PersonProvider.md)
or
[CompanyProvider](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)
we fall back to `en_US` Also note that you

## Value

A InternetProvider object with specific functions for internet.

## See also

Other ParentProviders:
[`AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md),
[`ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
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
-\> `InternetProvider`

## Methods

### Public methods

- [`InternetProvider$new()`](#method-InternetProvider-new)

- [`InternetProvider$to_ascii()`](#method-InternetProvider-to_ascii)

- [`InternetProvider$email()`](#method-InternetProvider-email)

- [`InternetProvider$safe_email()`](#method-InternetProvider-safe_email)

- [`InternetProvider$free_email()`](#method-InternetProvider-free_email)

- [`InternetProvider$company_email()`](#method-InternetProvider-company_email)

- [`InternetProvider$ascii_email()`](#method-InternetProvider-ascii_email)

- [`InternetProvider$ascii_safe_email()`](#method-InternetProvider-ascii_safe_email)

- [`InternetProvider$ascii_free_email()`](#method-InternetProvider-ascii_free_email)

- [`InternetProvider$ascii_company_email()`](#method-InternetProvider-ascii_company_email)

- [`InternetProvider$user_name()`](#method-InternetProvider-user_name)

- [`InternetProvider$tld()`](#method-InternetProvider-tld)

- [`InternetProvider$free_email_domain()`](#method-InternetProvider-free_email_domain)

- [`InternetProvider$url()`](#method-InternetProvider-url)

- [`InternetProvider$domain_name()`](#method-InternetProvider-domain_name)

- [`InternetProvider$domain_word()`](#method-InternetProvider-domain_word)

- [`InternetProvider$ipv4()`](#method-InternetProvider-ipv4)

- [`InternetProvider$ipv6()`](#method-InternetProvider-ipv6)

- [`InternetProvider$mac_address()`](#method-InternetProvider-mac_address)

- [`InternetProvider$uri_page()`](#method-InternetProvider-uri_page)

- [`InternetProvider$uri_path()`](#method-InternetProvider-uri_path)

- [`InternetProvider$uri_extension()`](#method-InternetProvider-uri_extension)

- [`InternetProvider$uri()`](#method-InternetProvider-uri)

- [`InternetProvider$slug()`](#method-InternetProvider-slug)

- [`InternetProvider$image_url()`](#method-InternetProvider-image_url)

- [`InternetProvider$clone()`](#method-InternetProvider-clone)

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

Create a new Provider object

#### Usage

    InternetProvider$new()

#### Returns

A new object

------------------------------------------------------------------------

### Method `to_ascii()`

convert to ascii

#### Usage

    InternetProvider$to_ascii(x)

#### Arguments

- `x`:

  the stringn to convert to ascii

------------------------------------------------------------------------

### Method `email()`

get an email address

#### Usage

    InternetProvider$email(domain = NULL)

#### Arguments

- `domain`:

  (character) a domain name, if not given, a random name is chosen

------------------------------------------------------------------------

### Method `safe_email()`

get a safe email address

#### Usage

    InternetProvider$safe_email()

------------------------------------------------------------------------

### Method `free_email()`

a free email address

#### Usage

    InternetProvider$free_email()

------------------------------------------------------------------------

### Method `company_email()`

company email address

#### Usage

    InternetProvider$company_email()

------------------------------------------------------------------------

### Method `ascii_email()`

ascii email address

#### Usage

    InternetProvider$ascii_email()

------------------------------------------------------------------------

### Method `ascii_safe_email()`

safe ascii email address

#### Usage

    InternetProvider$ascii_safe_email()

------------------------------------------------------------------------

### Method `ascii_free_email()`

an ascii free email address

#### Usage

    InternetProvider$ascii_free_email()

------------------------------------------------------------------------

### Method `ascii_company_email()`

ascii company email address

#### Usage

    InternetProvider$ascii_company_email()

------------------------------------------------------------------------

### Method `user_name()`

a user name

#### Usage

    InternetProvider$user_name()

------------------------------------------------------------------------

### Method `tld()`

a tld

#### Usage

    InternetProvider$tld()

------------------------------------------------------------------------

### Method `free_email_domain()`

free email domain name

#### Usage

    InternetProvider$free_email_domain()

------------------------------------------------------------------------

### Method [`url()`](https://rdrr.io/r/base/connections.html)

a url

#### Usage

    InternetProvider$url(schemes = NULL)

#### Arguments

- `schemes`:

  (character vector) a url scheme, defaults are http and https

------------------------------------------------------------------------

### Method `domain_name()`

Produce an Internet domain name with the specified number of subdomain
levels

#### Usage

    InternetProvider$domain_name(levels = 1)

#### Arguments

- `levels`:

  (integer) how many levels, must be \>1

------------------------------------------------------------------------

### Method `domain_word()`

a domain word

#### Usage

    InternetProvider$domain_word()

------------------------------------------------------------------------

### Method `ipv4()`

an ipv4 address or network

#### Usage

    InternetProvider$ipv4(network = FALSE)

#### Arguments

- `network`:

  (logical) produce a network

------------------------------------------------------------------------

### Method `ipv6()`

an ipv6 address or network

#### Usage

    InternetProvider$ipv6(network = FALSE)

#### Arguments

- `network`:

  (logical) produce a network

------------------------------------------------------------------------

### Method `mac_address()`

a mac address

#### Usage

    InternetProvider$mac_address()

------------------------------------------------------------------------

### Method `uri_page()`

a uri page

#### Usage

    InternetProvider$uri_page()

------------------------------------------------------------------------

### Method `uri_path()`

a uri path

#### Usage

    InternetProvider$uri_path(deep = NULL)

#### Arguments

- `deep`:

  how deep to go, an integer, if not given an integer between 1 and 4
  (inclusive) is chosen

------------------------------------------------------------------------

### Method `uri_extension()`

a uri extension

#### Usage

    InternetProvider$uri_extension()

------------------------------------------------------------------------

### Method `uri()`

a uri

#### Usage

    InternetProvider$uri()

------------------------------------------------------------------------

### Method `slug()`

a slug

#### Usage

    InternetProvider$slug(value = NULL)

#### Arguments

- `value`:

  (character) a string, if given, returns itself, if not, uses
  [LoremProvider](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
  to get a random string. default: `NULL`

------------------------------------------------------------------------

### Method `image_url()`

Returns URL to placeholder image - Example: http://placehold.it/640x480

#### Usage

    InternetProvider$image_url(width = NULL, height = NULL)

#### Arguments

- `width`:

  image width, in pixels

- `height`:

  image height, in pixels

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    InternetProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
