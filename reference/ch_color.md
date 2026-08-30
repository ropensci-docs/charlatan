# Create fake colors

Create fake colors

## Usage

``` r
ch_color_name(n = 1, locale = NULL)

ch_safe_color_name(n = 1, locale = NULL)

ch_hex_color(n = 1)

ch_safe_hex_color(n = 1)

ch_rgb_color(n = 1)

ch_rgb_css_color(n = 1)
```

## Arguments

- n:

  (integer) number of things to get, any non-negative integer

- locale:

  (character) the locale to use. See `colors()$allowed_locales()` for
  locales supported. Affects the `ch_color_name` and
  `ch_safe_color_name` functions

## See also

[ColorProvider](https://docs.ropensci.org/charlatan/reference/ColorProvider.md)

## Examples

``` r
ch_color_name()
#> [1] "Orchid"
ch_color_name(10)
#>  [1] "Moccasin"      "DarkViolet"    "Turquoise"     "DeepSkyBlue"  
#>  [5] "DarkSlateBlue" "Snow"          "DarkBlue"      "WhiteSmoke"   
#>  [9] "DeepPink"      "MediumBlue"   
# or even ch_color_name(500)

ch_safe_color_name()
#> [1] "navy"
ch_safe_color_name(10)
#>  [1] "maroon"  "green"   "black"   "maroon"  "navy"    "yellow"  "yellow" 
#>  [8] "aqua"    "maroon"  "fuchsia"

ch_hex_color()
#> [1] "#10BD77"
ch_hex_color(10)
#>  [1] "#50C64C" "#A602E9" "#F40AC7" "#3FC13D" "#06A7D5" "#8EDFFC" "#4FCD9D"
#>  [8] "#2CC973" "#39C3C0" "#CC14A6"
# or even ch_hex_color(1000)

ch_safe_hex_color()
#> [1] "#ff6699"
ch_safe_hex_color(10)
#>  [1] "#9933ff" "#33ff33" "#cc99ff" "#cc0033" "#990099" "#66cc00" "#990099"
#>  [8] "#6699cc" "#ccffff" "#ff99cc"

ch_rgb_color()
#> [[1]]
#> [1] 149 168 201
#> 
ch_rgb_color(10)
#> [[1]]
#> [1]  91 104 225
#> 
#> [[2]]
#> [1]  99 143 169
#> 
#> [[3]]
#> [1] 184 182 202
#> 
#> [[4]]
#> [1] 91 34 98
#> 
#> [[5]]
#> [1] 197  17 215
#> 
#> [[6]]
#> [1] 197 158 197
#> 
#> [[7]]
#> [1] 189 153 212
#> 
#> [[8]]
#> [1] 224   1  37
#> 
#> [[9]]
#> [1]   3 214 120
#> 
#> [[10]]
#> [1] 206  35 145
#> 

ch_rgb_css_color()
#> [1] "rgb(69, 245, 167)"
ch_rgb_css_color(10)
#>  [1] "rgb(250, 178, 189)" "rgb(86, 39, 78)"    "rgb(67, 201, 119)" 
#>  [4] "rgb(208, 226, 214)" "rgb(154, 236, 142)" "rgb(101, 215, 0)"  
#>  [7] "rgb(37, 90, 98)"    "rgb(98, 156, 183)"  "rgb(122, 127, 226)"
#> [10] "rgb(152, 119, 177)"

ch_color_name(locale = "uk_UA")
#> [1] "Джинсовий"
ch_color_name(n = 10, locale = "uk_UA")
#>  [1] "Синя пил"                         "Жовтий"                          
#>  [3] "Колір жовтого шкільного автобуса" "Гумігут"                         
#>  [5] "Шафрановий"                       "Темно-бірюзовий"                 
#>  [7] "Персиковий"                       "Фіолетово-баклажановий"          
#>  [9] "Помаранчевий"                     "Сапфіровий"                      

ch_safe_color_name(locale = "uk_UA")
#> [1] "Чорний"
ch_safe_color_name(n = 10, locale = "uk_UA")
#>  [1] "Жовтий"               "Ціан (колір)"         "Жовтий"              
#>  [4] "Срібний"              "Ціан (колір)"         "Жовтий"              
#>  [7] "Ціан (колір)"         "Колір морської хвилі" "Чорний"              
#> [10] "Колір морської хвилі"
```
