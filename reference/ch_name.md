# Create fake person names

Create fake person names

## Usage

``` r
ch_name(n = 1, locale = NULL, messy = FALSE)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. See
  `PersonProvider$new()$allowed_locales()` for locales supported
  (default: en_US)

- messy:

  (logical) make some messy data. Default: `FALSE`

## See also

[PersonProvider_en_US](https://docs.ropensci.org/charlatan/reference/PersonProvider_en_US.md)

## Examples

``` r
ch_name()
#> [1] "Christ Hane II"
ch_name(10)
#>  [1] "Summer Terry"        "Paige Ullrich DDS"   "Cato McLaughlin"    
#>  [4] "Alden Rowe"          "Hank Yost"           "Nanna Bayer"        
#>  [7] "Ernst Weimann"       "Simmie Ritchie"      "Jamin Runolfsdottir"
#> [10] "Mrs. Dicy Stanton"  
# or even ch_name(500)

ch_name(locale = "fr_FR", n = 10)
#>  [1] "Virginie Rogér"              "Maurice-Raymond Potier"     
#>  [3] "Christophe Guillot"          "Louise Guillot"             
#>  [5] "Gilles Blondel"              "Antoine Lacombe L'Laroche"  
#>  [7] "daisy Thomas"                "Philippine-Capucine Perrier"
#>  [9] "André Bértrand L'Bazin"      "Jacqueline Allain-Duval"    
ch_name(locale = "fr_CH", n = 10)
#>  [1] "Laetitia Chenaux"     "Jean-Claude Comment"  "Stéphane Marty"      
#>  [4] "Isabelle Paccot"      "Céline Chevrolet"     "Emma Mottet"         
#>  [7] "Louis Gubéran-Pellet" "Roger Mottet"         "Raymond Rapin"       
#> [10] "Julie Brahier"       
ch_name(locale = "fa_IR", n = 10)
#>  [1] "حسنا جلیلی"                    "محمدپارسا سمسار"              
#>  [3] "آتنا نیلوفری"                  "آريا عقیلی"                   
#>  [5] "حسين عباسی"                    "محمدمهدي رستمی"               
#>  [7] "سرکار خانم دکتر الناز علیجانی" "كیانا سغیری"                  
#>  [9] "یگانه محمدی"                   "محمدرضا موحد"                 
ch_name(locale = "fi_FI", n = 10)
#>  [1] "Osmo Eerikäinen"    "Ylätalo, Sara"      "Juho Ahtisaari"    
#>  [4] "Rautavaara, Jami"   "Hillevi Issakainen" "Eerika Nikkonen"   
#>  [7] "Sillanpää, Aleksi"  "Mirjam Mäkilä"      "Pulkkinen, Alpo"   
#> [10] "Riku Rantala"      
```
