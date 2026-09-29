# FraudsterClient

Fraudster R6 client

## Public fields

- `locale`:

  (character) the locale to use

## Methods

### Public methods

- [`FraudsterClient$new()`](#method-FraudsterClient-new)

- [`FraudsterClient$print()`](#method-FraudsterClient-print)

- [`FraudsterClient$job()`](#method-FraudsterClient-job)

- [`FraudsterClient$name()`](#method-FraudsterClient-name)

- [`FraudsterClient$color_name()`](#method-FraudsterClient-color_name)

- [`FraudsterClient$phone_number()`](#method-FraudsterClient-phone_number)

- [`FraudsterClient$safe_color_name()`](#method-FraudsterClient-safe_color_name)

- [`FraudsterClient$address()`](#method-FraudsterClient-address)

- [`FraudsterClient$company()`](#method-FraudsterClient-company)

- [`FraudsterClient$element()`](#method-FraudsterClient-element)

- [`FraudsterClient$file_name()`](#method-FraudsterClient-file_name)

- [`FraudsterClient$email()`](#method-FraudsterClient-email)

- [`FraudsterClient$url()`](#method-FraudsterClient-url)

- [`FraudsterClient$lorem_paragraph()`](#method-FraudsterClient-lorem_paragraph)

- [`FraudsterClient$ssn()`](#method-FraudsterClient-ssn)

- [`FraudsterClient$mac_address()`](#method-FraudsterClient-mac_address)

- [`FraudsterClient$element_symbol()`](#method-FraudsterClient-element_symbol)

- [`FraudsterClient$hex_color()`](#method-FraudsterClient-hex_color)

- [`FraudsterClient$safe_hex_color()`](#method-FraudsterClient-safe_hex_color)

- [`FraudsterClient$rgb_color()`](#method-FraudsterClient-rgb_color)

- [`FraudsterClient$rgb_css_color()`](#method-FraudsterClient-rgb_css_color)

- [`FraudsterClient$lat()`](#method-FraudsterClient-lat)

- [`FraudsterClient$lon()`](#method-FraudsterClient-lon)

- [`FraudsterClient$position()`](#method-FraudsterClient-position)

- [`FraudsterClient$doi()`](#method-FraudsterClient-doi)

- [`FraudsterClient$timezone()`](#method-FraudsterClient-timezone)

- [`FraudsterClient$unix_time()`](#method-FraudsterClient-unix_time)

- [`FraudsterClient$date_time()`](#method-FraudsterClient-date_time)

- [`FraudsterClient$genus()`](#method-FraudsterClient-genus)

- [`FraudsterClient$epithet()`](#method-FraudsterClient-epithet)

- [`FraudsterClient$species()`](#method-FraudsterClient-species)

- [`FraudsterClient$sequence()`](#method-FraudsterClient-sequence)

- [`FraudsterClient$double()`](#method-FraudsterClient-double)

- [`FraudsterClient$integer()`](#method-FraudsterClient-integer)

- [`FraudsterClient$uniform()`](#method-FraudsterClient-uniform)

- [`FraudsterClient$norm()`](#method-FraudsterClient-norm)

- [`FraudsterClient$lnorm()`](#method-FraudsterClient-lnorm)

- [`FraudsterClient$beta()`](#method-FraudsterClient-beta)

- [`FraudsterClient$currency()`](#method-FraudsterClient-currency)

- [`FraudsterClient$credit_card_provider()`](#method-FraudsterClient-credit_card_provider)

- [`FraudsterClient$credit_card_number()`](#method-FraudsterClient-credit_card_number)

- [`FraudsterClient$credit_card_security_code()`](#method-FraudsterClient-credit_card_security_code)

- [`FraudsterClient$clone()`](#method-FraudsterClient-clone)

------------------------------------------------------------------------

### Method `new()`

Create a new `FraudsterClient` object

#### Usage

    FraudsterClient$new(locale = NULL)

#### Arguments

- `locale`:

  (character) the locale to use. options: en_US (default), fr_FR, fr_CH,
  hr_FR, fa_IR, pl_PL, ru_RU, uk_UA, zh_TW.

#### Returns

A new `RequestSignature` object

------------------------------------------------------------------------

### Method [`print()`](https://rdrr.io/r/base/print.html)

print method for the `FraudsterClient` class

#### Usage

    FraudsterClient$print(x, ...)

#### Arguments

- `x`:

  self

- `...`:

  ignored

------------------------------------------------------------------------

### Method `job()`

jobs

#### Usage

    FraudsterClient$job(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `name()`

names

#### Usage

    FraudsterClient$name(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `color_name()`

colors

#### Usage

    FraudsterClient$color_name(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `phone_number()`

phone number

#### Usage

    FraudsterClient$phone_number(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `safe_color_name()`

safe color name

#### Usage

    FraudsterClient$safe_color_name(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `address()`

Create address

#### Usage

    FraudsterClient$address(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `company()`

Create company

#### Usage

    FraudsterClient$company(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `element()`

Create an element (name).

#### Usage

    FraudsterClient$element(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `file_name()`

Create a File name.

#### Usage

    FraudsterClient$file_name(n = 1, category = NULL)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `category`:

  (character) a category of file extension type, one of audio, image,
  office, text or video. default: `NULL`.

------------------------------------------------------------------------

### Method `email()`

get an email address

#### Usage

    FraudsterClient$email(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method [`url()`](https://rdrr.io/r/base/connections.html)

a url

#### Usage

    FraudsterClient$url(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `lorem_paragraph()`

Generate many paragraphs

#### Usage

    FraudsterClient$lorem_paragraph(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `ssn()`

Make a SSN (Social Security Number).

#### Usage

    FraudsterClient$ssn(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `mac_address()`

a mac address

#### Usage

    FraudsterClient$mac_address(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `element_symbol()`

create a element symbol

#### Usage

    FraudsterClient$element_symbol(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `hex_color()`

hex color

#### Usage

    FraudsterClient$hex_color(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `safe_hex_color()`

safe hex color

#### Usage

    FraudsterClient$safe_hex_color(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `rgb_color()`

rgb color

#### Usage

    FraudsterClient$rgb_color(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `rgb_css_color()`

rgb css color

#### Usage

    FraudsterClient$rgb_css_color(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `lat()`

latitude

#### Usage

    FraudsterClient$lat(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `lon()`

longitude

#### Usage

    FraudsterClient$lon(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `position()`

long/lat coordinate pair

#### Usage

    FraudsterClient$position(n = 1, bbox = NULL)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `bbox`:

  a bounding box, see
  [`ch_position()`](https://docs.ropensci.org/charlatan/reference/coordinates.md)

------------------------------------------------------------------------

### Method `doi()`

DOIs

#### Usage

    FraudsterClient$doi(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `timezone()`

date times

#### Usage

    FraudsterClient$timezone(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `unix_time()`

unix time

#### Usage

    FraudsterClient$unix_time(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method [`date_time()`](https://docs.ropensci.org/charlatan/reference/date_time.md)

date time

#### Usage

    FraudsterClient$date_time(n = 1, tzinfo = NULL)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `tzinfo`:

  timezone, see [timezone](https://rdrr.io/r/base/timezones.html)

------------------------------------------------------------------------

### Method `genus()`

taxonomic genus

#### Usage

    FraudsterClient$genus(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `epithet()`

taxonomic epithet

#### Usage

    FraudsterClient$epithet(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `species()`

taxonomic species (genus + epithet)

#### Usage

    FraudsterClient$species(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method [`sequence()`](https://rdrr.io/r/base/sequence.html)

random genetic sequence

#### Usage

    FraudsterClient$sequence(n = 1, length = 30)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `length`:

  (integer) length of the sequence. default: 30

------------------------------------------------------------------------

### Method [`double()`](https://rdrr.io/r/base/double.html)

a double

#### Usage

    FraudsterClient$double(n = 1, mean = 0, sd = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `mean`:

  mean value, default: 0

- `sd`:

  standard deviation, default: 1

------------------------------------------------------------------------

### Method [`integer()`](https://rdrr.io/r/base/integer.html)

an integer

#### Usage

    FraudsterClient$integer(n = 1, min = 1, max = 1000)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `min`:

  minimum value, default: 1

- `max`:

  maximum value, default: 1000

------------------------------------------------------------------------

### Method `uniform()`

an integer from a uniform distribution

#### Usage

    FraudsterClient$uniform(n = 1, min = 0, max = 9999)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `min`:

  minimum value, default: 0

- `max`:

  maximum value, default: 9999

------------------------------------------------------------------------

### Method [`norm()`](https://rdrr.io/r/base/norm.html)

an integer from a normal distribution

#### Usage

    FraudsterClient$norm(n = 1, mean = 0, sd = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `mean`:

  mean value, default: 0

- `sd`:

  standard deviation, default: 1

------------------------------------------------------------------------

### Method `lnorm()`

an integer from a lognormal distribution

#### Usage

    FraudsterClient$lnorm(n = 1, mean = 0, sd = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `mean`:

  mean value, default: 0

- `sd`:

  standard deviation, default: 1

------------------------------------------------------------------------

### Method [`beta()`](https://rdrr.io/r/base/Special.html)

an integer from a beta distribution

#### Usage

    FraudsterClient$beta(n = 1, shape1, shape2, ncp = 0)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

- `shape1`:

  non-negative parameters of the Beta distribution

- `shape2`:

  non-negative parameters of the Beta distribution

- `ncp`:

  non-centrality parameter, default: 0

------------------------------------------------------------------------

### Method `currency()`

currency

#### Usage

    FraudsterClient$currency(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `credit_card_provider()`

credit card provider

#### Usage

    FraudsterClient$credit_card_provider(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `credit_card_number()`

credit card number

#### Usage

    FraudsterClient$credit_card_number(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `credit_card_security_code()`

credit card security code

#### Usage

    FraudsterClient$credit_card_security_code(n = 1)

#### Arguments

- `n`:

  number of random things to generaate. an integer; default: 1

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    FraudsterClient$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
