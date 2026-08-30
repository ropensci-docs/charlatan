# Create Localized Provider

Create Localized Provider

## Usage

``` r
subclass(provider, locale = NULL)
```

## Arguments

- provider:

  The name of the provider you want to create

- locale:

  Locale to use

## Value

Localized provider

## Examples

``` r
x <- subclass("AddressProvider")
#> Warning: No locale provided for  AddressProvider  defaulting to en_US
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
```
