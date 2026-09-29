# Get elements

Get elements

## Usage

``` r
ch_element_symbol(n = 1)

ch_element_element(n = 1)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

## See also

[ElementProvider](https://docs.ropensci.org/charlatan/reference/ElementProvider.md)

## Examples

``` r
ch_element_symbol()
#> [1] "Cn"
ch_element_symbol(10)
#>  [1] "Ir" "Bi" "Li" "Np" "Be" "Xe" "Br" "Ne" "Al" "Kr"
ch_element_symbol(50)
#>  [1] "Th" "Re" "Ni" "C"  "Ca" "Ta" "Sg" "Sr" "Tm" "Cu" "Ce" "Tl" "Pu" "Db" "Nh"
#> [16] "Hs" "Se" "H"  "Fl" "B"  "Hs" "Nb" "Sr" "Rf" "B"  "Lu" "Cs" "Ir" "Am" "Co"
#> [31] "Sr" "Sc" "I"  "Ts" "Ts" "C"  "Mg" "Mo" "Al" "Re" "Kr" "Er" "Zr" "Cf" "Dy"
#> [46] "Si" "Hs" "As" "Os" "Rf"

ch_element_element()
#> [1] "Zinc"
ch_element_element(10)
#>  [1] "Oganesson"   "Bismuth"     "Yttrium"     "Zirconium"   "Magnesium"  
#>  [6] "Astatine"    "Arsenic"     "Livermorium" "Meitnerium"  "Cerium"     
ch_element_element(50)
#>  [1] "Darmstadtium" "Argon"        "Thulium"      "Nitrogen"     "Erbium"      
#>  [6] "Iridium"      "Oxygen"       "Roentgenium"  "Platinum"     "Tellurium"   
#> [11] "Yttrium"      "Praseodymium" "Sodium"       "Lithium"      "Carbon"      
#> [16] "Selenium"     "Neodymium"    "Einsteinium"  "Californium"  "Meitnerium"  
#> [21] "Lithium"      "Radium"       "Copernicium"  "Polonium"     "Xenon"       
#> [26] "Flerovium"    "Arsenic"      "Vanadium"     "Molybdenum"   "Sulfur"      
#> [31] "Phosphorus"   "Tantalum"     "Meitnerium"   "Cobalt"       "Xenon"       
#> [36] "Osmium"       "Argon"        "Arsenic"      "Helium"       "Antimony"    
#> [41] "Manganese"    "Antimony"     "Rubidium"     "Dubnium"      "Aluminium"   
#> [46] "Arsenic"      "Tellurium"    "Mercury"      "Helium"       "Thulium"     
```
