# Introduction to the charlatan package

`charlatan` makes realistic looking fake data, inspired from and
borrowing some code from Python’s
[faker](https://github.com/joke2k/faker)

Why would you want to make fake data that looks real? Here’s some
possible use cases to give you a sense for what you can do with this
package:

- Students in a classroom setting learning any task that needs a
  dataset.
- People doing simulations/modeling that need some fake data
- Generate fake dataset of users for a database before actual users
  exist
- Complete missing spots in a dataset
- Generate fake data to replace sensitive real data with before public
  release
- Create a random set of colors for visualization
- Generate random coordinates for a map
- Get a set of randomly generated DOIs (Digital Object Identifiers) to
  assign to fake scholarly artifacts
- Generate fake taxonomic names for a biological dataset
- Get a set of fake sequences to use to test code/software that uses
  sequence data

See the [**Creating realistic
data**](https://docs.ropensci.org/charlatan/articles/creating-realistic-data.html)
vignette for a few realistic examples.

## Contributing

See the [**Contributing to
charlatan**](https://docs.ropensci.org/charlatan/articles/contributing.html)
vignette.

## Package API

- Low level interfaces: All of these are `R6` objects that a user can
  initialize and then call methods on. These contain all the logic that
  the below interfaces use.
- High level interfaces: There are high level functions prefixed with
  `ch_*()` that wrap low level interfaces, and are meant to be easier to
  use and provide an easy way to make many instances of a thing.
- [`ch_generate()`](https://docs.ropensci.org/charlatan/reference/ch_generate.md) -
  generate a data.frame with fake data, choosing which columns to
  include from the data types provided in `charlatan`
- [`fraudster()`](https://docs.ropensci.org/charlatan/reference/fraudster.md) -
  single interface to all fake data methods, - returns vectors/lists of
  data - this function wraps the `ch_*()` functions described above

## Install

Stable version from CRAN

``` r

install.packages("charlatan")
```

Development version from Github

``` r

remotes::install_github("ropensci/charlatan")
```

``` r

library("charlatan")
```

## high level function

… for all fake data operations

``` r

x <- fraudster()
x$job()
#> [1] "Dispensing optician"
x$name()
#> [1] "Loy Roob"
x$job()
#> [1] "Sports administrator"
x$color_name()
#> [1] "Azure"
```

## locale support

Here we create 3 jobs, for different locales:

- English USA
- French, France
- Croatian, Croatia
- Ukrainian, Ukraine
- Chinese, Taiwan

``` r

ch_job(locale = "en_US", n = 3)
#> [1] "Scientist, research (medical)" "Cabin crew"                   
#> [3] "Presenter, broadcasting"
ch_job(locale = "fr_FR", n = 3)
#> [1] "Restaurateur d'oeuvres d'art" "Électromécanicien"           
#> [3] "Aromaticien"
ch_job(locale = "hr_HR", n = 3)
#> [1] "Elektroničar – mehaničar"            
#> [2] "Viši restaurator"                    
#> [3] "Doktor dentalne medicine specijalist"
ch_job(locale = "uk_UA", n = 3)
#> [1] "Кінорежисер" "Акушер"      "Дантист"
ch_job(locale = "zh_TW", n = 3)
#> [1] "農藝／畜產研究人員" "人力資源人員"       "電機工程技術員"
```

For colors:

``` r

ch_color_name(locale = "en_US", n = 3)
#> [1] "LightPink"      "BlanchedAlmond" "Blue"
ch_color_name(locale = "uk_UA", n = 3)
#> [1] "Темний індиго"     "Пастельно-зелений" "Темно-брунатний"
```

## generate a dataset

``` r

ch_generate()
#> # A tibble: 10 × 3
#>    name                      job                                   phone_number 
#>    <chr>                     <chr>                                 <chr>        
#>  1 Archibald Howe IV         Solicitor                             (462)040-500…
#>  2 Dulce Hayes               Emergency planning/management officer 06671782858  
#>  3 Denver Bechtelar          Designer, blown glass/stained glass   216-331-8122…
#>  4 Ignatius Hegmann-Luettgen Producer, radio                       +26(0)569750…
#>  5 Mikalah Runte             Administrator, arts                   (235)184-2149
#>  6 Mr. Ed Morar              Physiotherapist                       327.380.6379 
#>  7 Zoey Runolfsdottir        Architect                             688.982.8206…
#>  8 Joella Wilkinson          Surveyor, rural practice              1-272-771-61…
#>  9 Reinhold Kuhic            Child psychotherapist                 918-806-3088…
#> 10 Jaimee Hackett-Littel     Recruitment consultant                +99(1)423144…
```

``` r

ch_generate("job", "phone_number", n = 30)
#> # A tibble: 30 × 2
#>    job                                 phone_number       
#>    <chr>                               <chr>              
#>  1 Development worker, community       134.633.3245x42384 
#>  2 Proofreader                         (669)547-1971      
#>  3 Restaurant manager                  (504)458-0083x17669
#>  4 Bookseller                          1-549-857-2991     
#>  5 Adult guidance worker               (663)691-8959      
#>  6 Neurosurgeon                        +18(0)0008128475   
#>  7 Chartered public finance accountant +39(2)1699145965   
#>  8 Community arts worker               03253968801        
#>  9 Scientist, research (medical)       1-909-446-6745x1440
#> 10 Illustrator                         893-592-2074x83289 
#> # ℹ 20 more rows
```

## Data types, localized

We can create locale specific versions of:

- Colors
- Companies
- Elements *(of the periodic table)*
- Files
- Internet
- Jobs
- Lorem
- Persons
- Phone numbers
- Social Security Numbers
- Taxonomies
- UserAgent

Examples:

### person name

``` r

ch_name()
#> [1] "Lempi Lueilwitz DVM"
```

``` r

ch_name(10)
#>  [1] "Mr. Elmer Pouros Jr."    "Dr. Axel Thompson"      
#>  [3] "Jazlyn Berge-Upton"      "Dr. Ozzie Bahringer Jr."
#>  [5] "Shatara Miller"          "Benjaman Upton-Bernhard"
#>  [7] "Rosendo Hoeger"          "Teddy Gusikowski"       
#>  [9] "Darlene Becker"          "Dr. Berkley McDermott"
```

### phone number

``` r

ch_phone_number()
#> [1] "00983984857"
```

``` r

ch_phone_number(10)
#>  [1] "1-750-771-0882"      "1-503-140-4937x4600" "627-255-7243x72667" 
#>  [4] "738.515.9740"        "1-102-581-5742x986"  "479-363-9505x515"   
#>  [7] "526.764.5338x38873"  "164.363.6007x29826"  "1-457-659-7114"     
#> [10] "924-138-8337"
```

### job

``` r

ch_job()
#> [1] "Herpetologist"
```

``` r

ch_job(10)
#>  [1] "Charity fundraiser"                         
#>  [2] "Estate agent"                               
#>  [3] "Child psychotherapist"                      
#>  [4] "Agricultural engineer"                      
#>  [5] "Leisure centre manager"                     
#>  [6] "Psychologist, prison and probation services"
#>  [7] "Designer, ceramics/pottery"                 
#>  [8] "Scientist, biomedical"                      
#>  [9] "Chartered management accountant"            
#> [10] "Hotel manager"
```

## Data types, universal

Some data types are not localized (arguably the files and user_agents,
are mostly universal too).

- Currency
- credit card
- Sequence (DNA)
- Numerics (doubles, integers, numbers from a distribution; uniform,
  normal, log-normal, and beta)
- Miscellaneous (booleans, language codes)
- DOIs (Digital Object Identifiers, used in scientific journals)
- Coordinates (GPS coordinates)

### currency

``` r

ch_currency(3)
#> [1] "PEN" "XPF" "STD"
```

### credit cards

``` r

ch_credit_card_provider()
#> [1] "JCB 16 digit"
ch_credit_card_provider(n = 4)
#> [1] "JCB 16 digit"  "VISA 16 digit" "VISA 13 digit" "JCB 16 digit"
```

``` r

ch_credit_card_number()
#> [1] "3528588375726996578"
ch_credit_card_number(n = 10)
#>  [1] "869923674811447486"  "3058571612909475"    "53699104395695097"  
#>  [4] "4040150643695153"    "210022871412708941"  "869974993874530667" 
#>  [7] "4273030620980737"    "52186064938976448"   "3088524399543540416"
#> [10] "4946059061636224"
```

``` r

ch_credit_card_security_code()
#> [1] "827"
ch_credit_card_security_code(10)
#>  [1] "987" "263" "940" "965" "778" "086" "768" "924" "914" "589"
```

## Missing data

`charlatan` makes it very easy to generate fake data with missing
entries. First, you need to run
[`MissingDataProvider()`](https://docs.ropensci.org/charlatan/reference/MissingDataProvider.md)
and then make an appropriate `make_missing()` call specifying the data
type to be generated. This method picks a random number (`N`) of slots
in the input `make_missing` vector and then picks `N` random positions
that will be replaced with NA matching the input class.

``` r

testVector <- MissingDataProvider$new()
```

### character strings

``` r

testVector$make_missing(x = ch_generate()$name)
#>  [1] NA                      NA                      NA                     
#>  [4] NA                      "Mrs. Lulu Kunze"       "Dr. Braulio Durgan II"
#>  [7] NA                      "Elba Cremin DVM"       "Carmel Bashirian"     
#> [10] "Christie Orn"
```

### numeric data

``` r

testVector$make_missing(x = ch_integer(10))
#>  [1]  NA  NA  NA  NA  NA 688 942 919  NA  NA
```

### logicals

``` r

set.seed(123)
testVector$make_missing(x = sample(c(TRUE, FALSE), 10, replace = TRUE))
#>  [1]  TRUE    NA    NA FALSE  TRUE    NA FALSE FALSE    NA  TRUE
```

## Messy data

Real data is messy, right? `charlatan` makes it easy to create messy
data. This is still in the early stages so is not available across most
data types and languages, but we’re working on it.

For example, create messy names:

``` r

ch_name(50, messy = TRUE)
#>  [1] "Destiney Dicki"            "Mrs. Freddie Pouros DDS"  
#>  [3] "Ms. Jada Lesch"            "Inga Dach"                
#>  [5] "Keyshawn Schaefer"         "Ferdinand Bergstrom"      
#>  [7] "Justen Simonis"            "Ms. Doloris Stroman DVM"  
#>  [9] "Mrs. Ermine Heidenreich"   "Marion Corwin"            
#> [11] "Jalen Grimes"              "Mr. Sullivan Hammes IV"   
#> [13] "Adrien Vandervort-Dickens" "Dr. Sharif Kunde"         
#> [15] "Marlena Reichert PhD"      "Mr. Brandan Oberbrunner"  
#> [17] "Lloyd Adams III"           "Randy Ziemann"            
#> [19] "Gina Sanford"              "Cornell Funk"             
#> [21] "Yadiel Collier"            "Kamryn Johnson"           
#> [23] "Tyesha Schmeler"           "Ernie Hegmann-Graham"     
#> [25] "Zackery Runolfsdottir"     "Cleveland Predovic"       
#> [27] "Melvyn Hickle"             "Larry Nienow IV"          
#> [29] "Vilma Rutherford"          "Wiliam Ziemann-Fadel"     
#> [31] "Mrs. Kathy Halvorson"      "Mirtie Harvey-Shanahan"   
#> [33] "Eliezer Pfeffer"           "Dr. Shep Buckridge"       
#> [35] "Kyree Kutch"               "Ms. Delpha Grant"         
#> [37] "Ms. Icie Crooks"           "Loney Jenkins-Lindgren"   
#> [39] "Shania Donnelly DVM"       "Dr. Patric Veum"          
#> [41] "Amirah Rippin DVM"         "Randle Hilpert"           
#> [43] "Soren Dare"                "Roderic Walter"           
#> [45] "Farah Daugherty MD"        "Marva Crooks"             
#> [47] "Ryland Ledner"             "Girtha Harvey DDS"        
#> [49] "Staci Spencer"             "Mr. Olan Bernhard"
```

Right now only suffixes and prefixes for names in `en_US` locale are
supported. Notice above some variation in prefixes and suffixes.
