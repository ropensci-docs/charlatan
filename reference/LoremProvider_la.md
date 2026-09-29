# Lorem provider Latin

lorem ipsum methods for generating random words in a language. Lorem
Ipsum is a placeholder text commonly used to demonstrate the visual form
of a document or a typeface without relying on meaningful content.

## See also

Other la:
[`latin-language`](https://docs.ropensci.org/charlatan/reference/latin-language.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_la`

## Methods

### Public methods

- [`LoremProvider_la$clone()`](#method-LoremProvider_la-clone)

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

    LoremProvider_la$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_la$new()
x$word()
#> [1] "voluptatum"
x$words(3)
#> [1] "amet"       "aspernatur" "ratione"   
x$words(6)
#> [1] "perferendis" "vero"        "quidem"      "quo"         "fugit"      
#> [6] "recusandae" 
x$sentence()
#> [1] "Accusantium repudiandae nam in corporis iste."
x$paragraph()
#> [1] "Ea voluptatibus natus repudiandae eos id. Recusandae saepe velit quidem optio maxime esse ex. Hic non temporibus natus impedit inventore. Ea sequi provident beatae."
x$paragraphs(3)
#> [1] "Saepe ut natus velit iste dignissimos iusto optio. Illo nulla iusto ipsam animi dolorum incidunt."                                                      
#> [2] "Voluptatum reprehenderit maxime quidem."                                                                                                                
#> [3] "Asperiores dicta ea dolorem provident delectus atque beatae. Maxime doloremque optio iusto non dolores. Iste optio officiis voluptate ipsum eius quasi."
cat(x$paragraphs(6), sep = "\n")
#> Tempore sequi earum fuga accusamus possimus labore. Molestias explicabo ducimus commodi vero fugiat.
#> Delectus optio optio ducimus dignissimos porro voluptates. Aperiam ipsam beatae molestiae.
#> Suscipit molestias soluta at architecto eos inventore. Quod quia provident commodi rem totam.
#> Voluptatem minima perspiciatis iusto sit. Provident officiis quae.
#> Eius molestias tempore. In voluptates eius.
#> Explicabo dolore excepturi voluptatibus quos asperiores. Commodi ad iste officia quasi. Rem corporis eius perferendis quam autem. Illo laboriosam quae facilis earum laborum.
x$text(19)
#> [1] "Aperiam vel quo."
x <- LoremProvider_la$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "Dolore --- cum --- voluptatum --- animi --- ea --- temporibus --- praesentium. --- Neque --- perspiciatis --- assumenda. --- Amet --- voluptas --- exercitationem --- dicta --- sequi --- culpa --- aut."
```
