# MissingDataProvider

make missing data

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `MissingDataProvider`

## Methods

### Public methods

- [`MissingDataProvider$make_missing()`](#method-MissingDataProvider-make_missing)

- [`MissingDataProvider$clone()`](#method-MissingDataProvider-clone)

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

### Method `make_missing()`

make missing data

#### Usage

    MissingDataProvider$make_missing(x)

#### Arguments

- `x`:

  a vector of characters, numeric, integers, logicals, etc

#### Details

This method picks a random number (`N`) of slots in the input vector `x`
(up to `length(x)`). Then picks `N` random positions and replaces them
with NA matching the input class.

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    MissingDataProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- MissingDataProvider$new()
z$make_missing(x = letters)
#>  [1] NA  NA  NA  NA  NA  NA  NA  NA  NA  NA  "k" NA  NA  NA  NA  NA  "q" NA  NA 
#> [20] NA  NA  NA  NA  NA  NA  NA 
```
