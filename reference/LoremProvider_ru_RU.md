# Lorem provider Russian (Russia)

Methods for Lorem Ipsum generation. Lorem Ipsum is a placeholder text
commonly used to demonstrate the visual form of a document or a typeface
without relying on meaningful content.

## See also

Other ru:
[`JobProvider_ru_RU`](https://docs.ropensci.org/charlatan/reference/JobProvider_ru_RU.md),
[`PhoneNumberProvider_ru_RU`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_ru_RU.md),
[`russian-language`](https://docs.ropensci.org/charlatan/reference/russian-language.md)

Other RU:
[`JobProvider_ru_RU`](https://docs.ropensci.org/charlatan/reference/JobProvider_ru_RU.md),
[`PhoneNumberProvider_ru_RU`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_ru_RU.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_ru_RU`

## Methods

### Public methods

- [`LoremProvider_ru_RU$clone()`](#method-LoremProvider_ru_RU-clone)

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

    LoremProvider_ru_RU$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_ru_RU$new()
x$word()
#> [1] "триста"
x$words(3)
#> [1] "крыса"     "запретить" "нервно"   
x$words(6)
#> [1] "способ"      "пропасть"    "невыносимый" "кожа"        "бегать"     
#> [6] "сынок"      
x$sentence()
#> [1] "выразить невозможно аллея стакан необычный руководитель."
x$paragraph()
#> [1] "зима строительство болото исследование помимо цель. прежний заработать место. мусор ручей бегать потом июнь поезд."
x$paragraphs(3)
#> [1] "серьезный угроза обида уточнить тусклый горький природа костер. мимо решетка руководитель социалистический салон близко расстройство. идея народ металл еврейский неожиданный полевой тревога. видимо команда слишком мгновение."
#> [2] "построить разуметься тяжелый о засунуть ломать какой. умолять совет деловой услать степь. интеллектуальный строительство июнь премьера точно выраженный возможно ныне."                                                          
#> [3] "мучительно зачем бак медицина заявление дурацкий. ночь мелочь выкинуть назначить."                                                                                                                                               
cat(x$paragraphs(6), sep = "\n")
#> тысяча заложить исполнять ломать протягивать результат. житель совещание одиннадцать столетие спасть изредка интеллектуальный. пламя намерение миф монета деньги мальчишка головной.
#> художественный присесть монета коллектив о куча. покидать ученый издали снимать полоска.
#> пропадать адвокат процесс. прошептать инфекция медицина изучить.
#> товар забирать порядок дрогнуть термин проход актриса. тяжелый растеряться жить сравнение невыносимый сверкать. выдержать спорт рис экзамен следовательно.
#> рот близко устройство основание. народ угол нажать. цвет рассуждение жестокий приличный лапа решение.
#> танцевать выкинуть даль указанный при. невыносимый господь угроза деньги.
x$text(19)
#> [1] "Пересечь."
x <- LoremProvider_ru_RU$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "крутой --- изучить --- шлем --- редактор --- отражение. --- гулять --- покинуть --- единый --- а --- монета --- радость --- цвет. --- изображать --- господь --- палата --- падаль --- остановить --- казнь --- разнообразный. --- слишком --- дальний --- число --- заведение --- валюта. --- штаб --- костер --- ответить --- болото --- совещание --- бегать --- школьный."
```
