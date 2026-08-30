# Generate a fake dataset

Generate a fake dataset

## Usage

``` r
ch_generate(..., n = 10, locale = NULL)
```

## Arguments

- ...:

  columns to include. must be in the allowed set. See **Allowed column
  names** below. Three default columns are included (name, job,
  phone_number) if nothing is specified - but are overridden by any
  input.

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. options: only supported for data types
  that have locale support, See each data provider for details.

## Allowed column names

- name (default included)

- job (default included)

- phone_number (default included)

- currency

- color_name

- rgb_color

- rgb_css_color

## Examples

``` r
ch_generate()
#> # A tibble: 10 × 3
#>    name                     job                                   phone_number  
#>    <chr>                    <chr>                                 <chr>         
#>  1 Chrystal Mitchell        Education administrator               (066)146-4004 
#>  2 Dr. Gwendolyn Gleason MD Financial manager                     1-368-816-926…
#>  3 Wilmer Kling             Librarian, academic                   403.301.5133x…
#>  4 Yetta Reilly             Research scientist (life sciences)    821.272.6844x…
#>  5 Bernice Halvorson        Medical sales representative          812-090-1803x…
#>  6 Ms. Tabitha Lakin MD     Forest/woodland manager               1-595-507-371…
#>  7 Mrs. Mayra Bogisich      Electronics engineer                  (671)676-0902 
#>  8 Maren Schuster           Development worker, international aid 071-793-2871x…
#>  9 Hasan Gaylord            Chartered public finance accountant   215.386.1532x…
#> 10 Noel Mraz DDS            Psychiatrist                          (043)158-2095…
ch_generate(n = 1)
#> # A tibble: 1 × 3
#>   name           job                 phone_number      
#>   <chr>          <chr>               <chr>             
#> 1 Corean Simonis Corporate treasurer 433.600.5661x57388
ch_generate(n = 100)
#> # A tibble: 100 × 3
#>    name                      job                                    phone_number
#>    <chr>                     <chr>                                  <chr>       
#>  1 Omar Ledner               Company secretary                      (354)208-70…
#>  2 Carie Breitenberg         Geneticist, molecular                  1-977-931-8…
#>  3 Jovanny Wiza              Purchasing manager                     928.534.3025
#>  4 Ms. Leann Bergstrom PhD   Operations geologist                   1-332-240-1…
#>  5 Burney Bartell            Presenter, broadcasting                842-806-390…
#>  6 Dr. Franklin Konopelski V Dispensing optician                    (278)611-64…
#>  7 Alex Miller PhD           Publishing copy                        1-850-762-1…
#>  8 Mr. Brittany Renner IV    Museum/gallery conservator             (874)262-06…
#>  9 Tristan Schmidt           Conservation officer, historic buildi… +97(7)34739…
#> 10 Teela Bahringer           Therapist, art                         502.944.708…
#> # ℹ 90 more rows

ch_generate("job")
#> # A tibble: 10 × 1
#>    job                                                      
#>    <chr>                                                    
#>  1 Outdoor activities/education manager                     
#>  2 Radio broadcast assistant                                
#>  3 Research scientist (medical)                             
#>  4 Clinical scientist, histocompatibility and immunogenetics
#>  5 Engineer, technical sales                                
#>  6 Industrial/product designer                              
#>  7 Commercial/residential surveyor                          
#>  8 Commercial art gallery manager                           
#>  9 Community education officer                              
#> 10 Chiropodist                                              
ch_generate("job", "name")
#> # A tibble: 10 × 2
#>    job                                 name                      
#>    <chr>                               <chr>                     
#>  1 Chemist, analytical                 Edison VonRueden-O'Connell
#>  2 Engineer, manufacturing             Michael Kertzmann-Rau     
#>  3 Engineer, broadcasting (operations) Kyree Corwin              
#>  4 Artist                              Axel Skiles               
#>  5 Counsellor                          Judge Little              
#>  6 Barrister's clerk                   Willa Nitzsche            
#>  7 Therapeutic radiographer            Ms. Brigitte Maggio PhD   
#>  8 Professor Emeritus                  Sibyl Muller              
#>  9 Interpreter                         Clare Beier               
#> 10 Television camera operator          Mr. Garfield Sawayn PhD   
ch_generate("job", "color_name")
#> # A tibble: 10 × 2
#>    job                                color_name       
#>    <chr>                              <chr>            
#>  1 Teacher, early years/pre           LightGreen       
#>  2 Building control surveyor          MediumSpringGreen
#>  3 Amenity horticulturist             LightSteelBlue   
#>  4 Financial planner                  GreenYellow      
#>  5 Psychotherapist                    Teal             
#>  6 Community pharmacist               Chocolate        
#>  7 Public relations account executive Violet           
#>  8 Records manager                    DarkGoldenRod    
#>  9 Ceramics designer                  PeachPuff        
#> 10 Musician                           Aqua             

# locale
ch_generate(locale = "en_US")
#> # A tibble: 10 × 3
#>    name                      job                             phone_number      
#>    <chr>                     <chr>                           <chr>             
#>  1 Dewayne Heller            Geophysical data processor      00090724093       
#>  2 Carrol Veum-Runolfsdottir Land/geomatics surveyor         1-454-662-9527x107
#>  3 Milford Wisoky Jr.        Special effects artist          +51(8)6661803650  
#>  4 Ms. Audrianna Hauck       Biomedical engineer             568-902-6037      
#>  5 Stefan Robel              Engineering geologist           074-736-1094x506  
#>  6 Solon Graham-Bergnaum     Manufacturing engineer          +37(1)6940759022  
#>  7 Kaci Erdman               Barista                         371.062.8192x10880
#>  8 Mr. Len Runolfsdottir     Ophthalmologist                 (562)254-6182     
#>  9 Dr. Shaquan Lakin         Chartered management accountant (359)908-3441x9943
#> 10 Ishaan Grant              General practice doctor         501-655-9195x3819 
ch_generate(locale = "fr_FR")
#> # A tibble: 10 × 3
#>    name                job                             phone_number        
#>    <chr>               <chr>                           <chr>               
#>  1 Rémy-Timothée Louis Apiculteur                      0844845011          
#>  2 Catherine Humbert   Podo-orthésiste                 01 92 41 28 77      
#>  3 Juliette Auger      Auxiliaire de vie sociale       05 53 78 09 08      
#>  4 Léon Dijoux         Journaliste                     +33 2 56 58 66 48   
#>  5 Guillaume L'Briand  Technicien                      0194446582          
#>  6 Pénélope Dupre      Cordonnier                      0291999484          
#>  7 Alexandre Schmitt   Contrôleur technique automobile 04 26 61 20 43      
#>  8 Dorothée Didier     Conseiller en génétique         +33 (0)2 03 60 52 87
#>  9 Marthe Leduc        Pédiatre                        +33 (0)4 78 64 04 69
#> 10 Noël Roussél        Chef de publicité               +33 (0)1 90 70 79 51
ch_generate(locale = "fr_CH")
#> # A tibble: 10 × 3
#>    name                    job                                      phone_number
#>    <chr>                   <chr>                                    <chr>       
#>  1 Nicole Bourquin         Préparateur Humains avec brevet fédéral  +41 49 523 …
#>  2 Daniel Besse-Robadey    Chef d'entreprise diplomée en boulanger… 0900 396 429
#>  3 Marcel Chenaux          Couturier avec brevet fédéral            0901 429 089
#>  4 René Pasquier           Opticien en instruments de précision CFC 020 092 13 …
#>  5 Yvonne Jacot-Guillarmod Vannier créateur CFC                     052 816 52 …
#>  6 Manon Chopard           Vannier créateur CFC                     0900 605 619
#>  7 Nolan Brandt            Policier avec brevet fédéral             090 662 98 …
#>  8 Hugo Monnard            Gouvernant de maison avec brevet fédéral +41 27 800 …
#>  9 Nathalie Bavaud         Accompagnateur de randonnée avec brevet… +41 (0)88 2…
#> 10 Jean-Pierre Menthonnex  Gestionnaire d'entreprise diplômé de la… +41 (0)57 3…
```
