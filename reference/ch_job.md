# Create fake jobs

Create fake jobs

## Usage

``` r
ch_job(n = 1, locale = NULL)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. Run
  `JobProvider$new()$allowed_locales()` for locales supported (default:
  en_US)

## See also

[JobProvider](https://docs.ropensci.org/charlatan/reference/JobProvider.md)

## Examples

``` r
ch_job()
#> [1] "Dentist"
ch_job(10)
#>  [1] "Gaffer"                                   
#>  [2] "Music therapist"                          
#>  [3] "Scientist, audiological"                  
#>  [4] "Geophysical data processor"               
#>  [5] "Sound technician, broadcasting/film/video"
#>  [6] "Systems analyst"                          
#>  [7] "Management consultant"                    
#>  [8] "Surveyor, rural practice"                 
#>  [9] "Scientist, research (maths)"              
#> [10] "Surveyor, hydrographic"                   
# or even ch_job(500)

ch_job(locale = "da_DK", n = 10)
#>  [1] "Kosmetolog"            "Administrationsøkonom" "Webudvikler"          
#>  [4] "Vagtplanlægger"        "Skibsmekaniker"        "Kemiingeniør"         
#>  [7] "Pedelmedhjælper"       "IT-projektassistent"   "Driftschef"           
#> [10] "Teknisk koordinator"  
ch_job(locale = "fi_FI", n = 10)
#>  [1] "Näönkäytön asiantuntija"           "Edunvalvontasihteeri"             
#>  [3] "Graafikko"                         "Karjamestari"                     
#>  [5] "Digitaalisen kokeen toteuttaja"    "Ohjaaja"                          
#>  [7] "Media- ja kulttuurikoordinaattori" "Innoittaja"                       
#>  [9] "Tallentaja"                        "Faktori"                          
ch_job(locale = "fr_FR", n = 10)
#>  [1] "Biologiste médical"                "Éditeur"                          
#>  [3] "Conducteur de train / TGV"         "Auxiliaire spécialisé vétérinaire"
#>  [5] "Architecte réseau"                 "Technicien automobile"            
#>  [7] "Chanteur"                          "Responsable micro"                
#>  [9] "Ingénieur brevets"                 "Vétérinaire"                      
ch_job(locale = "fr_CH", n = 10)
#>  [1] "Contremaître ramoneur avec brevet fédéral"                                                                    
#>  [2] "Mécanicien d'appareils à moteur CFC"                                                                          
#>  [3] "Expert domaine opératoire avec diplôme fédéral"                                                               
#>  [4] "Employé en restauration AFP"                                                                                  
#>  [5] "Employé en intendance AFP"                                                                                    
#>  [6] "Médiamaticien avec brevet fédéral"                                                                            
#>  [7] "Calorifugeur-tôlier CFC"                                                                                      
#>  [8] "Projeteur en technique du bâtiment chauffage CFC (champ professionnel Planification en technique du bâtiment)"
#>  [9] "Contrôleur de combustion avec brevet fédéral"                                                                 
#> [10] "Aide-peintre AFP"                                                                                             
ch_job(locale = "hr_HR", n = 10)
#>  [1] "Viši konzervator –  restaurator"  "Porezni savjetnik"               
#>  [3] "Viši informatičar"                "Magistar sestrinstva"            
#>  [5] "Magistar sanitarnog inženjerstva" "Krojač ženske odjeće"            
#>  [7] "Sigurnosni savjetnik"             "Inženjer rudarstva"              
#>  [9] "Slastičar"                        "Viši preparator"                 
ch_job(locale = "fa_IR", n = 10)
#>  [1] "نویسنده"    "باغ\fدار"   "خبر\fنگار"  "دانش\fآموز" "نجار"      
#>  [6] "مؤذن"       "آتش\fنشان"  "خبر\fنگار"  "نانوا"      "نانوا"     
ch_job(locale = "pl_PL", n = 10)
#>  [1] "Certyfikator energetyczny"  "Technik technologii drewna"
#>  [3] "Grabarz"                    "Pokojówka"                 
#>  [5] "Salowa"                     "Pośrednik ubezpieczeniowy" 
#>  [7] "Pisarz"                     "Rybak"                     
#>  [9] "Trener personalny"          "Kurator sztuki"            
ch_job(locale = "ru_RU", n = 10)
#>  [1] "Инженер-лесотехник"     "Портье"                 "Хирург"                
#>  [4] "Актёр"                  "Промышленный альпинист" "Упаковщик"             
#>  [7] "Радиолог"               "Металлург"              "Диджей"                
#> [10] "Педиатр"               
ch_job(locale = "uk_UA", n = 10)
#>  [1] "Режисер"        "Фермер"         "Доцент"         "Патологоанатом"
#>  [5] "Композитор"     "Швачка"         "Єгер"           "Фрілансер"     
#>  [9] "Адвокат"        "Живописець"    
ch_job(locale = "zh_TW", n = 10)
#>  [1] "西餐廚師"         "水利工程師"       "幼教班老師"       "廠務"            
#>  [5] "調音技術員"       "硬體工程研發主管" "量測／儀校人員"   "照顧指導員"      
#>  [9] "資料庫管理人員"   "食品衛生管理師"  
```
