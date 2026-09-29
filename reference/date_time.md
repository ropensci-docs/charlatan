# Create dates and times

Create dates and times

## Usage

``` r
ch_timezone(n = 1)

ch_unix_time(n = 1)

ch_date_time(n = 1)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

## See also

[DateTimeProvider](https://docs.ropensci.org/charlatan/reference/DateTimeProvider.md)

## Examples

``` r
ch_timezone()
#> [[1]]
#> [[1]][[1]]
#> [1] "Asia/Riyadh"
#> 
#> [[1]]$code
#> [1] "SA"
#> 
#> [[1]]$continent
#> [1] "Asia"
#> 
#> [[1]]$name
#> [1] "Saudi Arabia"
#> 
#> [[1]]$capital
#> [1] "Riyadh"
#> 
#> 
ch_timezone(10)
#> [[1]]
#> [[1]][[1]]
#> [1] "Africa/Lusaka"
#> 
#> [[1]]$code
#> [1] "ZM"
#> 
#> [[1]]$continent
#> [1] "Africa"
#> 
#> [[1]]$name
#> [1] "Zambia"
#> 
#> [[1]]$capital
#> [1] "Lusaka"
#> 
#> 
#> [[2]]
#> [[2]][[1]]
#> [1] "America/Dominica"
#> 
#> [[2]]$code
#> [1] "DM"
#> 
#> [[2]]$continent
#> [1] "North America"
#> 
#> [[2]]$name
#> [1] "Dominica"
#> 
#> [[2]]$capital
#> [1] "Roseau"
#> 
#> 
#> [[3]]
#> [[3]][[1]]
#> [1] "America/Santo_Domingo"
#> 
#> [[3]]$code
#> [1] "DO"
#> 
#> [[3]]$continent
#> [1] "North America"
#> 
#> [[3]]$name
#> [1] "Dominican Republic"
#> 
#> [[3]]$capital
#> [1] "Santo Domingo"
#> 
#> 
#> [[4]]
#> [[4]][[1]]
#> [1] "Asia/Kuwait"
#> 
#> [[4]]$code
#> [1] "KW"
#> 
#> [[4]]$continent
#> [1] "Asia"
#> 
#> [[4]]$name
#> [1] "Kuwait"
#> 
#> [[4]]$capital
#> [1] "Kuwait City"
#> 
#> 
#> [[5]]
#> [[5]][[1]]
#> [1] "America/Guatemala"
#> 
#> [[5]]$code
#> [1] "GT"
#> 
#> [[5]]$continent
#> [1] "North America"
#> 
#> [[5]]$name
#> [1] "Haiti"
#> 
#> [[5]]$capital
#> [1] "Port-au-Prince"
#> 
#> 
#> [[6]]
#> [[6]][[1]]
#> [1] "Europe/Budapest"
#> 
#> [[6]]$code
#> [1] "HU"
#> 
#> [[6]]$continent
#> [1] "Europe"
#> 
#> [[6]]$name
#> [1] "Hungary"
#> 
#> [[6]]$capital
#> [1] "Budapest"
#> 
#> 
#> [[7]]
#> [[7]][[1]]
#> [1] "America/Lima"
#> 
#> [[7]]$code
#> [1] "PE"
#> 
#> [[7]]$continent
#> [1] "South America"
#> 
#> [[7]]$name
#> [1] "Peru"
#> 
#> [[7]]$capital
#> [1] "Lima"
#> 
#> 
#> [[8]]
#> [[8]][[1]]
#> [1] "America/La_Paz"
#> 
#> [[8]]$code
#> [1] "BO"
#> 
#> [[8]]$continent
#> [1] "South America"
#> 
#> [[8]]$name
#> [1] "Bolivia"
#> 
#> [[8]]$capital
#> [1] "Sucre"
#> 
#> 
#> [[9]]
#> [[9]][[1]]
#> [1] "Europe/Istanbul"
#> 
#> [[9]]$code
#> [1] "TR"
#> 
#> [[9]]$continent
#> [1] "Asia"
#> 
#> [[9]]$name
#> [1] "Turkey"
#> 
#> [[9]]$capital
#> [1] "Ankara"
#> 
#> 
#> [[10]]
#> [[10]][[1]]
#> [1] "Europe/Dublin"
#> 
#> [[10]]$code
#> [1] "IE"
#> 
#> [[10]]$continent
#> [1] "Europe"
#> 
#> [[10]]$name
#> [1] "Republic of Ireland"
#> 
#> [[10]]$capital
#> [1] "Dublin"
#> 
#> 

ch_unix_time()
#> [1] 113662259
ch_unix_time(20)
#>  [1] 1328871724 1650834172  160056718 1523437171   22104268  546563339
#>  [7]   50754396  337847381  655176008  225148779 1475383621 1149143058
#> [13] 1332383042  834603208  392687067 1016029832 1115499326 1420257130
#> [19]  610739009  743096837

ch_date_time()
#> [1] "1980-11-23 08:12:08 UTC"
ch_date_time(20)
#> [[1]]
#> [1] "1982-04-02 20:10:25 UTC"
#> 
#> [[2]]
#> [1] "1985-02-08 19:04:16 UTC"
#> 
#> [[3]]
#> [1] "2004-03-14 23:21:32 UTC"
#> 
#> [[4]]
#> [1] "1977-05-01 04:49:42 UTC"
#> 
#> [[5]]
#> [1] "1976-02-08 12:47:35 UTC"
#> 
#> [[6]]
#> [1] "1983-04-12 03:55:47 UTC"
#> 
#> [[7]]
#> [1] "1999-11-07 04:24:11 UTC"
#> 
#> [[8]]
#> [1] "2014-06-29 20:39:49 UTC"
#> 
#> [[9]]
#> [1] "1988-09-19 15:56:48 UTC"
#> 
#> [[10]]
#> [1] "2025-07-14 05:23:57 UTC"
#> 
#> [[11]]
#> [1] "1989-06-09 21:29:42 UTC"
#> 
#> [[12]]
#> [1] "1987-01-01 15:14:57 UTC"
#> 
#> [[13]]
#> [1] "1971-02-05 06:57:42 UTC"
#> 
#> [[14]]
#> [1] "2013-11-21 20:16:48 UTC"
#> 
#> [[15]]
#> [1] "2019-10-18 09:35:20 UTC"
#> 
#> [[16]]
#> [1] "2016-01-05 16:33:57 UTC"
#> 
#> [[17]]
#> [1] "1991-01-24 15:57:09 UTC"
#> 
#> [[18]]
#> [1] "1976-04-25 11:23:13 UTC"
#> 
#> [[19]]
#> [1] "1974-03-12 21:28:08 UTC"
#> 
#> [[20]]
#> [1] "1988-06-22 09:06:23 UTC"
#> 
```
