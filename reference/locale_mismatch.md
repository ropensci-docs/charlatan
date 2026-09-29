# Find mismatch between parent and child locales

Find mismatch between parent and child locales

## Usage

``` r
locale_mismatch(parent_provider, child_provider)
```

## Arguments

- parent_provider:

  provider that you want the locales to check for

- child_provider:

  provider where we check if parent locales are in. For example
  InternetProvider has en_AU but LoremProvider does not.

## Value

locales that ARE in the parent, but are not available in the child.
