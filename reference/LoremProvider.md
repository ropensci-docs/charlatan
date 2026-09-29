# LoremProvider

lorem ipsum methods for generating random words in a language. Lorem
Ipsum is a placeholder text commonly used to demonstrate the visual form
of a document or a typeface without relying on meaningful content.

## Note

You cannot instantiate the Parent providers. You must use one of the
localized one.

## See also

Other ParentProviders:
[`AddressProvider`](https://docs.ropensci.org/charlatan/reference/AddressProvider.md),
[`ColorProvider`](https://docs.ropensci.org/charlatan/reference/ColorProvider.md),
[`CompanyProvider`](https://docs.ropensci.org/charlatan/reference/CompanyProvider.md),
[`InternetProvider`](https://docs.ropensci.org/charlatan/reference/InternetProvider.md),
[`JobProvider`](https://docs.ropensci.org/charlatan/reference/JobProvider.md),
[`PersonProvider`](https://docs.ropensci.org/charlatan/reference/PersonProvider.md),
[`PhoneNumberProvider`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider.md),
[`TaxonomyProvider`](https://docs.ropensci.org/charlatan/reference/TaxonomyProvider.md),
[`UserAgentProvider`](https://docs.ropensci.org/charlatan/reference/UserAgentProvider.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `LoremProvider`

## Methods

### Public methods

- [`LoremProvider$new()`](#method-LoremProvider-new)

- [`LoremProvider$word()`](#method-LoremProvider-word)

- [`LoremProvider$words()`](#method-LoremProvider-words)

- [`LoremProvider$sentence()`](#method-LoremProvider-sentence)

- [`LoremProvider$sentences()`](#method-LoremProvider-sentences)

- [`LoremProvider$paragraph()`](#method-LoremProvider-paragraph)

- [`LoremProvider$paragraphs()`](#method-LoremProvider-paragraphs)

- [`LoremProvider$text()`](#method-LoremProvider-text)

- [`LoremProvider$clone()`](#method-LoremProvider-clone)

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

------------------------------------------------------------------------

### Method `new()`

Create a new `LoremProvider` object

#### Usage

    LoremProvider$new(sentence_punctuation = ".", word_connector = " ")

#### Arguments

- `sentence_punctuation`:

  (character) End of sentence punctuation

- `word_connector`:

  (character) Default connector between words

#### Returns

A new `LoremProvider` object

------------------------------------------------------------------------

### Method `word()`

Generate a random word

#### Usage

    LoremProvider$word(ext_words = NULL)

#### Arguments

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

a single word

------------------------------------------------------------------------

### Method `words()`

Generate a character vector of random words

#### Usage

    LoremProvider$words(nb = 3, ext_words = NULL)

#### Arguments

- `nb`:

  (integer) how many words to return

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

many words

------------------------------------------------------------------------

### Method `sentence()`

Generate a random sentence

#### Usage

    LoremProvider$sentence(
      nb_words = 6,
      variable_nb_words = TRUE,
      ext_words = NULL
    )

#### Arguments

- `nb_words`:

  (integer) around how many words the sentence should contain

- `variable_nb_words`:

  set to `FALSE` if you want exactly `nb` words returned, otherwise the
  result may include a number of words of `nb` +/-40% (with a minimum of
  1)

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

a single sentence

------------------------------------------------------------------------

### Method `sentences()`

Generate a character vector of random sentences

#### Usage

    LoremProvider$sentences(nb = 3, ext_words = NULL)

#### Arguments

- `nb`:

  (integer) how many sentences to return

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

many sentences

------------------------------------------------------------------------

### Method `paragraph()`

Generate a single paragraph

#### Usage

    LoremProvider$paragraph(
      nb_sentences = 3,
      variable_nb_sentences = TRUE,
      ext_words = NULL
    )

#### Arguments

- `nb_sentences`:

  (integer) around how many sentences the paragraph should contain

- `variable_nb_sentences`:

  set to `FALSE` if you want exactly `nb` sentences returned, otherwise
  the result may include a number of sentences of `nb` +/-40% (with a
  minimum of 1)

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

a single paragraph

------------------------------------------------------------------------

### Method `paragraphs()`

Generate many paragraphs

#### Usage

    LoremProvider$paragraphs(nb = 3, ext_words = NULL)

#### Arguments

- `nb`:

  (integer) how many paragraphs to return

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

many paragraphs

------------------------------------------------------------------------

### Method [`text()`](https://rdrr.io/r/graphics/text.html)

Generate a random text string. Depending on the `max_nb_chars`, returns
a string made of words, sentences, or paragraphs.

#### Usage

    LoremProvider$text(max_nb_chars = 200, ext_words = NULL)

#### Arguments

- `max_nb_chars`:

  Maximum number of characters the text should contain (minimum 5)

- `ext_words`:

  a character vector of words you would like to have instead of "Lorem
  ipsum"

#### Returns

character string of words

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    LoremProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
