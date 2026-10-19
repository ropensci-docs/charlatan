# FileProvider

file methods

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\> `FileProvider`

## Methods

### Public methods

- [`FileProvider$new()`](#method-FileProvider-new)

- [`FileProvider$mime_type()`](#method-FileProvider-mime_type)

- [`FileProvider$file_name()`](#method-FileProvider-file_name)

- [`FileProvider$file_extension()`](#method-FileProvider-file_extension)

- [`FileProvider$file_path()`](#method-FileProvider-file_path)

- [`FileProvider$clone()`](#method-FileProvider-clone)

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

Create a new `FileProvider` object

#### Usage

    FileProvider$new()

#### Returns

A new `FileProvider` object

------------------------------------------------------------------------

### Method `mime_type()`

a random mime type

#### Usage

    FileProvider$mime_type(category = NULL)

#### Arguments

- `category`:

  (character) a mime type category of mime types, one of application,
  audio, image, message, model, multipart, text or video. default:
  `NULL`

------------------------------------------------------------------------

### Method `file_name()`

a random file name

#### Usage

    FileProvider$file_name(category = NULL, extension = NULL)

#### Arguments

- `category`:

  (character) a category of file extension type, one of audio, image,
  office, text or video. default: `NULL`. If this is given, `extension`
  is ignored

- `extension`:

  (character) a file extension. if this is given, `category` is ignored.

------------------------------------------------------------------------

### Method `file_extension()`

a random file extension

#### Usage

    FileProvider$file_extension(category = NULL)

#### Arguments

- `category`:

  (character) a category of file extension type, one of audio, image,
  office, text or video. default: `NULL`

------------------------------------------------------------------------

### Method `file_path()`

a random file path

#### Usage

    FileProvider$file_path(depth = 1, category = NULL, extension = NULL)

#### Arguments

- `depth`:

  (character) depth of the file (depth \>= 0). default: 1

- `category`:

  (character) a category of file extension type, one of audio, image,
  office, text or video. default: `NULL`. If this is given, `extension`
  is ignored

- `extension`:

  (character) a file extension. if this is given, `category` is ignored.

------------------------------------------------------------------------

### Method `clone()`

The objects of this class are cloneable with this method.

#### Usage

    FileProvider$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.
