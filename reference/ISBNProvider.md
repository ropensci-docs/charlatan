# ISBNProvider

International Standard Book Number - Provider. ISBN starts with group
code, all English language ISBN-10 codes start with a 0 or 1, and all
German language books start with a 3. see
<https://en.wikipedia.org/wiki/List_of_ISBN_registration_groups>.

Charlatan does not provide further helpers for you, but you can supply
the prefix yourself, if for instance you want to create Mexican ISBNs
you can by supplying the ISBN10 prefix 970, or for Andorra supply the
ISBN 13 prefix 97899920 (that is 978 for ISBN13, and 99920 for Andorra).

## Super class

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\> `ISBNProvider`

## Methods

### Public methods

- [`ISBNProvider$isbn10()`](#method-ISBNProvider-isbn10)

- [`ISBNProvider$isbn13()`](#method-ISBNProvider-isbn13)

- [`ISBNProvider$clone()`](#method-ISBNProvider-clone)

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

### Method `isbn10()`

Make a ISBN10 This is a completely random (apart from the prefix), but
valid ISBN10 number.

#### Usage

    ISBNProvider$isbn10(n = 1, prefix = NULL)

#### Arguments

- `n`:

  (integer) number of ISBN10s to make, default=1

- `prefix`:

  (integer/character) prefix for ISBN

------------------------------------------------------------------------

### Method `isbn13()`

Make a ISBN13. This is a completely random (apart from the prefix), but
valid ISBN13 number.

#### Usage

    ISBNProvider$isbn13(n = 1, prefix = NULL)

#### Arguments

- `n`:

  (integer) number of ISBN10s to make, default=1

- `prefix`:

  (integer/character) prefix for ISBN

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    ISBNProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
z <- ISBNProvider$new()
z$isbn10()
#> [1] "5957248592"
z$isbn13()
#> [1] "0835502080911"
z$isbn10(10)
#>  [1] "7990380129" "1078641692" "6991391778" "3781347478" "353755866X"
#>  [6] "1336834692" "1417432306" "6045962761" "1008929379" "7460187216"
z$isbn13(100)
#>   [1] "3420028320077" "3591063620627" "6662150363608" "5981880022984"
#>   [5] "4720598175930" "8261293589197" "8494311314932" "7102758984557"
#>   [9] "0672999927301" "6032716456929" "5199572800585" "8059589376640"
#>  [13] "6404180720910" "3976341669701" "1305515021908" "9244224899984"
#>  [17] "4309839848576" "7507710882924" "5031404937468" "0046272557248"
#>  [21] "3726677385154" "9740102581571" "4298647936394" "5055157526762"
#>  [25] "4533838873714" "6436360072984" "2664576597111" "4492413883374"
#>  [29] "2464956992303" "3882385588376" "5726996579621" "3674811447483"
#>  [33] "6857161290948" "7166991043952" "6950904015065" "4369515782280"
#>  [37] "7141270894937" "7499387453067" "6273030620980" "0731918606496"
#>  [41] "3897644805248" "3995435404127" "1946059061632" "6228273987024"
#>  [45] "6309400965877" "7850862768999" "2469147589065" "3451423196738"
#>  [49] "5376319023272" "2785113070802" "8918058189290" "7390953355252"
#>  [53] "2935046906123" "0585569475884" "4707943310215" "6749067938287"
#>  [57] "9099612809836" "1642421032704" "5983810742894" "3644288778038"
#>  [61] "6109036640120" "3369363802797" "0611295794613" "0505262409313"
#>  [65] "0006090179824" "2464571020665" "5534305360361" "5005796983853"
#>  [69] "9038902472084" "2046137386400" "3624803906146" "9483351358302"
#>  [73] "6404962843073" "3138380603010" "8917260786051" "8821864303425"
#>  [77] "7534906588469" "8983506579671" "3090640138697" "6863261798376"
#>  [81] "6826207331464" "4855244757151" "5948721602507" "4058689717210"
#>  [85] "5283281931316" "3438183283106" "3778974248335" "4687267709592"
#>  [89] "8154854038268" "5821926087525" "8518321088550" "3312769278864"
#>  [93] "8882132069474" "7900628601944" "5476184204902" "0326425901617"
#>  [97] "0065669321842" "7691267562887" "8315139022987" "3348697761932"
# or even z$isbn10(500)
```
