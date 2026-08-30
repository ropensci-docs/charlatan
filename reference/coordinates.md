# Create fake coordinates

Create fake coordinates

## Usage

``` r
ch_lon(n = 1)

ch_lat(n = 1)

ch_position(n = 1, bbox = NULL)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- bbox:

  a bounding box of the form `[w,s,e,n]`

## See also

[CoordinateProvider](https://docs.ropensci.org/charlatan/reference/CoordinateProvider.md)

## Examples

``` r
ch_lon()
#> [1] -108.1812
ch_lon(10)
#>  [1] -23.886744   7.790736 163.712059  79.698705  35.943234 138.860003
#>  [7] -24.601470 -24.366346 -35.637328 173.205845

ch_lat()
#> [1] -58.24318
ch_lat(10)
#>  [1]   9.446560  19.842189  24.871366  -8.660396  -3.050394 -31.209591
#>  [7] -29.108583 -88.657547 -68.613321  87.785768

ch_position()
#> [1] 49.49061 83.47938
ch_position(10)
#> [[1]]
#> [1] -93.40342  71.66036
#> 
#> [[2]]
#> [1] -41.49152 -44.80282
#> 
#> [[3]]
#> [1] -27.82014 -72.74738
#> 
#> [[4]]
#> [1] -101.1923  -16.2330
#> 
#> [[5]]
#> [1] 116.55821  46.32434
#> 
#> [[6]]
#> [1]  74.27417 -83.51964
#> 
#> [[7]]
#> [1] -74.810434  -7.643556
#> 
#> [[8]]
#> [1] 123.00337  84.30372
#> 
#> [[9]]
#> [1] 98.79158 77.77534
#> 
#> [[10]]
#> [1] 18.90133 11.84621
#> 
ch_position(bbox = c(-120, 30, -110, 60))
#> [1] -116.87508   42.23199
```
