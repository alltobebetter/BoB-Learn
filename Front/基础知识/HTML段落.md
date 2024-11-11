# HTML 段落

在 HTML 中，`<p>` 标签用于定义段落。段落是网页内容的基本组成部分，用于组织和呈现文本信息。

### 语法

HTML 段落的语法如下：

```html
<p>This is a paragraph of text.</p>
```

### 示例

```html
<!DOCTYPE html>
<html>
<head>
  <title>HTML Paragraphs</title>
</head>
<body>

  <p>This is the first paragraph.</p>
  <p>This is the second paragraph.</p>

</body>
</html>
```

### 段落格式化

浏览器会自动在段落之间添加垂直间距。可以通过 CSS 样式来进一步控制段落的格式，例如：

*   `text-align`: 设置段落的水平对齐方式，例如左对齐、居中对齐或右对齐。
*   `line-height`: 设置段落的行高。
*   `margin`: 设置段落的边距。
*   `padding`: 设置段落的内边距。
*   `font-size`: 设置段落的字体大小。
*   `font-family`: 设置段落的字体。
*   `color`: 设置段落的文本颜色。

### 示例 (CSS 格式化)

```html
<!DOCTYPE html>
<html>
<head>
  <title>HTML Paragraphs with CSS</title>
  <style>
    p {
      text-align: justify;
      line-height: 1.5;
      margin: 20px;
      padding: 10px;
      font-size: 16px;
      font-family: sans-serif;
      color: #333;
    }
  </style>
</head>
<body>

  <p>This is a paragraph with custom CSS formatting.</p>

</body>
</html>
```

### 其他文本格式化标签

除了 `<p>` 标签之外，HTML 还提供了一些其他的文本格式化标签，例如：

*   `<b>` 和 `<strong>`: 用于加粗文本。
*   `<i>` 和 `<em>`: 用于斜体文本。
*   `<br>`: 用于插入换行符。
*   `<pre>`: 用于预格式化文本，保留空格和换行符。

### 总结

HTML 段落是网页内容的基本组成部分，用于组织和呈现文本信息。可以使用 CSS 样式来控制段落的格式，例如对齐方式、行高、边距、字体大小和颜色等。
