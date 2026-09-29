# UserAgentProvider

user agent methods For instance mac_processor, user_agents, chrome and
firefox user agents.

## Value

UserAgentProvider object.

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
[`TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `UserAgentProvider`

## Methods

### Public methods

- [`UserAgentProvider$mac_processor()`](#method-UserAgentProvider-mac_processor)

- [`UserAgentProvider$linux_processor()`](#method-UserAgentProvider-linux_processor)

- [`UserAgentProvider$user_agent()`](#method-UserAgentProvider-user_agent)

- [`UserAgentProvider$chrome()`](#method-UserAgentProvider-chrome)

- [`UserAgentProvider$firefox()`](#method-UserAgentProvider-firefox)

- [`UserAgentProvider$safari()`](#method-UserAgentProvider-safari)

- [`UserAgentProvider$opera()`](#method-UserAgentProvider-opera)

- [`UserAgentProvider$internet_explorer()`](#method-UserAgentProvider-internet_explorer)

- [`UserAgentProvider$windows_platform_token()`](#method-UserAgentProvider-windows_platform_token)

- [`UserAgentProvider$linux_platform_token()`](#method-UserAgentProvider-linux_platform_token)

- [`UserAgentProvider$mac_platform_token()`](#method-UserAgentProvider-mac_platform_token)

- [`UserAgentProvider$clone()`](#method-UserAgentProvider-clone)

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

### Method `mac_processor()`

a mac processor

#### Usage

    UserAgentProvider$mac_processor()

------------------------------------------------------------------------

### Method `linux_processor()`

a linux processor

#### Usage

    UserAgentProvider$linux_processor()

------------------------------------------------------------------------

### Method `user_agent()`

a random user agent string

#### Usage

    UserAgentProvider$user_agent()

------------------------------------------------------------------------

### Method `chrome()`

a chrome user agent string

#### Usage

    UserAgentProvider$chrome(
      version_from = 13,
      version_to = 63,
      build_from = 800,
      build_to = 899
    )

#### Arguments

- `version_from`:

  (integer) minimum version

- `version_to`:

  (integer) maximum version

- `build_from`:

  (integer) minimum build

- `build_to`:

  (integer) maximum build

------------------------------------------------------------------------

### Method `firefox()`

a firefox user agent string

#### Usage

    UserAgentProvider$firefox()

------------------------------------------------------------------------

### Method `safari()`

a safari user agent string

#### Usage

    UserAgentProvider$safari()

------------------------------------------------------------------------

### Method `opera()`

an opera user agent string

#### Usage

    UserAgentProvider$opera()

------------------------------------------------------------------------

### Method `internet_explorer()`

an internet explorer user agent string

#### Usage

    UserAgentProvider$internet_explorer()

------------------------------------------------------------------------

### Method `windows_platform_token()`

a windows platform token

#### Usage

    UserAgentProvider$windows_platform_token()

------------------------------------------------------------------------

### Method `linux_platform_token()`

a linux platform token

#### Usage

    UserAgentProvider$linux_platform_token()

------------------------------------------------------------------------

### Method `mac_platform_token()`

a mac platform token

#### Usage

    UserAgentProvider$mac_platform_token()

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    UserAgentProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
