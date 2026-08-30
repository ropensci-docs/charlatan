# DateTimeProvider

date and time methods

## References

https://en.wikipedia.org/wiki/Unix_time

https://en.wikipedia.org/wiki/Unix_time

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `DateTimeProvider`

## Public fields

- `centuries`:

  (character) centuries in roman numerals

- `countries`:

  (list) countries list

## Methods

### Public methods

- [`DateTimeProvider$unix_time()`](#method-DateTimeProvider-unix_time)

- [`DateTimeProvider$date()`](#method-DateTimeProvider-date)

- [`DateTimeProvider$date_time()`](#method-DateTimeProvider-date_time)

- [`DateTimeProvider$date_time_fromtimestamp()`](#method-DateTimeProvider-date_time_fromtimestamp)

- [`DateTimeProvider$iso8601()`](#method-DateTimeProvider-iso8601)

- [`DateTimeProvider$year()`](#method-DateTimeProvider-year)

- [`DateTimeProvider$century()`](#method-DateTimeProvider-century)

- [`DateTimeProvider$timezone()`](#method-DateTimeProvider-timezone)

- [`DateTimeProvider$date_time_between()`](#method-DateTimeProvider-date_time_between)

- [`DateTimeProvider$clone()`](#method-DateTimeProvider-clone)

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

### Method `unix_time()`

Get a timestamp between January 1, 1970 and now, unless passed explicit
`start_date` or `end_date` values

#### Usage

    DateTimeProvider$unix_time(start_date = NULL, end_date = "now")

#### Arguments

- `start_date`:

  start date, a valid date format

- `end_date`:

  start date, a valid date format, default: "now"

------------------------------------------------------------------------

### Method [`date()`](https://rdrr.io/r/base/date.html)

Generate a date between January 1, 1970 and now, with given pattern

#### Usage

    DateTimeProvider$date(pattern = "%Y-%m-%d")

#### Arguments

- `pattern`:

  date pattern, default: `%Y-%m-%d`

------------------------------------------------------------------------

### Method [`date_time()`](https://docs.ropensci.org/charlatan/reference/date_time.md)

Generate a date time between January 1, 1970 and now

#### Usage

    DateTimeProvider$date_time(tzinfo = NULL)

#### Arguments

- `tzinfo`:

  timezone, see [timezone](https://rdrr.io/r/base/timezones.html)

------------------------------------------------------------------------

### Method `date_time_fromtimestamp()`

Generate a iso8601 format date

#### Usage

    DateTimeProvider$date_time_fromtimestamp(timestamp, tzinfo = NULL)

#### Arguments

- `timestamp`:

  a timestamp

- `tzinfo`:

  timezone, see [timezone](https://rdrr.io/r/base/timezones.html)

------------------------------------------------------------------------

### Method `iso8601()`

Generate a iso8601 format date

#### Usage

    DateTimeProvider$iso8601(date, tzinfo = NULL)

#### Arguments

- `date`:

  a date, in a valid date format

- `tzinfo`:

  timezone, see [timezone](https://rdrr.io/r/base/timezones.html)

------------------------------------------------------------------------

### Method `year()`

generate a year

#### Usage

    DateTimeProvider$year()

------------------------------------------------------------------------

### Method `century()`

generate a century

#### Usage

    DateTimeProvider$century()

------------------------------------------------------------------------

### Method `timezone()`

generate a timezone

#### Usage

    DateTimeProvider$timezone()

------------------------------------------------------------------------

### Method `date_time_between()`

Generate a date time based on a random date between two given dates

#### Usage

    DateTimeProvider$date_time_between(start_date, end_date = "now", tzinfo = NULL)

#### Arguments

- `start_date`:

  start date, a valid date format

- `end_date`:

  start date, a valid date format, default: "now"

- `tzinfo`:

  timezone, see [timezone](https://rdrr.io/r/base/timezones.html)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    DateTimeProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- DateTimeProvider$new()
z$countries
#> [[1]]
#> [[1]][[1]]
#> [1] "Europe/Andorra"
#> 
#> [[1]]$code
#> [1] "AD"
#> 
#> [[1]]$continent
#> [1] "Europe"
#> 
#> [[1]]$name
#> [1] "Andorra"
#> 
#> [[1]]$capital
#> [1] "Andorra la Vella"
#> 
#> 
#> [[2]]
#> [[2]][[1]]
#> [1] "Asia/Kabul"
#> 
#> [[2]]$code
#> [1] "AF"
#> 
#> [[2]]$continent
#> [1] "Asia"
#> 
#> [[2]]$name
#> [1] "Afghanistan"
#> 
#> [[2]]$capital
#> [1] "Kabul"
#> 
#> 
#> [[3]]
#> [[3]][[1]]
#> [1] "America/Antigua"
#> 
#> [[3]]$code
#> [1] "AG"
#> 
#> [[3]]$continent
#> [1] "North America"
#> 
#> [[3]]$name
#> [1] "Antigua and Barbuda"
#> 
#> [[3]]$capital
#> [1] "St. John's"
#> 
#> 
#> [[4]]
#> [[4]][[1]]
#> [1] "Europe/Tirane"
#> 
#> [[4]]$code
#> [1] "AL"
#> 
#> [[4]]$continent
#> [1] "Europe"
#> 
#> [[4]]$name
#> [1] "Albania"
#> 
#> [[4]]$capital
#> [1] "Tirana"
#> 
#> 
#> [[5]]
#> [[5]][[1]]
#> [1] "Asia/Yerevan"
#> 
#> [[5]]$code
#> [1] "AM"
#> 
#> [[5]]$continent
#> [1] "Asia"
#> 
#> [[5]]$name
#> [1] "Armenia"
#> 
#> [[5]]$capital
#> [1] "Yerevan"
#> 
#> 
#> [[6]]
#> [[6]][[1]]
#> [1] "Africa/Luanda"
#> 
#> [[6]]$code
#> [1] "AO"
#> 
#> [[6]]$continent
#> [1] "Africa"
#> 
#> [[6]]$name
#> [1] "Angola"
#> 
#> [[6]]$capital
#> [1] "Luanda"
#> 
#> 
#> [[7]]
#> [[7]][[1]]
#>  [1] "America/Argentina/Buenos_Aires" "America/Argentina/Cordoba"     
#>  [3] "America/Argentina/Jujuy"        "America/Argentina/Tucuman"     
#>  [5] "America/Argentina/Catamarca"    "America/Argentina/La_Rioja"    
#>  [7] "America/Argentina/San_Juan"     "America/Argentina/Mendoza"     
#>  [9] "America/Argentina/Rio_Gallegos" "America/Argentina/Ushuaia"     
#> 
#> [[7]]$code
#> [1] "AR"
#> 
#> [[7]]$continent
#> [1] "South America"
#> 
#> [[7]]$name
#> [1] "Argentina"
#> 
#> [[7]]$capital
#> [1] "Buenos Aires"
#> 
#> 
#> [[8]]
#> [[8]][[1]]
#> [1] "Europe/Vienna"
#> 
#> [[8]]$code
#> [1] "AT"
#> 
#> [[8]]$continent
#> [1] "Europe"
#> 
#> [[8]]$name
#> [1] "Austria"
#> 
#> [[8]]$capital
#> [1] "Vienna"
#> 
#> 
#> [[9]]
#> [[9]][[1]]
#>  [1] "Australia/Lord_Howe"   "Australia/Hobart"      "Australia/Currie"     
#>  [4] "Australia/Melbourne"   "Australia/Sydney"      "Australia/Broken_Hill"
#>  [7] "Australia/Brisbane"    "Australia/Lindeman"    "Australia/Adelaide"   
#> [10] "Australia/Darwin"      "Australia/Perth"      
#> 
#> [[9]]$code
#> [1] "AU"
#> 
#> [[9]]$continent
#> [1] "Oceania"
#> 
#> [[9]]$name
#> [1] "Australia"
#> 
#> [[9]]$capital
#> [1] "Canberra"
#> 
#> 
#> [[10]]
#> [[10]][[1]]
#> [1] "Asia/Baku"
#> 
#> [[10]]$code
#> [1] "AZ"
#> 
#> [[10]]$continent
#> [1] "Asia"
#> 
#> [[10]]$name
#> [1] "Azerbaijan"
#> 
#> [[10]]$capital
#> [1] "Baku"
#> 
#> 
#> [[11]]
#> [[11]][[1]]
#> [1] "America/Barbados"
#> 
#> [[11]]$code
#> [1] "BB"
#> 
#> [[11]]$continent
#> [1] "North America"
#> 
#> [[11]]$name
#> [1] "Barbados"
#> 
#> [[11]]$capital
#> [1] "Bridgetown"
#> 
#> 
#> [[12]]
#> [[12]][[1]]
#> [1] "Asia/Dhaka"
#> 
#> [[12]]$code
#> [1] "BD"
#> 
#> [[12]]$continent
#> [1] "Asia"
#> 
#> [[12]]$name
#> [1] "Bangladesh"
#> 
#> [[12]]$capital
#> [1] "Dhaka"
#> 
#> 
#> [[13]]
#> [[13]][[1]]
#> [1] "Europe/Brussels"
#> 
#> [[13]]$code
#> [1] "BE"
#> 
#> [[13]]$continent
#> [1] "Europe"
#> 
#> [[13]]$name
#> [1] "Belgium"
#> 
#> [[13]]$capital
#> [1] "Brussels"
#> 
#> 
#> [[14]]
#> [[14]][[1]]
#> [1] "Africa/Ouagadougou"
#> 
#> [[14]]$code
#> [1] "BF"
#> 
#> [[14]]$continent
#> [1] "Africa"
#> 
#> [[14]]$name
#> [1] "Burkina Faso"
#> 
#> [[14]]$capital
#> [1] "Ouagadougou"
#> 
#> 
#> [[15]]
#> [[15]][[1]]
#> [1] "Europe/Sofia"
#> 
#> [[15]]$code
#> [1] "BG"
#> 
#> [[15]]$continent
#> [1] "Europe"
#> 
#> [[15]]$name
#> [1] "Bulgaria"
#> 
#> [[15]]$capital
#> [1] "Sofia"
#> 
#> 
#> [[16]]
#> [[16]][[1]]
#> [1] "Asia/Bahrain"
#> 
#> [[16]]$code
#> [1] "BH"
#> 
#> [[16]]$continent
#> [1] "Asia"
#> 
#> [[16]]$name
#> [1] "Bahrain"
#> 
#> [[16]]$capital
#> [1] "Manama"
#> 
#> 
#> [[17]]
#> [[17]][[1]]
#> [1] "Africa/Bujumbura"
#> 
#> [[17]]$code
#> [1] "BI"
#> 
#> [[17]]$continent
#> [1] "Africa"
#> 
#> [[17]]$name
#> [1] "Burundi"
#> 
#> [[17]]$capital
#> [1] "Bujumbura"
#> 
#> 
#> [[18]]
#> [[18]][[1]]
#> [1] "Africa/Porto-Novo"
#> 
#> [[18]]$code
#> [1] "BJ"
#> 
#> [[18]]$continent
#> [1] "Africa"
#> 
#> [[18]]$name
#> [1] "Benin"
#> 
#> [[18]]$capital
#> [1] "Porto-Novo"
#> 
#> 
#> [[19]]
#> [[19]][[1]]
#> [1] "Asia/Brunei"
#> 
#> [[19]]$code
#> [1] "BN"
#> 
#> [[19]]$continent
#> [1] "Asia"
#> 
#> [[19]]$name
#> [1] "Brunei Darussalam"
#> 
#> [[19]]$capital
#> [1] "Bandar Seri Begawan"
#> 
#> 
#> [[20]]
#> [[20]][[1]]
#> [1] "America/La_Paz"
#> 
#> [[20]]$code
#> [1] "BO"
#> 
#> [[20]]$continent
#> [1] "South America"
#> 
#> [[20]]$name
#> [1] "Bolivia"
#> 
#> [[20]]$capital
#> [1] "Sucre"
#> 
#> 
#> [[21]]
#> [[21]][[1]]
#>  [1] "America/Noronha"      "America/Belem"        "America/Fortaleza"   
#>  [4] "America/Recife"       "America/Araguaina"    "America/Maceio"      
#>  [7] "America/Bahia"        "America/Sao_Paulo"    "America/Campo_Grande"
#> [10] "America/Cuiaba"       "America/Porto_Velho"  "America/Boa_Vista"   
#> [13] "America/Manaus"       "America/Eirunepe"     "America/Rio_Branco"  
#> 
#> [[21]]$code
#> [1] "BR"
#> 
#> [[21]]$continent
#> [1] "South America"
#> 
#> [[21]]$name
#> [1] "Brazil"
#> 
#> [[21]]$capital
#> [1] "Brasília"
#> 
#> 
#> [[22]]
#> [[22]][[1]]
#> [1] "America/Nassau"
#> 
#> [[22]]$code
#> [1] "BS"
#> 
#> [[22]]$continent
#> [1] "North America"
#> 
#> [[22]]$name
#> [1] "Bahamas"
#> 
#> [[22]]$capital
#> [1] "Nassau"
#> 
#> 
#> [[23]]
#> [[23]][[1]]
#> [1] "Asia/Thimphu"
#> 
#> [[23]]$code
#> [1] "BT"
#> 
#> [[23]]$continent
#> [1] "Asia"
#> 
#> [[23]]$name
#> [1] "Bhutan"
#> 
#> [[23]]$capital
#> [1] "Thimphu"
#> 
#> 
#> [[24]]
#> [[24]][[1]]
#> [1] "Africa/Gaborone"
#> 
#> [[24]]$code
#> [1] "BW"
#> 
#> [[24]]$continent
#> [1] "Africa"
#> 
#> [[24]]$name
#> [1] "Botswana"
#> 
#> [[24]]$capital
#> [1] "Gaborone"
#> 
#> 
#> [[25]]
#> [[25]][[1]]
#> [1] "Europe/Minsk"
#> 
#> [[25]]$code
#> [1] "BY"
#> 
#> [[25]]$continent
#> [1] "Europe"
#> 
#> [[25]]$name
#> [1] "Belarus"
#> 
#> [[25]]$capital
#> [1] "Minsk"
#> 
#> 
#> [[26]]
#> [[26]][[1]]
#> [1] "America/Belize"
#> 
#> [[26]]$code
#> [1] "BZ"
#> 
#> [[26]]$continent
#> [1] "North America"
#> 
#> [[26]]$name
#> [1] "Belize"
#> 
#> [[26]]$capital
#> [1] "Belmopan"
#> 
#> 
#> [[27]]
#> [[27]][[1]]
#>  [1] "America/St_Johns"      "America/Halifax"       "America/Glace_Bay"    
#>  [4] "America/Moncton"       "America/Goose_Bay"     "America/Blanc-Sablon" 
#>  [7] "America/Montreal"      "America/Toronto"       "America/Nipigon"      
#> [10] "America/Thunder_Bay"   "America/Pangnirtung"   "America/Iqaluit"      
#> [13] "America/Atikokan"      "America/Rankin_Inlet"  "America/Winnipeg"     
#> [16] "America/Rainy_River"   "America/Cambridge_Bay" "America/Regina"       
#> [19] "America/Swift_Current" "America/Edmonton"      "America/Yellowknife"  
#> [22] "America/Inuvik"        "America/Dawson_Creek"  "America/Vancouver"    
#> [25] "America/Whitehorse"    "America/Dawson"       
#> 
#> [[27]]$code
#> [1] "CA"
#> 
#> [[27]]$continent
#> [1] "North America"
#> 
#> [[27]]$name
#> [1] "Canada"
#> 
#> [[27]]$capital
#> [1] "Ottawa"
#> 
#> 
#> [[28]]
#> [[28]][[1]]
#> [1] "Africa/Kinshasa"   "Africa/Lubumbashi"
#> 
#> [[28]]$code
#> [1] "CD"
#> 
#> [[28]]$continent
#> [1] "Africa"
#> 
#> [[28]]$name
#> [1] "Democratic Republic of the Congo"
#> 
#> [[28]]$capital
#> [1] "Kinshasa"
#> 
#> 
#> [[29]]
#> [[29]][[1]]
#> [1] "Africa/Brazzaville"
#> 
#> [[29]]$code
#> [1] "CG"
#> 
#> [[29]]$continent
#> [1] "Africa"
#> 
#> [[29]]$name
#> [1] "Republic of the Congo"
#> 
#> [[29]]$capital
#> [1] "Brazzaville"
#> 
#> 
#> [[30]]
#> [[30]][[1]]
#> [1] "Africa/Abidjan"
#> 
#> [[30]]$code
#> [1] "CI"
#> 
#> [[30]]$continent
#> [1] "Africa"
#> 
#> [[30]]$name
#> [1] "Côte d'Ivoire"
#> 
#> [[30]]$capital
#> [1] "Yamoussoukro"
#> 
#> 
#> [[31]]
#> [[31]][[1]]
#> [1] "America/Santiago" "Pacific/Easter"  
#> 
#> [[31]]$code
#> [1] "CL"
#> 
#> [[31]]$continent
#> [1] "South America"
#> 
#> [[31]]$name
#> [1] "Chile"
#> 
#> [[31]]$capital
#> [1] "Santiago"
#> 
#> 
#> [[32]]
#> [[32]][[1]]
#> [1] "Africa/Douala"
#> 
#> [[32]]$code
#> [1] "CM"
#> 
#> [[32]]$continent
#> [1] "Africa"
#> 
#> [[32]]$name
#> [1] "Cameroon"
#> 
#> [[32]]$capital
#> [1] "Yaoundé"
#> 
#> 
#> [[33]]
#> [[33]][[1]]
#> [1] "Asia/Shanghai"  "Asia/Harbin"    "Asia/Chongqing" "Asia/Urumqi"   
#> [5] "Asia/Kashgar"  
#> 
#> [[33]]$code
#> [1] "CN"
#> 
#> [[33]]$continent
#> [1] "Asia"
#> 
#> [[33]]$name
#> [1] "People's Republic of China"
#> 
#> [[33]]$capital
#> [1] "Beijing"
#> 
#> 
#> [[34]]
#> [[34]][[1]]
#> [1] "America/Bogota"
#> 
#> [[34]]$code
#> [1] "CO"
#> 
#> [[34]]$continent
#> [1] "South America"
#> 
#> [[34]]$name
#> [1] "Colombia"
#> 
#> [[34]]$capital
#> [1] "Bogotá"
#> 
#> 
#> [[35]]
#> [[35]][[1]]
#> [1] "America/Costa_Rica"
#> 
#> [[35]]$code
#> [1] "CR"
#> 
#> [[35]]$continent
#> [1] "North America"
#> 
#> [[35]]$name
#> [1] "Costa Rica"
#> 
#> [[35]]$capital
#> [1] "San José"
#> 
#> 
#> [[36]]
#> [[36]][[1]]
#> [1] "America/Havana"
#> 
#> [[36]]$code
#> [1] "CU"
#> 
#> [[36]]$continent
#> [1] "North America"
#> 
#> [[36]]$name
#> [1] "Cuba"
#> 
#> [[36]]$capital
#> [1] "Havana"
#> 
#> 
#> [[37]]
#> [[37]][[1]]
#> [1] "Atlantic/Cape_Verde"
#> 
#> [[37]]$code
#> [1] "CV"
#> 
#> [[37]]$continent
#> [1] "Africa"
#> 
#> [[37]]$name
#> [1] "Cape Verde"
#> 
#> [[37]]$capital
#> [1] "Praia"
#> 
#> 
#> [[38]]
#> [[38]][[1]]
#> [1] "Asia/Nicosia"
#> 
#> [[38]]$code
#> [1] "CY"
#> 
#> [[38]]$continent
#> [1] "Asia"
#> 
#> [[38]]$name
#> [1] "Cyprus"
#> 
#> [[38]]$capital
#> [1] "Nicosia"
#> 
#> 
#> [[39]]
#> [[39]][[1]]
#> [1] "Europe/Prague"
#> 
#> [[39]]$code
#> [1] "CZ"
#> 
#> [[39]]$continent
#> [1] "Europe"
#> 
#> [[39]]$name
#> [1] "Czech Republic"
#> 
#> [[39]]$capital
#> [1] "Prague"
#> 
#> 
#> [[40]]
#> [[40]][[1]]
#> [1] "Europe/Berlin"
#> 
#> [[40]]$code
#> [1] "DE"
#> 
#> [[40]]$continent
#> [1] "Europe"
#> 
#> [[40]]$name
#> [1] "Germany"
#> 
#> [[40]]$capital
#> [1] "Berlin"
#> 
#> 
#> [[41]]
#> [[41]][[1]]
#> [1] "Africa/Djibouti"
#> 
#> [[41]]$code
#> [1] "DJ"
#> 
#> [[41]]$continent
#> [1] "Africa"
#> 
#> [[41]]$name
#> [1] "Djibouti"
#> 
#> [[41]]$capital
#> [1] "Djibouti City"
#> 
#> 
#> [[42]]
#> [[42]][[1]]
#> [1] "Europe/Copenhagen"
#> 
#> [[42]]$code
#> [1] "DK"
#> 
#> [[42]]$continent
#> [1] "Europe"
#> 
#> [[42]]$name
#> [1] "Denmark"
#> 
#> [[42]]$capital
#> [1] "Copenhagen"
#> 
#> 
#> [[43]]
#> [[43]][[1]]
#> [1] "America/Dominica"
#> 
#> [[43]]$code
#> [1] "DM"
#> 
#> [[43]]$continent
#> [1] "North America"
#> 
#> [[43]]$name
#> [1] "Dominica"
#> 
#> [[43]]$capital
#> [1] "Roseau"
#> 
#> 
#> [[44]]
#> [[44]][[1]]
#> [1] "America/Santo_Domingo"
#> 
#> [[44]]$code
#> [1] "DO"
#> 
#> [[44]]$continent
#> [1] "North America"
#> 
#> [[44]]$name
#> [1] "Dominican Republic"
#> 
#> [[44]]$capital
#> [1] "Santo Domingo"
#> 
#> 
#> [[45]]
#> [[45]][[1]]
#> [1] "America/Guayaquil" "Pacific/Galapagos"
#> 
#> [[45]]$code
#> [1] "EC"
#> 
#> [[45]]$continent
#> [1] "South America"
#> 
#> [[45]]$name
#> [1] "Ecuador"
#> 
#> [[45]]$capital
#> [1] "Quito"
#> 
#> 
#> [[46]]
#> [[46]][[1]]
#> [1] "Europe/Tallinn"
#> 
#> [[46]]$code
#> [1] "EE"
#> 
#> [[46]]$continent
#> [1] "Europe"
#> 
#> [[46]]$name
#> [1] "Estonia"
#> 
#> [[46]]$capital
#> [1] "Tallinn"
#> 
#> 
#> [[47]]
#> [[47]][[1]]
#> [1] "Africa/Cairo"
#> 
#> [[47]]$code
#> [1] "EG"
#> 
#> [[47]]$continent
#> [1] "Africa"
#> 
#> [[47]]$name
#> [1] "Egypt"
#> 
#> [[47]]$capital
#> [1] "Cairo"
#> 
#> 
#> [[48]]
#> [[48]][[1]]
#> [1] "Africa/Asmera"
#> 
#> [[48]]$code
#> [1] "ER"
#> 
#> [[48]]$continent
#> [1] "Africa"
#> 
#> [[48]]$name
#> [1] "Eritrea"
#> 
#> [[48]]$capital
#> [1] "Asmara"
#> 
#> 
#> [[49]]
#> [[49]][[1]]
#> [1] "Africa/Addis_Ababa"
#> 
#> [[49]]$code
#> [1] "ET"
#> 
#> [[49]]$continent
#> [1] "Africa"
#> 
#> [[49]]$name
#> [1] "Ethiopia"
#> 
#> [[49]]$capital
#> [1] "Addis Ababa"
#> 
#> 
#> [[50]]
#> [[50]][[1]]
#> [1] "Europe/Helsinki"
#> 
#> [[50]]$code
#> [1] "FI"
#> 
#> [[50]]$continent
#> [1] "Europe"
#> 
#> [[50]]$name
#> [1] "Finland"
#> 
#> [[50]]$capital
#> [1] "Helsinki"
#> 
#> 
#> [[51]]
#> [[51]][[1]]
#> [1] "Pacific/Fiji"
#> 
#> [[51]]$code
#> [1] "FJ"
#> 
#> [[51]]$continent
#> [1] "Oceania"
#> 
#> [[51]]$name
#> [1] "Fiji"
#> 
#> [[51]]$capital
#> [1] "Suva"
#> 
#> 
#> [[52]]
#> [[52]][[1]]
#> [1] "Europe/Paris"
#> 
#> [[52]]$code
#> [1] "FR"
#> 
#> [[52]]$continent
#> [1] "Europe"
#> 
#> [[52]]$name
#> [1] "France"
#> 
#> [[52]]$capital
#> [1] "Paris"
#> 
#> 
#> [[53]]
#> [[53]][[1]]
#> [1] "Africa/Libreville"
#> 
#> [[53]]$code
#> [1] "GA"
#> 
#> [[53]]$continent
#> [1] "Africa"
#> 
#> [[53]]$name
#> [1] "Gabon"
#> 
#> [[53]]$capital
#> [1] "Libreville"
#> 
#> 
#> [[54]]
#> [[54]][[1]]
#> [1] "Asia/Tbilisi"
#> 
#> [[54]]$code
#> [1] "GE"
#> 
#> [[54]]$continent
#> [1] "Asia"
#> 
#> [[54]]$name
#> [1] "Georgia"
#> 
#> [[54]]$capital
#> [1] "Tbilisi"
#> 
#> 
#> [[55]]
#> [[55]][[1]]
#> [1] "Africa/Accra"
#> 
#> [[55]]$code
#> [1] "GH"
#> 
#> [[55]]$continent
#> [1] "Africa"
#> 
#> [[55]]$name
#> [1] "Ghana"
#> 
#> [[55]]$capital
#> [1] "Accra"
#> 
#> 
#> [[56]]
#> [[56]][[1]]
#> [1] "Africa/Banjul"
#> 
#> [[56]]$code
#> [1] "GM"
#> 
#> [[56]]$continent
#> [1] "Africa"
#> 
#> [[56]]$name
#> [1] "The Gambia"
#> 
#> [[56]]$capital
#> [1] "Banjul"
#> 
#> 
#> [[57]]
#> [[57]][[1]]
#> [1] "Africa/Conakry"
#> 
#> [[57]]$code
#> [1] "GN"
#> 
#> [[57]]$continent
#> [1] "Africa"
#> 
#> [[57]]$name
#> [1] "Guinea"
#> 
#> [[57]]$capital
#> [1] "Conakry"
#> 
#> 
#> [[58]]
#> [[58]][[1]]
#> [1] "Europe/Athens"
#> 
#> [[58]]$code
#> [1] "GR"
#> 
#> [[58]]$continent
#> [1] "Europe"
#> 
#> [[58]]$name
#> [1] "Greece"
#> 
#> [[58]]$capital
#> [1] "Athens"
#> 
#> 
#> [[59]]
#> [[59]][[1]]
#> [1] "America/Guatemala"
#> 
#> [[59]]$code
#> [1] "GT"
#> 
#> [[59]]$continent
#> [1] "North America"
#> 
#> [[59]]$name
#> [1] "Guatemala"
#> 
#> [[59]]$capital
#> [1] "Guatemala City"
#> 
#> 
#> [[60]]
#> [[60]][[1]]
#> [1] "America/Guatemala"
#> 
#> [[60]]$code
#> [1] "GT"
#> 
#> [[60]]$continent
#> [1] "North America"
#> 
#> [[60]]$name
#> [1] "Haiti"
#> 
#> [[60]]$capital
#> [1] "Port-au-Prince"
#> 
#> 
#> [[61]]
#> [[61]][[1]]
#> [1] "Africa/Bissau"
#> 
#> [[61]]$code
#> [1] "GW"
#> 
#> [[61]]$continent
#> [1] "Africa"
#> 
#> [[61]]$name
#> [1] "Guinea-Bissau"
#> 
#> [[61]]$capital
#> [1] "Bissau"
#> 
#> 
#> [[62]]
#> [[62]][[1]]
#> [1] "America/Guyana"
#> 
#> [[62]]$code
#> [1] "GY"
#> 
#> [[62]]$continent
#> [1] "South America"
#> 
#> [[62]]$name
#> [1] "Guyana"
#> 
#> [[62]]$capital
#> [1] "Georgetown"
#> 
#> 
#> [[63]]
#> [[63]][[1]]
#> [1] "America/Tegucigalpa"
#> 
#> [[63]]$code
#> [1] "HN"
#> 
#> [[63]]$continent
#> [1] "North America"
#> 
#> [[63]]$name
#> [1] "Honduras"
#> 
#> [[63]]$capital
#> [1] "Tegucigalpa"
#> 
#> 
#> [[64]]
#> [[64]][[1]]
#> [1] "Europe/Budapest"
#> 
#> [[64]]$code
#> [1] "HU"
#> 
#> [[64]]$continent
#> [1] "Europe"
#> 
#> [[64]]$name
#> [1] "Hungary"
#> 
#> [[64]]$capital
#> [1] "Budapest"
#> 
#> 
#> [[65]]
#> [[65]][[1]]
#> [1] "Asia/Jakarta"   "Asia/Pontianak" "Asia/Makassar"  "Asia/Jayapura" 
#> 
#> [[65]]$code
#> [1] "ID"
#> 
#> [[65]]$continent
#> [1] "Asia"
#> 
#> [[65]]$name
#> [1] "Indonesia"
#> 
#> [[65]]$capital
#> [1] "Jakarta"
#> 
#> 
#> [[66]]
#> [[66]][[1]]
#> [1] "Europe/Dublin"
#> 
#> [[66]]$code
#> [1] "IE"
#> 
#> [[66]]$continent
#> [1] "Europe"
#> 
#> [[66]]$name
#> [1] "Republic of Ireland"
#> 
#> [[66]]$capital
#> [1] "Dublin"
#> 
#> 
#> [[67]]
#> [[67]][[1]]
#> [1] "Asia/Jerusalem"
#> 
#> [[67]]$code
#> [1] "IL"
#> 
#> [[67]]$continent
#> [1] "Asia"
#> 
#> [[67]]$name
#> [1] "Israel"
#> 
#> [[67]]$capital
#> [1] "Jerusalem"
#> 
#> 
#> [[68]]
#> [[68]][[1]]
#> [1] "Asia/Calcutta"
#> 
#> [[68]]$code
#> [1] "IN"
#> 
#> [[68]]$continent
#> [1] "Asia"
#> 
#> [[68]]$name
#> [1] "India"
#> 
#> [[68]]$capital
#> [1] "New Delhi"
#> 
#> 
#> [[69]]
#> [[69]][[1]]
#> [1] "Asia/Baghdad"
#> 
#> [[69]]$code
#> [1] "IQ"
#> 
#> [[69]]$continent
#> [1] "Asia"
#> 
#> [[69]]$name
#> [1] "Iraq"
#> 
#> [[69]]$capital
#> [1] "Baghdad"
#> 
#> 
#> [[70]]
#> [[70]][[1]]
#> [1] "Asia/Tehran"
#> 
#> [[70]]$code
#> [1] "IR"
#> 
#> [[70]]$continent
#> [1] "Asia"
#> 
#> [[70]]$name
#> [1] "Iran"
#> 
#> [[70]]$capital
#> [1] "Tehran"
#> 
#> 
#> [[71]]
#> [[71]][[1]]
#> [1] "Atlantic/Reykjavik"
#> 
#> [[71]]$code
#> [1] "IS"
#> 
#> [[71]]$continent
#> [1] "Europe"
#> 
#> [[71]]$name
#> [1] "Iceland"
#> 
#> [[71]]$capital
#> [1] "Reykjavík"
#> 
#> 
#> [[72]]
#> [[72]][[1]]
#> [1] "Europe/Rome"
#> 
#> [[72]]$code
#> [1] "IT"
#> 
#> [[72]]$continent
#> [1] "Europe"
#> 
#> [[72]]$name
#> [1] "Italy"
#> 
#> [[72]]$capital
#> [1] "Rome"
#> 
#> 
#> [[73]]
#> [[73]][[1]]
#> [1] "America/Jamaica"
#> 
#> [[73]]$code
#> [1] "JM"
#> 
#> [[73]]$continent
#> [1] "North America"
#> 
#> [[73]]$name
#> [1] "Jamaica"
#> 
#> [[73]]$capital
#> [1] "Kingston"
#> 
#> 
#> [[74]]
#> [[74]][[1]]
#> [1] "Asia/Amman"
#> 
#> [[74]]$code
#> [1] "JO"
#> 
#> [[74]]$continent
#> [1] "Asia"
#> 
#> [[74]]$name
#> [1] "Jordan"
#> 
#> [[74]]$capital
#> [1] "Amman"
#> 
#> 
#> [[75]]
#> [[75]][[1]]
#> [1] "Asia/Tokyo"
#> 
#> [[75]]$code
#> [1] "JP"
#> 
#> [[75]]$continent
#> [1] "Asia"
#> 
#> [[75]]$name
#> [1] "Japan"
#> 
#> [[75]]$capital
#> [1] "Tokyo"
#> 
#> 
#> [[76]]
#> [[76]][[1]]
#> [1] "Africa/Nairobi"
#> 
#> [[76]]$code
#> [1] "KE"
#> 
#> [[76]]$continent
#> [1] "Africa"
#> 
#> [[76]]$name
#> [1] "Kenya"
#> 
#> [[76]]$capital
#> [1] "Nairobi"
#> 
#> 
#> [[77]]
#> [[77]][[1]]
#> [1] "Asia/Bishkek"
#> 
#> [[77]]$code
#> [1] "KG"
#> 
#> [[77]]$continent
#> [1] "Asia"
#> 
#> [[77]]$name
#> [1] "Kyrgyzstan"
#> 
#> [[77]]$capital
#> [1] "Bishkek"
#> 
#> 
#> [[78]]
#> [[78]][[1]]
#> [1] "Pacific/Tarawa"     "Pacific/Enderbury"  "Pacific/Kiritimati"
#> 
#> [[78]]$code
#> [1] "KI"
#> 
#> [[78]]$continent
#> [1] "Oceania"
#> 
#> [[78]]$name
#> [1] "Kiribati"
#> 
#> [[78]]$capital
#> [1] "Tarawa"
#> 
#> 
#> [[79]]
#> [[79]][[1]]
#> [1] "Asia/Pyongyang"
#> 
#> [[79]]$code
#> [1] "KP"
#> 
#> [[79]]$continent
#> [1] "Asia"
#> 
#> [[79]]$name
#> [1] "North Korea"
#> 
#> [[79]]$capital
#> [1] "Pyongyang"
#> 
#> 
#> [[80]]
#> [[80]][[1]]
#> [1] "Asia/Seoul"
#> 
#> [[80]]$code
#> [1] "KR"
#> 
#> [[80]]$continent
#> [1] "Asia"
#> 
#> [[80]]$name
#> [1] "South Korea"
#> 
#> [[80]]$capital
#> [1] "Seoul"
#> 
#> 
#> [[81]]
#> [[81]][[1]]
#> [1] "Asia/Kuwait"
#> 
#> [[81]]$code
#> [1] "KW"
#> 
#> [[81]]$continent
#> [1] "Asia"
#> 
#> [[81]]$name
#> [1] "Kuwait"
#> 
#> [[81]]$capital
#> [1] "Kuwait City"
#> 
#> 
#> [[82]]
#> [[82]][[1]]
#> [1] "Asia/Beirut"
#> 
#> [[82]]$code
#> [1] "LB"
#> 
#> [[82]]$continent
#> [1] "Asia"
#> 
#> [[82]]$name
#> [1] "Lebanon"
#> 
#> [[82]]$capital
#> [1] "Beirut"
#> 
#> 
#> [[83]]
#> [[83]][[1]]
#> [1] "Europe/Vaduz"
#> 
#> [[83]]$code
#> [1] "LI"
#> 
#> [[83]]$continent
#> [1] "Europe"
#> 
#> [[83]]$name
#> [1] "Liechtenstein"
#> 
#> [[83]]$capital
#> [1] "Vaduz"
#> 
#> 
#> [[84]]
#> [[84]][[1]]
#> [1] "Africa/Monrovia"
#> 
#> [[84]]$code
#> [1] "LR"
#> 
#> [[84]]$continent
#> [1] "Africa"
#> 
#> [[84]]$name
#> [1] "Liberia"
#> 
#> [[84]]$capital
#> [1] "Monrovia"
#> 
#> 
#> [[85]]
#> [[85]][[1]]
#> [1] "Africa/Maseru"
#> 
#> [[85]]$code
#> [1] "LS"
#> 
#> [[85]]$continent
#> [1] "Africa"
#> 
#> [[85]]$name
#> [1] "Lesotho"
#> 
#> [[85]]$capital
#> [1] "Maseru"
#> 
#> 
#> [[86]]
#> [[86]][[1]]
#> [1] "Europe/Vilnius"
#> 
#> [[86]]$code
#> [1] "LT"
#> 
#> [[86]]$continent
#> [1] "Europe"
#> 
#> [[86]]$name
#> [1] "Lithuania"
#> 
#> [[86]]$capital
#> [1] "Vilnius"
#> 
#> 
#> [[87]]
#> [[87]][[1]]
#> [1] "Europe/Luxembourg"
#> 
#> [[87]]$code
#> [1] "LU"
#> 
#> [[87]]$continent
#> [1] "Europe"
#> 
#> [[87]]$name
#> [1] "Luxembourg"
#> 
#> [[87]]$capital
#> [1] "Luxembourg City"
#> 
#> 
#> [[88]]
#> [[88]][[1]]
#> [1] "Europe/Riga"
#> 
#> [[88]]$code
#> [1] "LV"
#> 
#> [[88]]$continent
#> [1] "Europe"
#> 
#> [[88]]$name
#> [1] "Latvia"
#> 
#> [[88]]$capital
#> [1] "Riga"
#> 
#> 
#> [[89]]
#> [[89]][[1]]
#> [1] "Africa/Tripoli"
#> 
#> [[89]]$code
#> [1] "LY"
#> 
#> [[89]]$continent
#> [1] "Africa"
#> 
#> [[89]]$name
#> [1] "Libya"
#> 
#> [[89]]$capital
#> [1] "Tripoli"
#> 
#> 
#> [[90]]
#> [[90]][[1]]
#> [1] "Indian/Antananarivo"
#> 
#> [[90]]$code
#> [1] "MG"
#> 
#> [[90]]$continent
#> [1] "Africa"
#> 
#> [[90]]$name
#> [1] "Madagascar"
#> 
#> [[90]]$capital
#> [1] "Antananarivo"
#> 
#> 
#> [[91]]
#> [[91]][[1]]
#> [1] "Pacific/Majuro"    "Pacific/Kwajalein"
#> 
#> [[91]]$code
#> [1] "MH"
#> 
#> [[91]]$continent
#> [1] "Oceania"
#> 
#> [[91]]$name
#> [1] "Marshall Islands"
#> 
#> [[91]]$capital
#> [1] "Majuro"
#> 
#> 
#> [[92]]
#> [[92]][[1]]
#> [1] "Europe/Skopje"
#> 
#> [[92]]$code
#> [1] "MK"
#> 
#> [[92]]$continent
#> [1] "Europe"
#> 
#> [[92]]$name
#> [1] "Macedonia"
#> 
#> [[92]]$capital
#> [1] "Skopje"
#> 
#> 
#> [[93]]
#> [[93]][[1]]
#> [1] "Africa/Bamako"
#> 
#> [[93]]$code
#> [1] "ML"
#> 
#> [[93]]$continent
#> [1] "Africa"
#> 
#> [[93]]$name
#> [1] "Mali"
#> 
#> [[93]]$capital
#> [1] "Bamako"
#> 
#> 
#> [[94]]
#> [[94]][[1]]
#> [1] "Asia/Rangoon"
#> 
#> [[94]]$code
#> [1] "MM"
#> 
#> [[94]]$continent
#> [1] "Asia"
#> 
#> [[94]]$name
#> [1] "Myanmar"
#> 
#> [[94]]$capital
#> [1] "Naypyidaw"
#> 
#> 
#> [[95]]
#> [[95]][[1]]
#> [1] "Asia/Ulaanbaatar" "Asia/Hovd"        "Asia/Choibalsan" 
#> 
#> [[95]]$code
#> [1] "MN"
#> 
#> [[95]]$continent
#> [1] "Asia"
#> 
#> [[95]]$name
#> [1] "Mongolia"
#> 
#> [[95]]$capital
#> [1] "Ulaanbaatar"
#> 
#> 
#> [[96]]
#> [[96]][[1]]
#> [1] "Africa/Nouakchott"
#> 
#> [[96]]$code
#> [1] "MR"
#> 
#> [[96]]$continent
#> [1] "Africa"
#> 
#> [[96]]$name
#> [1] "Mauritania"
#> 
#> [[96]]$capital
#> [1] "Nouakchott"
#> 
#> 
#> [[97]]
#> [[97]][[1]]
#> [1] "Europe/Malta"
#> 
#> [[97]]$code
#> [1] "MT"
#> 
#> [[97]]$continent
#> [1] "Europe"
#> 
#> [[97]]$name
#> [1] "Malta"
#> 
#> [[97]]$capital
#> [1] "Valletta"
#> 
#> 
#> [[98]]
#> [[98]][[1]]
#> [1] "Indian/Mauritius"
#> 
#> [[98]]$code
#> [1] "MU"
#> 
#> [[98]]$continent
#> [1] "Africa"
#> 
#> [[98]]$name
#> [1] "Mauritius"
#> 
#> [[98]]$capital
#> [1] "Port Louis"
#> 
#> 
#> [[99]]
#> [[99]][[1]]
#> [1] "Indian/Maldives"
#> 
#> [[99]]$code
#> [1] "MV"
#> 
#> [[99]]$continent
#> [1] "Asia"
#> 
#> [[99]]$name
#> [1] "Maldives"
#> 
#> [[99]]$capital
#> [1] "Malé"
#> 
#> 
#> [[100]]
#> [[100]][[1]]
#> [1] "Africa/Blantyre"
#> 
#> [[100]]$code
#> [1] "MW"
#> 
#> [[100]]$continent
#> [1] "Africa"
#> 
#> [[100]]$name
#> [1] "Malawi"
#> 
#> [[100]]$capital
#> [1] "Lilongwe"
#> 
#> 
#> [[101]]
#> [[101]][[1]]
#> [1] "America/Mexico_City" "America/Cancun"      "America/Merida"     
#> [4] "America/Monterrey"   "America/Mazatlan"    "America/Chihuahua"  
#> [7] "America/Hermosillo"  "America/Tijuana"    
#> 
#> [[101]]$code
#> [1] "MX"
#> 
#> [[101]]$continent
#> [1] "North America"
#> 
#> [[101]]$name
#> [1] "Mexico"
#> 
#> [[101]]$capital
#> [1] "Mexico City"
#> 
#> 
#> [[102]]
#> [[102]][[1]]
#> [1] "Asia/Kuala_Lumpur" "Asia/Kuching"     
#> 
#> [[102]]$code
#> [1] "MY"
#> 
#> [[102]]$continent
#> [1] "Asia"
#> 
#> [[102]]$name
#> [1] "Malaysia"
#> 
#> [[102]]$capital
#> [1] "Kuala Lumpur"
#> 
#> 
#> [[103]]
#> [[103]][[1]]
#> [1] "Africa/Maputo"
#> 
#> [[103]]$code
#> [1] "MZ"
#> 
#> [[103]]$continent
#> [1] "Africa"
#> 
#> [[103]]$name
#> [1] "Mozambique"
#> 
#> [[103]]$capital
#> [1] "Maputo"
#> 
#> 
#> [[104]]
#> [[104]][[1]]
#> [1] "Africa/Windhoek"
#> 
#> [[104]]$code
#> [1] "NA"
#> 
#> [[104]]$continent
#> [1] "Africa"
#> 
#> [[104]]$name
#> [1] "Namibia"
#> 
#> [[104]]$capital
#> [1] "Windhoek"
#> 
#> 
#> [[105]]
#> [[105]][[1]]
#> [1] "Africa/Niamey"
#> 
#> [[105]]$code
#> [1] "NE"
#> 
#> [[105]]$continent
#> [1] "Africa"
#> 
#> [[105]]$name
#> [1] "Niger"
#> 
#> [[105]]$capital
#> [1] "Niamey"
#> 
#> 
#> [[106]]
#> [[106]][[1]]
#> [1] "Africa/Lagos"
#> 
#> [[106]]$code
#> [1] "NG"
#> 
#> [[106]]$continent
#> [1] "Africa"
#> 
#> [[106]]$name
#> [1] "Nigeria"
#> 
#> [[106]]$capital
#> [1] "Abuja"
#> 
#> 
#> [[107]]
#> [[107]][[1]]
#> [1] "America/Managua"
#> 
#> [[107]]$code
#> [1] "NI"
#> 
#> [[107]]$continent
#> [1] "North America"
#> 
#> [[107]]$name
#> [1] "Nicaragua"
#> 
#> [[107]]$capital
#> [1] "Managua"
#> 
#> 
#> [[108]]
#> [[108]][[1]]
#> [1] "Europe/Amsterdam"
#> 
#> [[108]]$code
#> [1] "NL"
#> 
#> [[108]]$continent
#> [1] "Europe"
#> 
#> [[108]]$name
#> [1] "Kingdom of the Netherlands"
#> 
#> [[108]]$capital
#> [1] "Amsterdam"
#> 
#> 
#> [[109]]
#> [[109]][[1]]
#> [1] "Europe/Oslo"
#> 
#> [[109]]$code
#> [1] "NO"
#> 
#> [[109]]$continent
#> [1] "Europe"
#> 
#> [[109]]$name
#> [1] "Norway"
#> 
#> [[109]]$capital
#> [1] "Oslo"
#> 
#> 
#> [[110]]
#> [[110]][[1]]
#> [1] "Asia/Katmandu"
#> 
#> [[110]]$code
#> [1] "NP"
#> 
#> [[110]]$continent
#> [1] "Asia"
#> 
#> [[110]]$name
#> [1] "Nepal"
#> 
#> [[110]]$capital
#> [1] "Kathmandu"
#> 
#> 
#> [[111]]
#> [[111]][[1]]
#> [1] "Pacific/Nauru"
#> 
#> [[111]]$code
#> [1] "NR"
#> 
#> [[111]]$continent
#> [1] "Oceania"
#> 
#> [[111]]$name
#> [1] "Nauru"
#> 
#> [[111]]$capital
#> [1] "Yaren"
#> 
#> 
#> [[112]]
#> [[112]][[1]]
#> [1] "Pacific/Auckland" "Pacific/Chatham" 
#> 
#> [[112]]$code
#> [1] "NZ"
#> 
#> [[112]]$continent
#> [1] "Oceania"
#> 
#> [[112]]$name
#> [1] "New Zealand"
#> 
#> [[112]]$capital
#> [1] "Wellington"
#> 
#> 
#> [[113]]
#> [[113]][[1]]
#> [1] "Asia/Muscat"
#> 
#> [[113]]$code
#> [1] "OM"
#> 
#> [[113]]$continent
#> [1] "Asia"
#> 
#> [[113]]$name
#> [1] "Oman"
#> 
#> [[113]]$capital
#> [1] "Muscat"
#> 
#> 
#> [[114]]
#> [[114]][[1]]
#> [1] "America/Panama"
#> 
#> [[114]]$code
#> [1] "PA"
#> 
#> [[114]]$continent
#> [1] "North America"
#> 
#> [[114]]$name
#> [1] "Panama"
#> 
#> [[114]]$capital
#> [1] "Panama City"
#> 
#> 
#> [[115]]
#> [[115]][[1]]
#> [1] "America/Lima"
#> 
#> [[115]]$code
#> [1] "PE"
#> 
#> [[115]]$continent
#> [1] "South America"
#> 
#> [[115]]$name
#> [1] "Peru"
#> 
#> [[115]]$capital
#> [1] "Lima"
#> 
#> 
#> [[116]]
#> [[116]][[1]]
#> [1] "Pacific/Port_Moresby"
#> 
#> [[116]]$code
#> [1] "PG"
#> 
#> [[116]]$continent
#> [1] "Oceania"
#> 
#> [[116]]$name
#> [1] "Papua New Guinea"
#> 
#> [[116]]$capital
#> [1] "Port Moresby"
#> 
#> 
#> [[117]]
#> [[117]][[1]]
#> [1] "Asia/Manila"
#> 
#> [[117]]$code
#> [1] "PH"
#> 
#> [[117]]$continent
#> [1] "Asia"
#> 
#> [[117]]$name
#> [1] "Philippines"
#> 
#> [[117]]$capital
#> [1] "Manila"
#> 
#> 
#> [[118]]
#> [[118]][[1]]
#> [1] "Asia/Karachi"
#> 
#> [[118]]$code
#> [1] "PK"
#> 
#> [[118]]$continent
#> [1] "Asia"
#> 
#> [[118]]$name
#> [1] "Pakistan"
#> 
#> [[118]]$capital
#> [1] "Islamabad"
#> 
#> 
#> [[119]]
#> [[119]][[1]]
#> [1] "Europe/Warsaw"
#> 
#> [[119]]$code
#> [1] "PL"
#> 
#> [[119]]$continent
#> [1] "Europe"
#> 
#> [[119]]$name
#> [1] "Poland"
#> 
#> [[119]]$capital
#> [1] "Warsaw"
#> 
#> 
#> [[120]]
#> [[120]][[1]]
#> [1] "Europe/Lisbon"    "Atlantic/Madeira" "Atlantic/Azores" 
#> 
#> [[120]]$code
#> [1] "PT"
#> 
#> [[120]]$continent
#> [1] "Europe"
#> 
#> [[120]]$name
#> [1] "Portugal"
#> 
#> [[120]]$capital
#> [1] "Lisbon"
#> 
#> 
#> [[121]]
#> [[121]][[1]]
#> [1] "Pacific/Palau"
#> 
#> [[121]]$code
#> [1] "PW"
#> 
#> [[121]]$continent
#> [1] "Oceania"
#> 
#> [[121]]$name
#> [1] "Palau"
#> 
#> [[121]]$capital
#> [1] "Ngerulmud"
#> 
#> 
#> [[122]]
#> [[122]][[1]]
#> [1] "America/Asuncion"
#> 
#> [[122]]$code
#> [1] "PY"
#> 
#> [[122]]$continent
#> [1] "South America"
#> 
#> [[122]]$name
#> [1] "Paraguay"
#> 
#> [[122]]$capital
#> [1] "Asunción"
#> 
#> 
#> [[123]]
#> [[123]][[1]]
#> [1] "Asia/Qatar"
#> 
#> [[123]]$code
#> [1] "QA"
#> 
#> [[123]]$continent
#> [1] "Asia"
#> 
#> [[123]]$name
#> [1] "Qatar"
#> 
#> [[123]]$capital
#> [1] "Doha"
#> 
#> 
#> [[124]]
#> [[124]][[1]]
#> [1] "Europe/Bucharest"
#> 
#> [[124]]$code
#> [1] "RO"
#> 
#> [[124]]$continent
#> [1] "Europe"
#> 
#> [[124]]$name
#> [1] "Romania"
#> 
#> [[124]]$capital
#> [1] "Bucharest"
#> 
#> 
#> [[125]]
#> [[125]][[1]]
#>  [1] "Europe/Kaliningrad" "Europe/Moscow"      "Europe/Volgograd"  
#>  [4] "Europe/Samara"      "Asia/Yekaterinburg" "Asia/Omsk"         
#>  [7] "Asia/Novosibirsk"   "Asia/Krasnoyarsk"   "Asia/Irkutsk"      
#> [10] "Asia/Yakutsk"       "Asia/Vladivostok"   "Asia/Sakhalin"     
#> [13] "Asia/Magadan"       "Asia/Kamchatka"     "Asia/Anadyr"       
#> 
#> [[125]]$code
#> [1] "RU"
#> 
#> [[125]]$continent
#> [1] "Europe"
#> 
#> [[125]]$name
#> [1] "Russia"
#> 
#> [[125]]$capital
#> [1] "Moscow"
#> 
#> 
#> [[126]]
#> [[126]][[1]]
#> [1] "Africa/Kigali"
#> 
#> [[126]]$code
#> [1] "RW"
#> 
#> [[126]]$continent
#> [1] "Africa"
#> 
#> [[126]]$name
#> [1] "Rwanda"
#> 
#> [[126]]$capital
#> [1] "Kigali"
#> 
#> 
#> [[127]]
#> [[127]][[1]]
#> [1] "Asia/Riyadh"
#> 
#> [[127]]$code
#> [1] "SA"
#> 
#> [[127]]$continent
#> [1] "Asia"
#> 
#> [[127]]$name
#> [1] "Saudi Arabia"
#> 
#> [[127]]$capital
#> [1] "Riyadh"
#> 
#> 
#> [[128]]
#> [[128]][[1]]
#> [1] "Pacific/Guadalcanal"
#> 
#> [[128]]$code
#> [1] "SB"
#> 
#> [[128]]$continent
#> [1] "Oceania"
#> 
#> [[128]]$name
#> [1] "Solomon Islands"
#> 
#> [[128]]$capital
#> [1] "Honiara"
#> 
#> 
#> [[129]]
#> [[129]][[1]]
#> [1] "Indian/Mahe"
#> 
#> [[129]]$code
#> [1] "SC"
#> 
#> [[129]]$continent
#> [1] "Africa"
#> 
#> [[129]]$name
#> [1] "Seychelles"
#> 
#> [[129]]$capital
#> [1] "Victoria"
#> 
#> 
#> [[130]]
#> [[130]][[1]]
#> [1] "Africa/Khartoum"
#> 
#> [[130]]$code
#> [1] "SD"
#> 
#> [[130]]$continent
#> [1] "Africa"
#> 
#> [[130]]$name
#> [1] "Sudan"
#> 
#> [[130]]$capital
#> [1] "Khartoum"
#> 
#> 
#> [[131]]
#> [[131]][[1]]
#> [1] "Europe/Stockholm"
#> 
#> [[131]]$code
#> [1] "SE"
#> 
#> [[131]]$continent
#> [1] "Europe"
#> 
#> [[131]]$name
#> [1] "Sweden"
#> 
#> [[131]]$capital
#> [1] "Stockholm"
#> 
#> 
#> [[132]]
#> [[132]][[1]]
#> [1] "Asia/Singapore"
#> 
#> [[132]]$code
#> [1] "SG"
#> 
#> [[132]]$continent
#> [1] "Asia"
#> 
#> [[132]]$name
#> [1] "Singapore"
#> 
#> [[132]]$capital
#> [1] "Singapore"
#> 
#> 
#> [[133]]
#> [[133]][[1]]
#> [1] "Europe/Ljubljana"
#> 
#> [[133]]$code
#> [1] "SI"
#> 
#> [[133]]$continent
#> [1] "Europe"
#> 
#> [[133]]$name
#> [1] "Slovenia"
#> 
#> [[133]]$capital
#> [1] "Ljubljana"
#> 
#> 
#> [[134]]
#> [[134]][[1]]
#> [1] "Europe/Bratislava"
#> 
#> [[134]]$code
#> [1] "SK"
#> 
#> [[134]]$continent
#> [1] "Europe"
#> 
#> [[134]]$name
#> [1] "Slovakia"
#> 
#> [[134]]$capital
#> [1] "Bratislava"
#> 
#> 
#> [[135]]
#> [[135]][[1]]
#> [1] "Africa/Freetown"
#> 
#> [[135]]$code
#> [1] "SL"
#> 
#> [[135]]$continent
#> [1] "Africa"
#> 
#> [[135]]$name
#> [1] "Sierra Leone"
#> 
#> [[135]]$capital
#> [1] "Freetown"
#> 
#> 
#> [[136]]
#> [[136]][[1]]
#> [1] "Europe/San_Marino"
#> 
#> [[136]]$code
#> [1] "SM"
#> 
#> [[136]]$continent
#> [1] "Europe"
#> 
#> [[136]]$name
#> [1] "San Marino"
#> 
#> [[136]]$capital
#> [1] "San Marino"
#> 
#> 
#> [[137]]
#> [[137]][[1]]
#> [1] "Africa/Dakar"
#> 
#> [[137]]$code
#> [1] "SN"
#> 
#> [[137]]$continent
#> [1] "Africa"
#> 
#> [[137]]$name
#> [1] "Senegal"
#> 
#> [[137]]$capital
#> [1] "Dakar"
#> 
#> 
#> [[138]]
#> [[138]][[1]]
#> [1] "Africa/Mogadishu"
#> 
#> [[138]]$code
#> [1] "SO"
#> 
#> [[138]]$continent
#> [1] "Africa"
#> 
#> [[138]]$name
#> [1] "Somalia"
#> 
#> [[138]]$capital
#> [1] "Mogadishu"
#> 
#> 
#> [[139]]
#> [[139]][[1]]
#> [1] "America/Paramaribo"
#> 
#> [[139]]$code
#> [1] "SR"
#> 
#> [[139]]$continent
#> [1] "South America"
#> 
#> [[139]]$name
#> [1] "Suriname"
#> 
#> [[139]]$capital
#> [1] "Paramaribo"
#> 
#> 
#> [[140]]
#> [[140]][[1]]
#> [1] "Africa/Sao_Tome"
#> 
#> [[140]]$code
#> [1] "ST"
#> 
#> [[140]]$continent
#> [1] "Africa"
#> 
#> [[140]]$name
#> [1] "São Tomé and Príncipe"
#> 
#> [[140]]$capital
#> [1] "São Tomé"
#> 
#> 
#> [[141]]
#> [[141]][[1]]
#> [1] "Asia/Damascus"
#> 
#> [[141]]$code
#> [1] "SY"
#> 
#> [[141]]$continent
#> [1] "Asia"
#> 
#> [[141]]$name
#> [1] "Syria"
#> 
#> [[141]]$capital
#> [1] "Damascus"
#> 
#> 
#> [[142]]
#> [[142]][[1]]
#> [1] "Africa/Lome"
#> 
#> [[142]]$code
#> [1] "TG"
#> 
#> [[142]]$continent
#> [1] "Africa"
#> 
#> [[142]]$name
#> [1] "Togo"
#> 
#> [[142]]$capital
#> [1] "Lomé"
#> 
#> 
#> [[143]]
#> [[143]][[1]]
#> [1] "Asia/Bangkok"
#> 
#> [[143]]$code
#> [1] "TH"
#> 
#> [[143]]$continent
#> [1] "Asia"
#> 
#> [[143]]$name
#> [1] "Thailand"
#> 
#> [[143]]$capital
#> [1] "Bangkok"
#> 
#> 
#> [[144]]
#> [[144]][[1]]
#> [1] "Asia/Dushanbe"
#> 
#> [[144]]$code
#> [1] "TJ"
#> 
#> [[144]]$continent
#> [1] "Asia"
#> 
#> [[144]]$name
#> [1] "Tajikistan"
#> 
#> [[144]]$capital
#> [1] "Dushanbe"
#> 
#> 
#> [[145]]
#> [[145]][[1]]
#> [1] "Asia/Ashgabat"
#> 
#> [[145]]$code
#> [1] "TM"
#> 
#> [[145]]$continent
#> [1] "Asia"
#> 
#> [[145]]$name
#> [1] "Turkmenistan"
#> 
#> [[145]]$capital
#> [1] "Ashgabat"
#> 
#> 
#> [[146]]
#> [[146]][[1]]
#> [1] "Africa/Tunis"
#> 
#> [[146]]$code
#> [1] "TN"
#> 
#> [[146]]$continent
#> [1] "Africa"
#> 
#> [[146]]$name
#> [1] "Tunisia"
#> 
#> [[146]]$capital
#> [1] "Tunis"
#> 
#> 
#> [[147]]
#> [[147]][[1]]
#> [1] "Pacific/Tongatapu"
#> 
#> [[147]]$code
#> [1] "TO"
#> 
#> [[147]]$continent
#> [1] "Oceania"
#> 
#> [[147]]$name
#> [1] "Tonga"
#> 
#> [[147]]$capital
#> [1] "Nukuʻalofa"
#> 
#> 
#> [[148]]
#> [[148]][[1]]
#> [1] "Europe/Istanbul"
#> 
#> [[148]]$code
#> [1] "TR"
#> 
#> [[148]]$continent
#> [1] "Asia"
#> 
#> [[148]]$name
#> [1] "Turkey"
#> 
#> [[148]]$capital
#> [1] "Ankara"
#> 
#> 
#> [[149]]
#> [[149]][[1]]
#> [1] "America/Port_of_Spain"
#> 
#> [[149]]$code
#> [1] "TT"
#> 
#> [[149]]$continent
#> [1] "North America"
#> 
#> [[149]]$name
#> [1] "Trinidad and Tobago"
#> 
#> [[149]]$capital
#> [1] "Port of Spain"
#> 
#> 
#> [[150]]
#> [[150]][[1]]
#> [1] "Pacific/Funafuti"
#> 
#> [[150]]$code
#> [1] "TV"
#> 
#> [[150]]$continent
#> [1] "Oceania"
#> 
#> [[150]]$name
#> [1] "Tuvalu"
#> 
#> [[150]]$capital
#> [1] "Funafuti"
#> 
#> 
#> [[151]]
#> [[151]][[1]]
#> [1] "Africa/Dar_es_Salaam"
#> 
#> [[151]]$code
#> [1] "TZ"
#> 
#> [[151]]$continent
#> [1] "Africa"
#> 
#> [[151]]$name
#> [1] "Tanzania"
#> 
#> [[151]]$capital
#> [1] "Dodoma"
#> 
#> 
#> [[152]]
#> [[152]][[1]]
#> [1] "Europe/Kiev"       "Europe/Uzhgorod"   "Europe/Zaporozhye"
#> [4] "Europe/Simferopol"
#> 
#> [[152]]$code
#> [1] "UA"
#> 
#> [[152]]$continent
#> [1] "Europe"
#> 
#> [[152]]$name
#> [1] "Ukraine"
#> 
#> [[152]]$capital
#> [1] "Kiev"
#> 
#> 
#> [[153]]
#> [[153]][[1]]
#> [1] "Africa/Kampala"
#> 
#> [[153]]$code
#> [1] "UG"
#> 
#> [[153]]$continent
#> [1] "Africa"
#> 
#> [[153]]$name
#> [1] "Uganda"
#> 
#> [[153]]$capital
#> [1] "Kampala"
#> 
#> 
#> [[154]]
#> [[154]][[1]]
#>  [1] "America/New_York"               "America/Detroit"               
#>  [3] "America/Kentucky/Louisville"    "America/Kentucky/Monticello"   
#>  [5] "America/Indiana/Indianapolis"   "America/Indiana/Marengo"       
#>  [7] "America/Indiana/Knox"           "America/Indiana/Vevay"         
#>  [9] "America/Chicago"                "America/Indiana/Vincennes"     
#> [11] "America/Indiana/Petersburg"     "America/Menominee"             
#> [13] "America/North_Dakota/Center"    "America/North_Dakota/New_Salem"
#> [15] "America/Denver"                 "America/Boise"                 
#> [17] "America/Shiprock"               "America/Phoenix"               
#> [19] "America/Los_Angeles"            "America/Anchorage"             
#> [21] "America/Juneau"                 "America/Yakutat"               
#> [23] "America/Nome"                   "America/Adak"                  
#> [25] "Pacific/Honolulu"              
#> 
#> [[154]]$code
#> [1] "US"
#> 
#> [[154]]$continent
#> [1] "North America"
#> 
#> [[154]]$name
#> [1] "United States"
#> 
#> [[154]]$capital
#> [1] "Washington, D.C."
#> 
#> 
#> [[155]]
#> [[155]][[1]]
#> [1] "America/Montevideo"
#> 
#> [[155]]$code
#> [1] "UY"
#> 
#> [[155]]$continent
#> [1] "South America"
#> 
#> [[155]]$name
#> [1] "Uruguay"
#> 
#> [[155]]$capital
#> [1] "Montevideo"
#> 
#> 
#> [[156]]
#> [[156]][[1]]
#> [1] "Asia/Samarkand" "Asia/Tashkent" 
#> 
#> [[156]]$code
#> [1] "UZ"
#> 
#> [[156]]$continent
#> [1] "Asia"
#> 
#> [[156]]$name
#> [1] "Uzbekistan"
#> 
#> [[156]]$capital
#> [1] "Tashkent"
#> 
#> 
#> [[157]]
#> [[157]][[1]]
#> [1] "Europe/Vatican"
#> 
#> [[157]]$code
#> [1] "VA"
#> 
#> [[157]]$continent
#> [1] "Europe"
#> 
#> [[157]]$name
#> [1] "Vatican City"
#> 
#> [[157]]$capital
#> [1] "Vatican City"
#> 
#> 
#> [[158]]
#> [[158]][[1]]
#> [1] "America/Caracas"
#> 
#> [[158]]$code
#> [1] "VE"
#> 
#> [[158]]$continent
#> [1] "South America"
#> 
#> [[158]]$name
#> [1] "Venezuela"
#> 
#> [[158]]$capital
#> [1] "Caracas"
#> 
#> 
#> [[159]]
#> [[159]][[1]]
#> [1] "Asia/Saigon"
#> 
#> [[159]]$code
#> [1] "VN"
#> 
#> [[159]]$continent
#> [1] "Asia"
#> 
#> [[159]]$name
#> [1] "Vietnam"
#> 
#> [[159]]$capital
#> [1] "Hanoi"
#> 
#> 
#> [[160]]
#> [[160]][[1]]
#> [1] "Pacific/Efate"
#> 
#> [[160]]$code
#> [1] "VU"
#> 
#> [[160]]$continent
#> [1] "Oceania"
#> 
#> [[160]]$name
#> [1] "Vanuatu"
#> 
#> [[160]]$capital
#> [1] "Port Vila"
#> 
#> 
#> [[161]]
#> [[161]][[1]]
#> [1] "Asia/Aden"
#> 
#> [[161]]$code
#> [1] "YE"
#> 
#> [[161]]$continent
#> [1] "Asia"
#> 
#> [[161]]$name
#> [1] "Yemen"
#> 
#> [[161]]$capital
#> [1] "Sana'a"
#> 
#> 
#> [[162]]
#> [[162]][[1]]
#> [1] "Africa/Lusaka"
#> 
#> [[162]]$code
#> [1] "ZM"
#> 
#> [[162]]$continent
#> [1] "Africa"
#> 
#> [[162]]$name
#> [1] "Zambia"
#> 
#> [[162]]$capital
#> [1] "Lusaka"
#> 
#> 
#> [[163]]
#> [[163]][[1]]
#> [1] "Africa/Harare"
#> 
#> [[163]]$code
#> [1] "ZW"
#> 
#> [[163]]$continent
#> [1] "Africa"
#> 
#> [[163]]$name
#> [1] "Zimbabwe"
#> 
#> [[163]]$capital
#> [1] "Harare"
#> 
#> 
#> [[164]]
#> [[164]][[1]]
#> [1] "Africa/Algiers"
#> 
#> [[164]]$code
#> [1] "DZ"
#> 
#> [[164]]$continent
#> [1] "Africa"
#> 
#> [[164]]$name
#> [1] "Algeria"
#> 
#> [[164]]$capital
#> [1] "Algiers"
#> 
#> 
#> [[165]]
#> [[165]][[1]]
#> [1] "Europe/Sarajevo"
#> 
#> [[165]]$code
#> [1] "BA"
#> 
#> [[165]]$continent
#> [1] "Europe"
#> 
#> [[165]]$name
#> [1] "Bosnia and Herzegovina"
#> 
#> [[165]]$capital
#> [1] "Sarajevo"
#> 
#> 
#> [[166]]
#> [[166]][[1]]
#> [1] "Asia/Phnom_Penh"
#> 
#> [[166]]$code
#> [1] "KH"
#> 
#> [[166]]$continent
#> [1] "Asia"
#> 
#> [[166]]$name
#> [1] "Cambodia"
#> 
#> [[166]]$capital
#> [1] "Phnom Penh"
#> 
#> 
#> [[167]]
#> [[167]][[1]]
#> [1] "Africa/Bangui"
#> 
#> [[167]]$code
#> [1] "CF"
#> 
#> [[167]]$continent
#> [1] "Africa"
#> 
#> [[167]]$name
#> [1] "Central African Republic"
#> 
#> [[167]]$capital
#> [1] "Bangui"
#> 
#> 
#> [[168]]
#> [[168]][[1]]
#> [1] "Africa/Ndjamena"
#> 
#> [[168]]$code
#> [1] "TD"
#> 
#> [[168]]$continent
#> [1] "Africa"
#> 
#> [[168]]$name
#> [1] "Chad"
#> 
#> [[168]]$capital
#> [1] "N'Djamena"
#> 
#> 
#> [[169]]
#> [[169]][[1]]
#> [1] "Indian/Comoro"
#> 
#> [[169]]$code
#> [1] "KM"
#> 
#> [[169]]$continent
#> [1] "Africa"
#> 
#> [[169]]$name
#> [1] "Comoros"
#> 
#> [[169]]$capital
#> [1] "Moroni"
#> 
#> 
#> [[170]]
#> [[170]][[1]]
#> [1] "Europe/Zagreb"
#> 
#> [[170]]$code
#> [1] "HR"
#> 
#> [[170]]$continent
#> [1] "Europe"
#> 
#> [[170]]$name
#> [1] "Croatia"
#> 
#> [[170]]$capital
#> [1] "Zagreb"
#> 
#> 
#> [[171]]
#> [[171]][[1]]
#> [1] "Asia/Dili"
#> 
#> [[171]]$code
#> [1] "TL"
#> 
#> [[171]]$continent
#> [1] "Asia"
#> 
#> [[171]]$name
#> [1] "East Timor"
#> 
#> [[171]]$capital
#> [1] "Dili"
#> 
#> 
#> [[172]]
#> [[172]][[1]]
#> [1] "America/El_Salvador"
#> 
#> [[172]]$code
#> [1] "SV"
#> 
#> [[172]]$continent
#> [1] "North America"
#> 
#> [[172]]$name
#> [1] "El Salvador"
#> 
#> [[172]]$capital
#> [1] "San Salvador"
#> 
#> 
#> [[173]]
#> [[173]][[1]]
#> [1] "Africa/Malabo"
#> 
#> [[173]]$code
#> [1] "GQ"
#> 
#> [[173]]$continent
#> [1] "Africa"
#> 
#> [[173]]$name
#> [1] "Equatorial Guinea"
#> 
#> [[173]]$capital
#> [1] "Malabo"
#> 
#> 
#> [[174]]
#> [[174]][[1]]
#> [1] "America/Grenada"
#> 
#> [[174]]$code
#> [1] "GD"
#> 
#> [[174]]$continent
#> [1] "North America"
#> 
#> [[174]]$name
#> [1] "Grenada"
#> 
#> [[174]]$capital
#> [1] "St. George's"
#> 
#> 
#> [[175]]
#> [[175]][[1]]
#> [1] "Asia/Almaty"    "Asia/Qyzylorda" "Asia/Aqtobe"    "Asia/Aqtau"    
#> [5] "Asia/Oral"     
#> 
#> [[175]]$code
#> [1] "KZ"
#> 
#> [[175]]$continent
#> [1] "Asia"
#> 
#> [[175]]$name
#> [1] "Kazakhstan"
#> 
#> [[175]]$capital
#> [1] "Astana"
#> 
#> 
#> [[176]]
#> [[176]][[1]]
#> [1] "Asia/Vientiane"
#> 
#> [[176]]$code
#> [1] "LA"
#> 
#> [[176]]$continent
#> [1] "Asia"
#> 
#> [[176]]$name
#> [1] "Laos"
#> 
#> [[176]]$capital
#> [1] "Vientiane"
#> 
#> 
#> [[177]]
#> [[177]][[1]]
#> [1] "Pacific/Truk"   "Pacific/Ponape" "Pacific/Kosrae"
#> 
#> [[177]]$code
#> [1] "FM"
#> 
#> [[177]]$continent
#> [1] "Oceania"
#> 
#> [[177]]$name
#> [1] "Federated States of Micronesia"
#> 
#> [[177]]$capital
#> [1] "Palikir"
#> 
#> 
#> [[178]]
#> [[178]][[1]]
#> [1] "Europe/Chisinau"
#> 
#> [[178]]$code
#> [1] "MD"
#> 
#> [[178]]$continent
#> [1] "Europe"
#> 
#> [[178]]$name
#> [1] "Moldova"
#> 
#> [[178]]$capital
#> [1] "Chişinău"
#> 
#> 
#> [[179]]
#> [[179]][[1]]
#> [1] "Europe/Monaco"
#> 
#> [[179]]$code
#> [1] "MC"
#> 
#> [[179]]$continent
#> [1] "Europe"
#> 
#> [[179]]$name
#> [1] "Monaco"
#> 
#> [[179]]$capital
#> [1] "Monaco"
#> 
#> 
#> [[180]]
#> [[180]][[1]]
#> [1] "Europe/Podgorica"
#> 
#> [[180]]$code
#> [1] "ME"
#> 
#> [[180]]$continent
#> [1] "Europe"
#> 
#> [[180]]$name
#> [1] "Montenegro"
#> 
#> [[180]]$capital
#> [1] "Podgorica"
#> 
#> 
#> [[181]]
#> [[181]][[1]]
#> [1] "Africa/Casablanca"
#> 
#> [[181]]$code
#> [1] "MA"
#> 
#> [[181]]$continent
#> [1] "Africa"
#> 
#> [[181]]$name
#> [1] "Morocco"
#> 
#> [[181]]$capital
#> [1] "Rabat"
#> 
#> 
#> [[182]]
#> [[182]][[1]]
#> [1] "America/St_Kitts"
#> 
#> [[182]]$code
#> [1] "KN"
#> 
#> [[182]]$continent
#> [1] "North America"
#> 
#> [[182]]$name
#> [1] "Saint Kitts and Nevis"
#> 
#> [[182]]$capital
#> [1] "Basseterre"
#> 
#> 
#> [[183]]
#> [[183]][[1]]
#> [1] "America/St_Lucia"
#> 
#> [[183]]$code
#> [1] "LC"
#> 
#> [[183]]$continent
#> [1] "North America"
#> 
#> [[183]]$name
#> [1] "Saint Lucia"
#> 
#> [[183]]$capital
#> [1] "Castries"
#> 
#> 
#> [[184]]
#> [[184]][[1]]
#> [1] "America/St_Vincent"
#> 
#> [[184]]$code
#> [1] "VC"
#> 
#> [[184]]$continent
#> [1] "North America"
#> 
#> [[184]]$name
#> [1] "Saint Vincent and the Grenadines"
#> 
#> [[184]]$capital
#> [1] "Kingstown"
#> 
#> 
#> [[185]]
#> [[185]][[1]]
#> [1] "Pacific/Apia"
#> 
#> [[185]]$code
#> [1] "WS"
#> 
#> [[185]]$continent
#> [1] "Oceania"
#> 
#> [[185]]$name
#> [1] "Samoa"
#> 
#> [[185]]$capital
#> [1] "Apia"
#> 
#> 
#> [[186]]
#> [[186]][[1]]
#> [1] "Europe/Belgrade"
#> 
#> [[186]]$code
#> [1] "RS"
#> 
#> [[186]]$continent
#> [1] "Europe"
#> 
#> [[186]]$name
#> [1] "Serbia"
#> 
#> [[186]]$capital
#> [1] "Belgrade"
#> 
#> 
#> [[187]]
#> [[187]][[1]]
#> [1] "Africa/Johannesburg"
#> 
#> [[187]]$code
#> [1] "ZA"
#> 
#> [[187]]$continent
#> [1] "Africa"
#> 
#> [[187]]$name
#> [1] "South Africa"
#> 
#> [[187]]$capital
#> [1] "Pretoria"
#> 
#> 
#> [[188]]
#> [[188]][[1]]
#> [1] "Europe/Madrid"   "Africa/Ceuta"    "Atlantic/Canary"
#> 
#> [[188]]$code
#> [1] "ES"
#> 
#> [[188]]$continent
#> [1] "Europe"
#> 
#> [[188]]$name
#> [1] "Spain"
#> 
#> [[188]]$capital
#> [1] "Madrid"
#> 
#> 
#> [[189]]
#> [[189]][[1]]
#> [1] "Asia/Colombo"
#> 
#> [[189]]$code
#> [1] "LK"
#> 
#> [[189]]$continent
#> [1] "Asia"
#> 
#> [[189]]$name
#> [1] "Sri Lanka"
#> 
#> [[189]]$capital
#> [1] "Sri Jayewardenepura Kotte"
#> 
#> 
#> [[190]]
#> [[190]][[1]]
#> [1] "Africa/Mbabane"
#> 
#> [[190]]$code
#> [1] "SZ"
#> 
#> [[190]]$continent
#> [1] "Africa"
#> 
#> [[190]]$name
#> [1] "Swaziland"
#> 
#> [[190]]$capital
#> [1] "Mbabane"
#> 
#> 
#> [[191]]
#> [[191]][[1]]
#> [1] "Europe/Zurich"
#> 
#> [[191]]$code
#> [1] "CH"
#> 
#> [[191]]$continent
#> [1] "Europe"
#> 
#> [[191]]$name
#> [1] "Switzerland"
#> 
#> [[191]]$capital
#> [1] "Bern"
#> 
#> 
#> [[192]]
#> [[192]][[1]]
#> [1] "Asia/Dubai"
#> 
#> [[192]]$code
#> [1] "AE"
#> 
#> [[192]]$continent
#> [1] "Asia"
#> 
#> [[192]]$name
#> [1] "United Arab Emirates"
#> 
#> [[192]]$capital
#> [1] "Abu Dhabi"
#> 
#> 
#> [[193]]
#> [[193]][[1]]
#> [1] "Europe/London"
#> 
#> [[193]]$code
#> [1] "GB"
#> 
#> [[193]]$continent
#> [1] "Europe"
#> 
#> [[193]]$name
#> [1] "United Kingdom"
#> 
#> [[193]]$capital
#> [1] "London"
#> 
#> 
z$centuries
#>  [1] "I"     "II"    "III"   "IV"    "V"     "VI"    "VII"   "VIII"  "IX"   
#> [10] "X"     "XI"    "XII"   "XIII"  "XIV"   "XV"    "XVI"   "XVII"  "XVIII"
#> [19] "XIX"   "XX"    "XXI"  
z$century()
#> [1] "XII"
z$timezone()
#> [[1]]
#> [[1]][[1]]
#> [1] "Asia/Katmandu"
#> 
#> [[1]]$code
#> [1] "NP"
#> 
#> [[1]]$continent
#> [1] "Asia"
#> 
#> [[1]]$name
#> [1] "Nepal"
#> 
#> [[1]]$capital
#> [1] "Kathmandu"
#> 
#> 
z$unix_time()
#> [1] 884047602
z$date("%Y-%M-%d")
#> [1] "2005-02-22"
z$date_time()
#> [1] "1980-08-29 11:44:12 UTC"
z$year()
#> [1] "2001"
z$iso8601("1932-02-12 05:32:12")
#> [1] "1932-02-12"
# z$iso8601("January 4, 1981")

# date time between a range of dates
(start_date <- Sys.time() - 604800L)
#> [1] "2026-08-23 07:25:03 UTC"
z$date_time_between(start_date = start_date)
#> [1] "2026-08-26 11:15:58 UTC"
# in the year 1900
z$date_time_between("1900-01-01 00:00:00 PST", "1900-12-31 00:00:00 PST")
#> [1] "1900-06-23 06:58:18 UTC"
z$date_time_between("1900-01-01", "1900-12-31")
#> [1] "1900-10-06 19:51:34 UTC"
```
