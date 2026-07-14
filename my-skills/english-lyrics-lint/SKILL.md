---
name: english-lyrics-lint
description: "检查和修正英文歌词的格式是否正确。包括歌曲标题和歌词英文大小写规则。Use when: checking or fixing song title capitalization, lyrics capitalization, title case, uppercase lowercase rules for music metadata, music tagging."
---

# English Lyrics Lint
## 歌词大小写规则
* 规则以 Apple Music 官方的标题大小写指南为基础。

### 适用场景
* 检查或修正歌曲标题（Song Title）的大小写
* 检查或修正歌词（Lyrics）每行的大小写
* 音乐元数据标注（Apple Music、iTunes、Spotify 等）

---

### 歌曲标题规则（Title Case）

#### 基本原则
* **禁止**全大写、全小写、或随意大小写
* 默认所有单词首字母大写（Title Case）
* `-`、`/`、`:` 前后的词同样适用所有规则

#### 首末词强制大写
* 标题的**第一个**和**最后一个**单词首字母必须大写，无论是否为小写词
* 括号内的**首词**和**末词**也适用此规则
    * 例：`War (What Is It Good For?)`

#### 强制小写词

以下词在非首末位置时**必须小写**：

| 语言 | 词列表 |
|------|--------|
| English | `a` `an` `and` `as` `but` `from` `nor` `of` `or` `so` `the` `to` `yet` |
| Spanish | `a` `al` `de` `del` `e` `el` `en` `la` `las` `los` `o` `para` `por` `un` `una` `y` |
| Portuguese | `a` `à` `ao` `aos` `as` `para` `das` `de` `do` `dos` `e` `pro` `um` `uma` `nas` `no` `nos` `o` `os` `às` `da` `pela` `pelas` `pelo` `pelos` `por` `em` `na` |

例：`In the Still of the Night`

#### 短介词小写（≤4 个字母）

以下介词在非首末位置时**小写**：`at` `by` `for` `from` `in` `into` `of` `off` `on` `onto` `out` `over` `to` `up` `with`

**例外（可大写的情况）**：
* 作为**动词短语**的一部分：`To Be, or Not to Be`
* 用作**其他词性**（副词、形容词、名词、动词）时可大写

**变体同样适用**：`da`（the）、`'Em`（Them）、`n'`（and）

例：`Viva la Gloria`

#### 强制大写词

以下词**必须大写**，即使位于非首末位置：

| 类型 | 词列表 |
|------|--------|
| 强制 | `Are` `If` `Is` `It` `Than` `That` `This` |
| 易混淆（建议大写） | `Be` `Will` `Do` `Not` `Me` `You` `Were` `Can` |

#### 版本信息

括号内的版本/说明信息**首词不强制大写**：
* 例：`珊瑚海 (feat. 梁心颐)`、`Something (Radio Edit)`

---

### 歌词规则（Lyrics Case）

#### 专有名词
按标准专有名词规则大小写：

| 类别 | 示例 |
|------|------|
| 宗教词汇 | `God` `You` `Him` `Your`（指代神） |
| 缩写 | `NASA` `FBI` |
| 地理位置 | `East Coast` `Southside` |
| 作品名 | 按作品原名 |
| 品牌名 | `Google` `Apple` `iPad` |

#### 每行首字母
* 每行歌词的**第一个字母必须大写**

---

### 快速对照示例

| 错误 | 正确 | 规则 |
|------|------|------|
| `i got the - single` | `I Got The - Single` | 全部首字母大写 |
| `What They're looking for` | `What They're Looking For` | 末词大写 |
| `In The Still Of The Night` | `In the Still of the Night` | 强制小写词 |
| `To be, Or Not To be` | `To Be, or Not to Be` | 强制大写 / 非首末小写 |
| `War (what is it good for?)` | `War (What Is It Good For?)` | 括号内首末大写；`Is` `It` 强制大写 |
| `珊瑚海 (Feat. 梁心颐)` | `珊瑚海 (feat. 梁心颐)` | 版本信息首词不大写 |
