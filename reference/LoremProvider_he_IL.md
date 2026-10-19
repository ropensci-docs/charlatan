# Lorem provider Hebrew

Methods for Lorem Ipsum generation. Lorem Ipsum is a placeholder text
commonly used to demonstrate the visual form of a document or a typeface
without relying on meaningful content.

## See also

Other he:
[`PhoneNumberProvider_he_IL`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_he_IL.md),
[`hebrew-language`](https://docs.ropensci.org/charlatan/reference/hebrew-language.md)

Other IL:
[`PhoneNumberProvider_he_IL`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_he_IL.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_he_IL`

## Methods

### Public methods

- [`LoremProvider_he_IL$clone()`](#method-LoremProvider_he_IL-clone)

Inherited methods

- [`charlatan::BareProvider$bothify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-bothify)
- [`charlatan::BareProvider$lexify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-lexify)
- [`charlatan::BareProvider$numerify()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-numerify)
- [`charlatan::BareProvider$random_digit()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit)
- [`charlatan::BareProvider$random_digit_not_zero()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero)
- [`charlatan::BareProvider$random_digit_not_zero_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_not_zero_or_empty)
- [`charlatan::BareProvider$random_digit_or_empty()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_digit_or_empty)
- [`charlatan::BareProvider$random_element()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element)
- [`charlatan::BareProvider$random_element_prob()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_element_prob)
- [`charlatan::BareProvider$random_int()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_int)
- [`charlatan::BareProvider$random_letter()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-random_letter)
- [`charlatan::BareProvider$randomize_nb_elements()`](https://docs.ropensci.org/charlatan/reference/BareProvider.html#method-randomize_nb_elements)
- [`charlatan::BaseProvider$allowed_locales()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-allowed_locales)
- [`charlatan::BaseProvider$check_locale()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-check_locale)
- [`charlatan::BaseProvider$print()`](https://docs.ropensci.org/charlatan/reference/BaseProvider.html#method-print)
- [`charlatan::LoremProvider$initialize()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-initialize)
- [`charlatan::LoremProvider$paragraph()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-paragraph)
- [`charlatan::LoremProvider$paragraphs()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-paragraphs)
- [`charlatan::LoremProvider$sentence()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-sentence)
- [`charlatan::LoremProvider$sentences()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-sentences)
- [`charlatan::LoremProvider$text()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-text)
- [`charlatan::LoremProvider$word()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-word)
- [`charlatan::LoremProvider$words()`](https://docs.ropensci.org/charlatan/reference/LoremProvider.html#method-words)

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    LoremProvider_he_IL$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_he_IL$new()
x$word()
#> [1] "ערששף"
x$words(3)
#> [1] "לכנו"  "הבקיץ" "טידום"
x$words(6)
#> [1] "קוויס"     "איאקוליס"  "נון"       "סאפיאן"    "וסטיבולום" "עמחליף"   
x$sentence()
#> [1] "סולגק דול לרטי כאנה למרקוח מא."
x$paragraph()
#> [1] "לפמעט בליקרה נשואי חשלו סילקוף נשואי נולום אט. בלינך ולחת סילקוף דולור שערש גדדיש שערש וולופטה."
x$paragraphs(3)
#> [1] "דלאמת רוגצה ותלברו כלרשט סיט. נובש שבצק למטכין סוברט."                                                          
#> [2] "נון אס רוגצה עמחליף מיחוצים."                                                                                   
#> [3] "סאפיאן קונסקטורר אס התידם. קלובר קלובר מרגשי שערש תצטנפל ולחת ברשג. אקווזמן שעותלשך מנכם טידום קוויז קוויז איף."
cat(x$paragraphs(6), sep = "\n")
#> בראיט ברומץ יהול כלרשט. אלמנקום אקווזמן כלרשט אדנדום. לתכי מורגם וסטיבולום פוסיליס.
#> דס להאמית מרגשי דלאמת ניצאחו. בגורמי צורק קרהשק. דס סוברט נולום.
#> קלאצי וולופטה דולור אאוגו צורק לתיג נונסטי. הועניב שנרא כלרשט. ישבעס קלובר שנרא ברומץ לתיג. לתיג בליקרה מורגם ברשג לתיג.
#> מונפרד קוויס ותלברו קלאצי ניצאחו. כלרשט נובש ארווס.
#> צופעט סתשם שערש מרגשי מיחוצים. סוליסי צורק ברומץ שנרא סילקוף מורגם. כאנה דס למטכין אלמנקום.
#> יבש לכנו ישבעס קלובר חשלו וואל בורק? ישבעס. קולורס אאוגו לרטי אלית דז דולור נובש. בלובק פוסיליס לרטי טידום מנק.
x$text(19)
#> [1] "יהול ולתיעם סחטיר."
x <- LoremProvider_he_IL$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "וק --- מא --- ניצאחו. --- גדדיש --- גק --- היושבב --- ניבאה. --- קוויס --- דולור --- להאמית --- מיחוצים --- קולורס --- שבצק --- לכנוץ --- אקווזמן. --- ארווס --- נמרגי --- לכימפו."
```
