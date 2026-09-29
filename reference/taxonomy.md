# Create fake taxonomic names

Create fake taxonomic names

## Usage

``` r
ch_taxonomic_genus(n = 1, locale = "en_US")

ch_taxonomic_epithet(n = 1, locale = "en_US")

ch_taxonomic_species(n = 1, locale = "en_US")
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  Locale for provider

## Names

Names were taken from Theplantlist. 500 genera names and 500 epithets
were chosen at random from the set of 10,000 names in the dataset in the
`taxize` package. Theplantlist is, as it says on the tin, composed of
plant names - so these fake names are derived from plant names if that
matters to you. These may generate names that match those of real taxa,
but may not as well.

## Taxonomic authority

Randomly, the taxonomic authority is in parentheses - which represents
that the given authority was not the original authority.

## See also

[TaxonomyProvider](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md)

## Examples

``` r
ch_taxonomic_genus()
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> [1] "Rafflesia"
ch_taxonomic_genus(10)
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#>  [1] "Rafflesia"       "Brachystelma"    "Chrysochlamys"   "Psephellus"     
#>  [5] "Dryopolystichum" "Antiphytum"      "Plagiobryum"     "Acrostichum"    
#>  [9] "Prinos"          "Raphanus"       
# or even ch_taxonomic_genus(500)

ch_taxonomic_epithet()
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> [1] "deltoidea"
ch_taxonomic_epithet(10)
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#>  [1] "blumeana"       "rubropilosa"    "decorticans"    "bracteosum"    
#>  [5] "aurosicus"      "neapolitana"    "rhaphidostegum" "bracteosum"    
#>  [9] "nothofagicola"  "aridus"        
# or even ch_taxonomic_epithet(500)

ch_taxonomic_species()
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> [1] "Normanbya pilmaiquen"
ch_taxonomic_species(10)
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#> Warning: Global setting for messy is TRUE
#>  [1] "Stylochiton daniel-jimenezii" "Sisyrinchium brevicaudata"   
#>  [3] "Modecca styriacum"            "Crocus neapolitana"          
#>  [5] "Soleirolia incanus"           "Synnema leratii"             
#>  [7] "Eucharis cacharensis"         "Eugenia hockii"              
#>  [9] "Peltoboykinia anamensis"      "Microcos saksenanus"         
# or even ch_taxonomic_species(500)
```
