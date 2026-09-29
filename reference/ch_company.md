# Create fake company names and other company bits

Create fake company names and other company bits

## Usage

``` r
ch_company(n = 1, locale = NULL)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. See `company()$allowed_locales()` for
  locales supported.

## See also

[CompanyProvider](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md)

## Examples

``` r
ch_company()
#> [1] "Krajcik Inc"
ch_company(10)
#>  [1] "Connelly, Gaylord and Thiel"   "Predovic, Gleason and Kreiger"
#>  [3] "Hilll, Pagac and Torphy"       "Schimmel Ltd"                 
#>  [5] "Kuhic-Schmeler"                "Will Ltd"                     
#>  [7] "Kuhlman, Haag and Okuneva"     "Lemke PLC"                    
#>  [9] "Koch Inc"                      "Lubowitz Ltd"                 
# or even ch_company(500)

ch_company(locale = "fr_FR", n = 10)
#>  [1] "Boucher"              "Jacques"              "Gosselin"            
#>  [4] "Riou et Fils"         "Pages SARL"           "Voisin Voisin SA"    
#>  [7] "Pires et Fils"        "Rey Rey S.A.R.L."     "Mendes"              
#> [10] "Labbe Labbe S.A.R.L."
ch_company(locale = "cs_CZ", n = 10)
#>  [1] "Procházka Urbanová a.s." "Kadlec"                 
#>  [3] "Holubová"                "Novotná"                
#>  [5] "Procházková Holub a.s."  "Kříž a.s."              
#>  [7] "Polák"                   "Bláhová Čermák o.s."    
#>  [9] "Růžičková"               "Pospíšil a.s."          
ch_company(locale = "es_MX", n = 10)
#>  [1] "Proyectos Guevara, Urbina y Pantoja" "Despacho Girón y Rocha"             
#>  [3] "Pizarro-Venegas"                     "Santana-Jaimes S.A."                
#>  [5] "Navarrete-Rodrígez S.C."             "Arevalo, Luevano y Valdivia"        
#>  [7] "Loya, Salcedo y Lebrón"              "Posada, Chavarría y Villa"          
#>  [9] "Gallardo-Linares e Hijos"            "Iglesias-Sauceda"                   
ch_company(locale = "hr_HR", n = 10)
#>  [1] "Marušić"                "Skupnjak"               "Malnar Načinović d.d." 
#>  [4] "Majdenić"               "Žerjav"                 "Trutanić d.d."         
#>  [7] "Jakuš"                  "Mamula Klasić j.d.o.o." "Klanac"                
#> [10] "Lojen j.d.o.o."        
```
