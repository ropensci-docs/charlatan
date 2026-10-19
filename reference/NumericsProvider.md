# NumericsProvider

numeric methods, generate numbers

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `NumericsProvider`

## Methods

### Public methods

- [`NumericsProvider$double()`](#method-NumericsProvider-double)

- [`NumericsProvider$integer()`](#method-NumericsProvider-integer)

- [`NumericsProvider$unif()`](#method-NumericsProvider-unif)

- [`NumericsProvider$norm()`](#method-NumericsProvider-norm)

- [`NumericsProvider$lnorm()`](#method-NumericsProvider-lnorm)

- [`NumericsProvider$beta()`](#method-NumericsProvider-beta)

- [`NumericsProvider$clone()`](#method-NumericsProvider-clone)

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

### Method [`double()`](https://rdrr.io/r/base/double.html)

get a double, pulls from normal distribution

#### Usage

    NumericsProvider$double(n = 1, mean = 0, sd = 1)

#### Arguments

- `n`:

  (integer) number of values, default: 1

- `mean`:

  mean value, default: 0

- `sd`:

  standard deviation, default: 1

------------------------------------------------------------------------

### Method [`integer()`](https://rdrr.io/r/base/integer.html)

get an integer, runs [`sample()`](https://rdrr.io/r/base/sample.html) on
range given

#### Usage

    NumericsProvider$integer(n = 1, min = 1, max = 1000)

#### Arguments

- `n`:

  (integer) number of values, default: 1

- `min`:

  minimum value, default: 1

- `max`:

  maximum value, default: 1000

------------------------------------------------------------------------

### Method `unif()`

get numbers from the uniform distribution

#### Usage

    NumericsProvider$unif(n = 1, min = 0, max = 9999)

#### Arguments

- `n`:

  (integer) number of values, default: 1

- `min`:

  minimum value, default: 1

- `max`:

  maximum value, default: 1000

------------------------------------------------------------------------

### Method [`norm()`](https://rdrr.io/r/base/norm.html)

get numbers from the normal distribution

#### Usage

    NumericsProvider$norm(n = 1, mean = 0, sd = 1)

#### Arguments

- `n`:

  (integer) number of values, default: 1

- `mean`:

  mean value, default: 0

- `sd`:

  standard deviation, default: 1

------------------------------------------------------------------------

### Method `lnorm()`

get numbers from the lognormal distribution

#### Usage

    NumericsProvider$lnorm(n = 1, mean = 0, sd = 1)

#### Arguments

- `n`:

  (integer) number of values, default: 1

- `mean`:

  mean value, default: 0

- `sd`:

  standard deviation, default: 1

------------------------------------------------------------------------

### Method [`beta()`](https://rdrr.io/r/base/Special.html)

get numbers from the beta distribution

#### Usage

    NumericsProvider$beta(n = 1, shape1, shape2, ncp = 0)

#### Arguments

- `n`:

  (integer) number of values, default: 1

- `shape1`:

  non-negative parameters of the Beta distribution

- `shape2`:

  non-negative parameters of the Beta distribution

- `ncp`:

  non-centrality parameter, default: 0

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    NumericsProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- NumericsProvider$new()

z$double()
#> [1] 0.6274909
z$double(10)
#>  [1]  0.82250394 -0.02234212  1.72386032 -0.29242599 -0.33458009 -0.01715730
#>  [7] -2.04457881 -1.29253095 -1.29238974 -0.55272404
z$double(10, mean = 100)
#>  [1] 100.20243  99.61637  99.05393  98.76779 100.29301 100.11733 100.70762
#>  [8] 101.96876 100.87035  99.08668
z$double(10, mean = 100, sd = 17)
#>  [1] 103.78318  77.55447 122.33381  87.59693  84.16423 108.78935 104.79715
#>  [8]  82.02750  90.21246  74.43614

z$integer()
#> [1] 2
z$integer(10)
#>  [1] 924 842 259 574 688 997 779 585 934 604
z$integer(10, 1, 20)
#>  [1]  7 14 17 12  2 17 10  3 13 19
z$integer(10, 1, 10000000L)
#>  [1] 6328585 7688163  511873 2943010 9077977 8966956 1584793 9592701 9116674
#> [10] 1725078

z$unif()
#> [1] 8273.355
z$norm()
#> [1] 0.8385327
z$lnorm(10)
#>  [1] 2.88931184 1.99709958 1.95929785 0.94663397 0.38663518 0.05385108
#>  [7] 3.74354215 1.54297478 0.29396991 1.67507462
z$beta(10, 1, 1)
#>  [1] 0.81059553 0.05705297 0.09481279 0.95385979 0.57083511 0.33032058
#>  [7] 0.41852217 0.33992936 0.23875820 0.09864429
```
