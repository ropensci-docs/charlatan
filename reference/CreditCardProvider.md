# CreditCardProvider

credit card methods

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `CreditCardProvider`

## Public fields

- `luhn_lookup`:

  (list) luhn lookup, named list

## Methods

### Public methods

- [`CreditCardProvider$credit_card_type()`](#method-CreditCardProvider-credit_card_type)

- [`CreditCardProvider$generate_number()`](#method-CreditCardProvider-generate_number)

- [`CreditCardProvider$credit_card_provider()`](#method-CreditCardProvider-credit_card_provider)

- [`CreditCardProvider$credit_card_number()`](#method-CreditCardProvider-credit_card_number)

- [`CreditCardProvider$credit_card_security_code()`](#method-CreditCardProvider-credit_card_security_code)

- [`CreditCardProvider$clone()`](#method-CreditCardProvider-clone)

Inherited methods

- [`charlatan::BareProvider$bothify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-bothify)
- [`charlatan::BareProvider$lexify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-lexify)
- [`charlatan::BareProvider$numerify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-numerify)
- [`charlatan::BareProvider$print()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-print)
- [`charlatan::BareProvider$random_digit()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit)
- [`charlatan::BareProvider$random_digit_not_zero()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero)
- [`charlatan::BareProvider$random_digit_not_zero_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero_or_empty)
- [`charlatan::BareProvider$random_digit_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_or_empty)
- [`charlatan::BareProvider$random_element()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element)
- [`charlatan::BareProvider$random_element_prob()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element_prob)
- [`charlatan::BareProvider$random_int()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_int)
- [`charlatan::BareProvider$random_letter()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_letter)
- [`charlatan::BareProvider$randomize_nb_elements()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-randomize_nb_elements)

------------------------------------------------------------------------

### Method `credit_card_type()`

Returns a random credit card type

#### Usage

    CreditCardProvider$credit_card_type(card_type = NULL)

#### Arguments

- `card_type`:

  (character) a card type, see `credit_card_types`

------------------------------------------------------------------------

### Method `generate_number()`

make a credit card number with specific starting numbers

#### Usage

    CreditCardProvider$generate_number(prefix, length = 13)

#### Arguments

- `prefix`:

  the start of the CC number as a string, any number of digits.

- `length`:

  the length of the CC number to generate. Typically 13 or 16

------------------------------------------------------------------------

### Method `credit_card_provider()`

credit card provider

#### Usage

    CreditCardProvider$credit_card_provider(card_type = NULL)

#### Arguments

- `card_type`:

  (character) a card type, see `credit_card_types`

------------------------------------------------------------------------

### Method `credit_card_number()`

credit card number

#### Usage

    CreditCardProvider$credit_card_number(card_type = NULL)

#### Arguments

- `card_type`:

  (character) a card type, see `credit_card_types`

------------------------------------------------------------------------

### Method `credit_card_security_code()`

credit card security code

#### Usage

    CreditCardProvider$credit_card_security_code(card_type = NULL)

#### Arguments

- `card_type`:

  (character) a card type, see `credit_card_types`

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CreditCardProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- CreditCardProvider$new()
z$credit_card_provider()
#> [1] "Voyager"
z$credit_card_number()
#> [1] "52800008128475030"
z$credit_card_security_code()
#> [1] "216"
z$generate_number(13)
#> [1] "13991459652327"
```
