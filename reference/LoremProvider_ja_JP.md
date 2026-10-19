# Lorem provider Japanese

Methods for Lorem Ipsum generation. Lorem Ipsum is a placeholder text
commonly used to demonstrate the visual form of a document or a typeface
without relying on meaningful content.

## See also

Other ja:
[`PersonProvider_ja_JP`](https://docs.ropensci.org/charlatan/reference/PersonProvider_ja_JP.md),
[`PhoneNumberProvider_ja_JP`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_ja_JP.md),
[`japanese-language`](https://docs.ropensci.org/charlatan/reference/japanese-language.md)

Other JP:
[`PersonProvider_ja_JP`](https://docs.ropensci.org/charlatan/reference/PersonProvider_ja_JP.md),
[`PhoneNumberProvider_ja_JP`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_ja_JP.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_ja_JP`

## Methods

### Public methods

- [`LoremProvider_ja_JP$clone()`](#method-LoremProvider_ja_JP-clone)

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

    LoremProvider_ja_JP$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_ja_JP$new()
x$word()
#> [1] "残る"
x$words(3)
#> [1] "催眠術" "カラム" "ボトル"
x$words(6)
#> [1] "販売"     "数字"     "ホイール" "ヒール"   "ジャム"   "ボトル"  
x$sentence()
#> [1] "サワー 明らかにする メニュー ベルベット."
x$paragraph()
#> [1] "柔らかい 尊敬する 式 ストレージ. リフト 助けて トス 部隊 必要."
x$paragraphs(3)
#> [1] "ブレーキ 知覚 高い 細かい バケツ コンペ カラム. 保証金 〜 は 教会 シェービング フェミニスト 主人. タワー 〜 コーラス 尿 偏差 は パン."
#> [2] "立派な 運 反射 ホイール 副 知覚. 憲法 探査 バナー 発生する 憲法 ホイール あなた自身."                                                 
#> [3] "評議会 再現する 憲法 雪 主人 屋根裏 部隊 不自然な. 文言 見落とす 指名."                                                               
cat(x$paragraphs(6), sep = "\n")
#> ノート クロス 暖かい リフト バナー. リハビリ 柔らかい 意図 不自然な. 明らかにする リハビリ ハンマー リハビリ 教授 キャビネット 月.
#> 狐 クルー バスケット コミュニティ 障害.
#> 隠す インチ パーセント あなた自身 偏差 日曜日 バナー 追放する.
#> 主婦 持っていました 持つ 彼. 倫理 指名 コンペ 柔らかい ストレージ 教授 陶器.
#> 差別する 創傷 クロス. キャビネット 探査 バケツ 文言 画面 敵対的な. 血まみれの クロス 省略 障害 デッド 目的 サラダ.
#> 普通の 風景 錯覚 月. ジャーナル 装置 トーン 立派な 尊敬する 証言する. ヒール 運 暖かい.
x$text(19)
#> [1] "数字 ピック アクセルペダル."
x <- LoremProvider_ja_JP$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "持つ --- 持ってる --- シェービング --- 立派な --- 戦略的 --- 追放する --- 持つ --- トーン. --- 電池 --- 販売 --- フェミニスト. --- ホイール --- 探査 --- ニュース --- 索引 --- 数字."
```
