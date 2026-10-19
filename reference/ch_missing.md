# Create missing data

Create missing data

## Usage

``` r
ch_missing(x, n = 1)
```

## Arguments

- x:

  Input vector, can be any class - only 1 vetor

- n:

  (integer) number of things to get, any non-negative integer

## See also

[MissingDataProvider](https://docs.ropensci.org/charlatan/reference/MissingDataProvider.md)

## Examples

``` r
ch_missing(letters)
#>  [1] NA  NA  "c" NA  "e" "f" NA  "h" NA  "j" "k" NA  "m" NA  "o" "p" "q" NA  "s"
#> [20] "t" NA  NA  NA  "x" NA  NA 
ch_missing(letters, 10)
#>       [,1] [,2] [,3] [,4] [,5] [,6] [,7] [,8] [,9] [,10]
#>  [1,] "a"  NA   NA   "a"  "a"  NA   "a"  "a"  "a"  NA   
#>  [2,] NA   NA   NA   "b"  "b"  "b"  "b"  "b"  "b"  NA   
#>  [3,] "c"  NA   NA   "c"  "c"  NA   NA   NA   "c"  NA   
#>  [4,] "d"  NA   NA   "d"  "d"  NA   "d"  "d"  NA   NA   
#>  [5,] "e"  NA   NA   "e"  "e"  "e"  NA   "e"  "e"  NA   
#>  [6,] "f"  NA   "f"  "f"  "f"  "f"  "f"  "f"  NA   NA   
#>  [7,] "g"  NA   NA   "g"  NA   "g"  NA   "g"  "g"  NA   
#>  [8,] "h"  NA   NA   "h"  "h"  NA   "h"  "h"  "h"  "h"  
#>  [9,] "i"  NA   NA   "i"  "i"  "i"  NA   "i"  "i"  NA   
#> [10,] "j"  NA   NA   "j"  "j"  "j"  NA   "j"  "j"  NA   
#> [11,] "k"  NA   NA   "k"  "k"  NA   "k"  "k"  "k"  NA   
#> [12,] "l"  NA   NA   "l"  "l"  NA   "l"  NA   "l"  NA   
#> [13,] "m"  NA   "m"  "m"  "m"  "m"  NA   NA   "m"  "m"  
#> [14,] NA   NA   NA   "n"  "n"  "n"  "n"  "n"  "n"  NA   
#> [15,] "o"  NA   "o"  "o"  "o"  NA   NA   NA   NA   NA   
#> [16,] "p"  NA   NA   "p"  "p"  NA   "p"  "p"  NA   NA   
#> [17,] "q"  NA   NA   "q"  "q"  NA   "q"  NA   "q"  NA   
#> [18,] "r"  NA   NA   "r"  "r"  NA   NA   NA   "r"  NA   
#> [19,] "s"  NA   NA   NA   "s"  NA   "s"  "s"  NA   NA   
#> [20,] "t"  NA   NA   "t"  NA   NA   "t"  NA   "t"  NA   
#> [21,] "u"  NA   NA   "u"  "u"  NA   "u"  "u"  "u"  NA   
#> [22,] NA   NA   NA   "v"  "v"  NA   "v"  "v"  "v"  NA   
#> [23,] "w"  NA   NA   "w"  "w"  NA   NA   NA   "w"  NA   
#> [24,] "x"  NA   NA   "x"  "x"  NA   NA   "x"  "x"  NA   
#> [25,] "y"  NA   NA   "y"  NA   NA   "y"  NA   NA   NA   
#> [26,] "z"  NA   NA   "z"  "z"  NA   NA   NA   "z"  NA   
ch_missing(letters, 20)
#>       [,1] [,2] [,3] [,4] [,5] [,6] [,7] [,8] [,9] [,10] [,11] [,12] [,13]
#>  [1,] "a"  NA   NA   NA   "a"  "a"  NA   "a"  NA   NA    NA    "a"   "a"  
#>  [2,] "b"  NA   "b"  NA   "b"  "b"  NA   "b"  NA   NA    NA    "b"   NA   
#>  [3,] NA   "c"  NA   NA   NA   "c"  NA   NA   NA   NA    "c"   "c"   NA   
#>  [4,] "d"  "d"  "d"  NA   "d"  "d"  NA   "d"  NA   NA    NA    NA    NA   
#>  [5,] "e"  NA   "e"  NA   "e"  "e"  "e"  "e"  "e"  NA    NA    NA    NA   
#>  [6,] "f"  "f"  NA   NA   "f"  "f"  NA   NA   "f"  NA    NA    "f"   NA   
#>  [7,] "g"  "g"  "g"  NA   "g"  "g"  "g"  "g"  NA   NA    NA    "g"   NA   
#>  [8,] "h"  "h"  "h"  NA   "h"  "h"  NA   "h"  NA   NA    NA    "h"   NA   
#>  [9,] "i"  "i"  "i"  NA   "i"  "i"  NA   "i"  NA   NA    "i"   NA    NA   
#> [10,] "j"  "j"  NA   NA   "j"  "j"  NA   "j"  "j"  "j"   "j"   "j"   NA   
#> [11,] "k"  "k"  "k"  NA   NA   NA   NA   "k"  NA   NA    NA    "k"   NA   
#> [12,] "l"  "l"  "l"  NA   "l"  "l"  NA   NA   NA   NA    "l"   "l"   NA   
#> [13,] "m"  "m"  NA   NA   "m"  "m"  NA   NA   NA   "m"   NA    "m"   NA   
#> [14,] "n"  "n"  "n"  NA   NA   "n"  NA   NA   NA   NA    "n"   "n"   NA   
#> [15,] "o"  "o"  "o"  NA   "o"  NA   NA   "o"  "o"  NA    NA    "o"   NA   
#> [16,] "p"  "p"  "p"  NA   NA   "p"  NA   NA   NA   "p"   NA    "p"   NA   
#> [17,] "q"  "q"  NA   NA   "q"  "q"  NA   "q"  NA   NA    "q"   NA    NA   
#> [18,] "r"  "r"  NA   NA   "r"  "r"  NA   "r"  NA   NA    "r"   "r"   NA   
#> [19,] "s"  "s"  NA   NA   "s"  "s"  NA   NA   "s"  "s"   NA    "s"   NA   
#> [20,] "t"  NA   "t"  NA   "t"  NA   NA   "t"  NA   NA    "t"   "t"   NA   
#> [21,] "u"  NA   "u"  NA   NA   "u"  NA   NA   NA   NA    NA    "u"   NA   
#> [22,] "v"  "v"  "v"  NA   "v"  NA   NA   "v"  NA   "v"   NA    "v"   NA   
#> [23,] "w"  NA   "w"  NA   "w"  "w"  NA   "w"  NA   NA    NA    "w"   NA   
#> [24,] "x"  "x"  "x"  NA   "x"  NA   NA   "x"  NA   NA    NA    NA    NA   
#> [25,] "y"  NA   "y"  NA   "y"  "y"  NA   "y"  NA   NA    NA    "y"   NA   
#> [26,] "z"  "z"  "z"  NA   "z"  "z"  NA   "z"  "z"  NA    NA    "z"   NA   
#>       [,14] [,15] [,16] [,17] [,18] [,19] [,20]
#>  [1,] "a"   "a"   NA    NA    NA    "a"   "a"  
#>  [2,] "b"   "b"   NA    NA    NA    NA    NA   
#>  [3,] "c"   "c"   NA    "c"   NA    NA    NA   
#>  [4,] "d"   "d"   NA    "d"   NA    NA    NA   
#>  [5,] "e"   "e"   NA    NA    NA    NA    "e"  
#>  [6,] "f"   "f"   NA    "f"   NA    NA    NA   
#>  [7,] "g"   "g"   NA    "g"   NA    "g"   NA   
#>  [8,] "h"   "h"   NA    NA    NA    NA    "h"  
#>  [9,] "i"   "i"   NA    NA    NA    NA    NA   
#> [10,] NA    "j"   NA    NA    NA    NA    "j"  
#> [11,] "k"   "k"   NA    NA    NA    NA    NA   
#> [12,] "l"   NA    NA    NA    NA    NA    "l"  
#> [13,] "m"   "m"   NA    "m"   NA    NA    "m"  
#> [14,] NA    "n"   NA    NA    NA    NA    NA   
#> [15,] "o"   NA    NA    "o"   NA    NA    "o"  
#> [16,] "p"   "p"   NA    NA    NA    NA    "p"  
#> [17,] "q"   "q"   NA    "q"   "q"   NA    "q"  
#> [18,] "r"   NA    NA    "r"   NA    "r"   "r"  
#> [19,] "s"   "s"   NA    "s"   NA    NA    "s"  
#> [20,] "t"   "t"   NA    NA    NA    NA    "t"  
#> [21,] "u"   "u"   NA    "u"   NA    NA    NA   
#> [22,] "v"   NA    NA    "v"   NA    "v"   NA   
#> [23,] "w"   "w"   NA    NA    NA    NA    "w"  
#> [24,] "x"   "x"   NA    "x"   NA    "x"   NA   
#> [25,] "y"   "y"   NA    NA    NA    NA    "y"  
#> [26,] "z"   "z"   NA    "z"   NA    "z"   NA   
```
