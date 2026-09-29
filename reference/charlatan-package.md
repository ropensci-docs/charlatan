# charlatan

Make fake data, supporting addresses, person names, dates, times,
colors, coordinates, currencies, digital object identifiers (DOIs),
jobs, phone numbers, DNA sequences, doubles and integers from
distributions and within a range.

## Package API

- [`ch_generate()`](https://docs.ropensci.org/charlatan/reference/ch_generate.md):
  generate a data.frame with fake data

- [`fraudster()`](https://docs.ropensci.org/charlatan/reference/fraudster.md):
  single interface to all fake data methods

- High level interfaces: There are high level functions prefixed with
  `ch_` that wrap low level interfaces, and are meant to be easier to
  use and provide easy way to make many instances of a thing.

- Low level interfaces: All of these are R6 objects that a user can
  initialize and then call methods on the them.

## See also

Useful links:

- <https://docs.ropensci.org/charlatan/>

- <https://github.com/ropensci/charlatan>

- Report bugs at <https://github.com/ropensci/charlatan/issues>

## Author

Roel M. Hogervorst <hogervorst.rm@gmail.com>

Scott Chamberlain

Kyle Voytovich

Martin Pedersen

## Examples

``` r
# generate individual types of data
ch_name()
#> [1] "Dr. Job Raynor PhD"
ch_phone_number()
#> [1] "070.087.3124x5939"
ch_job()
#> [1] "Sub"

# generate a data.frame
ch_generate()
#> # A tibble: 10 × 3
#>    name                  job                         phone_number       
#>    <chr>                 <chr>                       <chr>              
#>  1 Emma Abbott PhD       Public librarian            (232)230-2847      
#>  2 Deangelo Stanton      Air cabin crew              1-926-376-7152     
#>  3 Dr. Bliss Dickinson   Building control surveyor   (404)673-6003x34435
#>  4 Bena Wuckert          Engineer, land              902-068-5906x97034 
#>  5 Orvis Weissnat        Engineer, building services 604.074.0862x24194 
#>  6 Nanette Kohler        Probation officer           726-129-4270x28623 
#>  7 Darin Durgan          Energy manager              657.178.4982       
#>  8 Millie Bahringer      Airline pilot               854-078-1425x6042  
#>  9 Dr. Rosey Watsica MD  Secondary school teacher    +34(9)9200345364   
#> 10 Mrs. Courtney Lind MD Publishing copy             385-631-0667x312   

# one interface to all data types - generate the class first
#  reports the locale to be used, can change optionally
(x <- fraudster())
#> <fraudster>
#>   locale: en_US
x$job()
#> [1] "Financial adviser"
x$name()
#> [1] "Ms. Jessie Pouros DDS"
x$color_name()
#> [1] "AliceBlue"
x$hex_color()
#> [1] "#832436"

# low level interfaces to "data providers"
# these are exported by hidden from package man page
# as most users will likely not interact with these
x <- ColorProvider_en_US$new()
x$color_name()
#> [1] "FloralWhite"
x$hex_color()
#> [1] "#F9CA7B"
```
