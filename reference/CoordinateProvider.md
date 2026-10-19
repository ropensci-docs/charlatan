# CoordinateProvider

coordinates methods

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `CoordinateProvider`

## Methods

### Public methods

- [`CoordinateProvider$lon()`](#method-CoordinateProvider-lon)

- [`CoordinateProvider$lat()`](#method-CoordinateProvider-lat)

- [`CoordinateProvider$position()`](#method-CoordinateProvider-position)

- [`CoordinateProvider$clone()`](#method-CoordinateProvider-clone)

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

### Method `lon()`

a latitude value

#### Usage

    CoordinateProvider$lon()

------------------------------------------------------------------------

### Method `lat()`

a longitude value

#### Usage

    CoordinateProvider$lat()

------------------------------------------------------------------------

### Method `position()`

a position, of form `[longitude,latitude]`

#### Usage

    CoordinateProvider$position(bbox = NULL)

#### Arguments

- `bbox`:

  optionally, specify a bounding box for the position to be in, of the
  form `[west,south,east,north]` - checks that the bbox has valid values
  for lat and long

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    CoordinateProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- CoordinateProvider$new()
z$lon()
#> [1] 93.87401
z$lat()
#> [1] -88.04296
z$position()
#> [1] -157.27056  -42.50848
z$position(bbox = c(-120, 30, -110, 60))
#> [1] -114.0616   38.9268
```
