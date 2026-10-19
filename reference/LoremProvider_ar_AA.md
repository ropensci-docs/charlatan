# Lorem provider Arabic

Methods for Lorem Ipsum generation. Lorem Ipsum is a placeholder text
commonly used to demonstrate the visual form of a document or a typeface
without relying on meaningful content.

## See also

Other ar:
[`arabic-language`](https://docs.ropensci.org/charlatan/reference/arabic-language.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_ar_AA`

## Methods

### Public methods

- [`LoremProvider_ar_AA$clone()`](#method-LoremProvider_ar_AA-clone)

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

    LoremProvider_ar_AA$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_ar_AA$new()
x$word()
#> [1] "الصعداء"
x$words(3)
#> [1] "ولكسمبورغ" "بفرض"      "حالية"    
x$words(6)
#> [1] "الحكم"   "ذات"     "لبلجيكا" "لان"     "عرفها"   "قِبل"    
x$sentence()
#> [1] "بدارت الإمتعاض بمما المتاخمة على وانهاء."
x$paragraph()
#> [1] "العالمية الفرنسي حالية تمهيد تُصب المعاهدات وبعض نتيجة. الخاسر به دار و مسارح."
x$paragraphs(3)
#> [1] "بعلى بحث أفريقيا وحرمان. بسبب وبعض اتّجة بالسيطرة."                                                   
#> [2] "بضرب بالمحور للجزر لعملة مسؤولية. السبب اعتداء المارق. الشّعبين وصغار موالية واتّجه."                  
#> [3] "الخطّة مرمى وحتى. إعمار شرسة والفلبين ألمّ. ضمنها أخر فقامت تعديل شموليةً كما. ببعض ليرتفع ببحشد بتحدّي."
cat(x$paragraphs(6), sep = "\n")
#> العالمي وبحلول مشاركة أفريقيا بقسوة بكلّ. غضون اليابانية أدوات.
#> الصينية وبدأت بالرّغم الشرق أملاً ماليزيا المارق. لليابان اعتداء ديسمبر عُقر وايرلندا سقطت عشوائية. غضون التقليدية المتاخمة ماليزيا ماشاء الله بكلّ.
#> لدحر ووصف إتفاقية ثانية لكون كلّ ديسمبر. الحدود قررت تجهيز الأرض ليرتفع.
#> بمباركة مما شعار استبدال. مسرح بانه انه وبداية والعتاد. الصعداء وانهاء بقسوة وإقامة وتنصيب الشرق العظمى.
#> الصين الأوروبية بالجوي مقاطعة. عُقر قائمة لدحر اليميني الصينية بنقطة شمال. الساحة السيطرة الآخر للسيطرة.
#> ولاتّساع حتى وباءت بولندا تطوير مايو الجنود. والحزب زهاء الساحة غرّة ببحشد ارتكبها جهة بشرية.
x$text(19)
#> [1] "التاريخ إتفاقية."
x <- LoremProvider_ar_AA$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "نفس --- ونتج --- اليميني --- جسيمة --- بحيث --- لفشل. --- جديدة --- وقام --- للسيطرة --- وعُرفت. --- ساعة --- ومطالبة --- وعُرفت --- التبرعات --- لغات --- الهجوم --- بأيدي."
```
