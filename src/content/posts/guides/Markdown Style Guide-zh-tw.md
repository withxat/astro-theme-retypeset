---
title: Markdown 樣式指南
published: 2025-03-08
updated: 2025-03-23
tags:
  - 指南
pin: 98
toc: false
lang: zh-tw
abbrlink: markdown-style-guide
---

以下是一些基本的 Markdown 語法示例，及其在 Retypeset 主題中的樣式效果。

## 標題

在文字前添加井號 `#` 與空格，即可創建標題。井號數量對應標題等級。

### 語法

```
# 一級標題
## 二級標題
### 三級標題
#### 四級標題
##### 五級標題
###### 六級標題
```

### 效果

# 一級標題
## 二級標題
### 三級標題
#### 四級標題
##### 五級標題
###### 六級標題

## 段落

使用空行分隔文字，即可創建段落。

### 語法

```
孔乙己一到店，所有喝酒的人便都看著他笑，有的叫道："孔乙己，你臉上又添上新傷疤了！"他不回答，對櫃裡說："溫兩碗酒，要一碟茴香豆。"便排出九文大錢。他們又故意的高聲嚷道："你一定又偷了人家的東西了！"孔乙己睜大眼睛說："你怎麼這樣憑空污人清白……""什麼清白？我前天親眼見你偷了何家的書，吊著打。"孔乙己便漲紅了臉，額上的青筋條條綻出，爭辯道："竊書不能算偷……竊書！……讀書人的事，能算偷麼？"接連便是難懂的話，什麼"君子固窮"，什麼"者乎"之類，引得眾人都哄笑起來：店內外充滿了快活的空氣。

聽人家背地裡談論，孔乙己原來也讀過書，但終於沒有進學，又不會營生；於是愈過愈窮，弄到將要討飯了。
```

### 效果

孔乙己一到店，所有喝酒的人便都看著他笑，有的叫道："孔乙己，你臉上又添上新傷疤了！"他不回答，對櫃裡說："溫兩碗酒，要一碟茴香豆。"便排出九文大錢。他們又故意的高聲嚷道："你一定又偷了人家的東西了！"孔乙己睜大眼睛說："你怎麼這樣憑空污人清白……""什麼清白？我前天親眼見你偷了何家的書，吊著打。"孔乙己便漲紅了臉，額上的青筋條條綻出，爭辯道："竊書不能算偷……竊書！……讀書人的事，能算偷麼？"接連便是難懂的話，什麼"君子固窮"，什麼"者乎"之類，引得眾人都哄笑起來：店內外充滿了快活的空氣。

聽人家背地裡談論，孔乙己原來也讀過書，但終於沒有進學，又不會營生；於是愈過愈窮，弄到將要討飯了。

## 圖片

使用感嘆號 `!` 方括號 `[]` 與圓括號 `()`，即可添加圖片。這些都是半形符號，而非全形符號。

### 語法

```
![圖片描述](../_images/image-01.jpeg)

![圖片描述](https://image.example.com/image-01.webp)
```

### 效果

![圖片描述](https://image.radishzz.cc/picsmaller/03.webp)

## 區塊引用

使用 `>` 符號和空格，即可創建區塊引用，其中可包含多個段落。使用 `<cite>` 或 `<footer>` 標籤，即可標註引用來源，同時可通過 `[^1]` 或 `[^note]` 格式插入腳註。

### 多個段落

#### 語法

```markdown
> 天地不仁，以萬物為芻狗。
>
> **提示**：引用區塊內可使用 _Markdown 語法_。
```

#### 效果

> 天地不仁，以萬物為芻狗。
>
> **提示**：引用區塊內可使用 _Markdown 語法_。

### 標註引用來源

#### 語法

```markdown
> 在我的後園，可以看見牆外有兩株樹，一株是棗樹，還有一株也是棗樹。
>
> —— <cite>《秋夜》[^1]</cite>

[^1]: 《[秋夜](https://zh.wikisource.org/wiki/%E7%A7%8B%E5%A4%9C_(%E9%AD%AF%E8%BF%85))》是魯迅散文詩集《野草》中的第一首散文詩，創作於 1924 年。
```

#### 效果

> 在我的後園，可以看見牆外有兩株樹，一株是棗樹，還有一株也是棗樹。
>
> —— <cite>《秋夜》[^1]</cite>

[^1]: 《[秋夜](https://zh.wikisource.org/wiki/%E7%A7%8B%E5%A4%9C_(%E9%AD%AF%E8%BF%85))》是魯迅散文詩集《野草》中的第一首散文詩，創作於 1924 年。

## 表格

使用三個或多個連字符 `---` 分隔標題，並使用管道符 `|` 分隔每列，即可創建表格。

### 語法

```markdown
| 斜體   | 粗體     | 程式碼   |
| ----- | -------- | ------- |
| _斜體_ | **粗體** | `程式碼` |
| _斜體_ | **粗體** | `程式碼` |
```

### 效果

| 斜體   | 粗體     | 程式碼   |
| ------ | ------- | ------- |
| _斜體_ | **粗體** | `程式碼` |
| _斜體_ | **粗體** | `程式碼` |

## 程式碼區塊

使用三個反引號 ```` ``` ```` 包裹程式碼，即可創建程式碼區塊。在頂部的反引號後標註語言類型，例如 html、javascript、css、markdown 等，即可實現語法高亮。

### 語法

````
```html
<!doctype html>
<html lang="zh-TW">
  <head>
    <meta charset="utf-8" />
    <title>HTML5 示例文檔</title>
  </head>
  <body>
    <p>測試</p>
  </body>
</html>
```
````

### 效果

```html
<!doctype html>
<html lang="zh-TW">
  <head>
    <meta charset="utf-8" />
    <title>HTML5 示例文檔</title>
  </head>
  <body>
    <p>測試</p>
  </body>
</html>
```

## 列表

### 有序列表

#### 語法

```markdown
1. 第一項
2. 第二項
3. 第三項
```

#### 效果

1. 第一項
2. 第二項
3. 第三項

### 無序列表

#### 語法

```markdown
- 列表項
- 圖表項
- 更多項
```

#### 效果

- 列表項
- 圖表項
- 更多項

### 嵌套列表

#### 語法

```markdown
- 水果
  - 蘋果
  - 橙子
  - 香蕉
- 蔬菜
  - 青菜
  - 蘿蔔
```

#### 效果

- 水果
  - 蘋果
  - 橙子
  - 香蕉
- 蔬菜
  - 青菜
  - 蘿蔔

## 其他元素

包括 `<sup>` 上標，`<sub>` 下標，`<abbr>` 縮寫，`<del>` 刪除線，`<u>` 波浪線，`<kbd>` 鍵盤輸入，`<mark>` 高亮，`<hr>` 分隔線。

### 語法

```html
H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

<abbr title="Graphics Interchange Format">GIF</abbr> 是一種點陣圖圖像格式。

書籍是人類進步的<del>樓梯</del>階梯。

優秀的作家總是會仔細檢查<u title="拼寫">拚寫</u>問題。

按下 <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Delete</kbd> 以結束會話。

大多數<mark>蠑螈</mark>晝伏夜出，以昆蟲、蠕蟲等小生物為食。

使用三個連字符 `---` 或 `<hr>` 標籤，即可創建如下分隔線。

---
```

### 效果

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

<abbr title="Graphics Interchange Format">GIF</abbr> 是一種點陣圖圖像格式。

書籍是人類進步的<del>樓梯</del>階梯。

優秀的作家總是會仔細檢查<u title="拼寫">拚寫</u>問題。

按下 <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Delete</kbd> 以結束會話。

大多數<mark>蠑螈</mark>晝伏夜出，以昆蟲、蠕蟲等小生物為食。

使用三個連字符 `---` 或 `<hr>` 標籤，即可創建如下分隔線。

---
