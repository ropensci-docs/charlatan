# Lorem provider Chinese (Taiwan)

Methods for Lorem Ipsum generation. Lorem Ipsum is a placeholder text
commonly used to demonstrate the visual form of a document or a typeface
without relying on meaningful content.

## See also

Other zh:
[`JobProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/JobProvider_zh_TW.md),
[`LoremProvider_zh_CN`](https://docs.ropensci.org/charlatan/reference/LoremProvider_zh_CN.md),
[`PhoneNumberProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_zh_TW.md),
[`chinese-language`](https://docs.ropensci.org/charlatan/reference/chinese-language.md)

Other TW:
[`JobProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/JobProvider_zh_TW.md),
[`PhoneNumberProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_zh_TW.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_zh_TW`

## Methods

### Public methods

- [`LoremProvider_zh_TW$clone()`](#method-LoremProvider_zh_TW-clone)

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

    LoremProvider_zh_TW$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_zh_TW$new()
x$word()
#> [1] "全國"
x$words(3)
#> [1] "通過" "系列" "詳細"
x$words(6)
#> [1] "因為" "主要" "在線" "原因" "首頁" "項目"
x$sentence()
#> [1] "功能 成為 使用 方面 空間 那些."
x$paragraph()
#> [1] "朋友 這樣 不能 一種 人民. 時候 控制 歡迎 包括."
x$paragraphs(3)
#> [1] "怎麼 網站 國際 狀態 生活 作者 教育. 可是 數據 更新 自己."                          
#> [2] "國內 學生 這麼 表示."                                                              
#> [3] "法律 生活 通過 系列 其實. 正在 大小 你的 成為 投資. 新聞 論壇 應用 推薦 經營 組織."
cat(x$paragraphs(6), sep = "\n")
#> 你們 所以 成功 表示.
#> 這種 空間 日本 能夠. 如何 網上 其他 要求 已經 點擊 城市. 提供 上海 文化 包括.
#> 方面 空間 安全 政府 根據 狀態 日本. 國內 日本 有關 會員 環境.
#> 兩個 很多 等級 產品 以后 點擊 應該. 更新 音樂 網站 到了 瀏覽 世界.
#> 包括 都是 發布 通過 無法. 聯系 如此 有些 運行 經濟 希望 音樂. 登錄 現在 提高 新聞 名稱 以下 歡迎.
#> 作者 包括 處理 他們 點擊 分析. 軟體 一起 決定 到了 評論 評論.
x$text(19)
#> [1] "東西 游戲 積分 一切 學生 的是."
x <- LoremProvider_zh_TW$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "目前 --- 一次 --- 以及 --- 生產 --- 問題 --- 品牌. --- 數據 --- 覺得 --- 設備 --- 國際 --- 擁有. --- 那個 --- 作為 --- 當前 --- 所有. --- 進行 --- 方法 --- 大學 --- 感覺. --- 沒有 --- 下載 --- 一定 --- 人民 --- 是一 --- 他的 --- 查看."
```
