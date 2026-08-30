# Lorem provider Chinese (China)

Methods for Lorem Ipsum generation. Lorem Ipsum is a placeholder text
commonly used to demonstrate the visual form of a document or a typeface
without relying on meaningful content.

## See also

Other zh:
[`JobProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/JobProvider_zh_TW.md),
[`LoremProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/LoremProvider_zh_TW.md),
[`PhoneNumberProvider_zh_TW`](https://docs.ropensci.org/charlatan/reference/PhoneNumberProvider_zh_TW.md),
[`chinese-language`](https://docs.ropensci.org/charlatan/reference/chinese-language.md)

## Super classes

[`charlatan::BareProvider`](https://docs.ropensci.org/charlatan/reference/BareProvider.md)
-\>
[`charlatan::BaseProvider`](https://docs.ropensci.org/charlatan/reference/BaseProvider.md)
-\>
[`charlatan::LoremProvider`](https://docs.ropensci.org/charlatan/reference/LoremProvider.md)
-\> `LoremProvider_zh_CN`

## Methods

### Public methods

- [`LoremProvider_zh_CN$clone()`](#method-LoremProvider_zh_CN-clone)

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

    LoremProvider_zh_CN$clone(deep = FALSE)

#### Arguments

- `deep`:

  Whether to make a deep clone.

## Examples

``` r
x <- LoremProvider_zh_CN$new()
x$word()
#> [1] "原因"
x$words(3)
#> [1] "价格" "我的" "名称"
x$words(6)
#> [1] "之后" "东西" "提供" "威望" "系统" "但是"
x$sentence()
#> [1] "不能 出现 认为 还是."
x$paragraph()
#> [1] "一直 就是 投资 看到 支持 觉得 设备 发表. 浏览 问题 一次 之间 发布 作者."
x$paragraphs(3)
#> [1] "一个 特别 分析 以后 等级 有些 历史. 当然 都是 教育 影响 单位. 最大 成功 更多 所以 一次 地址."                
#> [2] "感觉 一种 有关 那个."                                                                                        
#> [3] "今年 销售 认为 感觉 控制 文化. 国际 到了 行业 这些 显示. 系统 感觉 关于 系列 下载 是否. 基本 学校 孩子 地方."
cat(x$paragraphs(6), sep = "\n")
#> 中文 大小 决定 得到 关于 广告 不要 一个. 美国 工具 已经 资源.
#> 如何 方面 提高 发布 生活.
#> 情况 目前 能够 推荐. 以后 一起 必须 不是.
#> 免费 类别 东西 的话 电脑 人员. 一些 系列 一直 文化 过程 商品. 标题 出来 环境 音乐 规定.
#> 企业 感觉 不同 当然 质量 网上 对于.
#> 注册 名称 一次 日本 由于 信息 对于.
x$text(19)
#> [1] "社区 管理 管理 进入 全国 时候."
x <- LoremProvider_zh_CN$new(word_connector = " --- ")
x$paragraph(4)
#> [1] "资源 --- 地址 --- 主题 --- 一点 --- 您的 --- 过程 --- 状态 --- 标题. --- 之间 --- 作者 --- 地区 --- 上海 --- 合作 --- 密码. --- 成为 --- 当然 --- 推荐 --- 电脑. --- 论坛 --- 全国 --- 一点 --- 公司. --- 而且 --- 企业 --- 上海."
```
