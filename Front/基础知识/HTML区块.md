# HTML 区块元素

HTML 区块元素 (Block-level Elements) 是指占据页面整行的元素，它们会自动换行，并且可以设置宽度、高度、边距和内边距等属性。

### 常用区块元素

以下是一些常用的 HTML 区块元素：

*   **`<p>` (Paragraph):**  定义段落。
*   **`<h1>` - `<h6>` (Headings):**  定义标题。
*   **`<div>` (Division):**  定义一个通用的块级容器，用于对网页内容进行分组和布局。
*   **`<ul>` / `<ol>` / `<li>` (Lists):**  定义无序列表、有序列表和列表项。
*   **`<dl>` / `<dt>` / `<dd>` (Definition List):**  定义定义列表、术语和定义。
*   **`<table>` (Table):**  定义表格。
*   **`<form>` (Form):**  定义表单。
*   **`<header>` (Header):**  定义文档或节的页眉。
*   **`<footer>` (Footer):**  定义文档或节的页脚。
*   **`<nav>` (Navigation):**  定义导航链接。
*   **`<article>` (Article):**  定义独立的、自包含的内容，例如博客文章或新闻报道。
*   **`<aside>` (Aside):**  定义与主要内容相关的内容，例如侧边栏或脚注。
*   **`<section>` (Section):**  定义文档中的一个节。

### 区块元素的特点

*   **占据整行:** 区块元素会自动换行，占据页面整行的宽度。
*   **可设置宽度和高度:** 可以使用 CSS 来设置区块元素的宽度和高度。
*   **可设置边距和内边距:** 可以使用 CSS 来设置区块元素的边距 (margin) 和内边距 (padding)。

### 区块元素 vs. 行内元素

与区块元素相对的是行内元素 (Inline Elements)，例如 `<span>`、`<a>`、`<strong>` 等等。行内元素只会占据内容所需的宽度，不会自动换行，并且不能设置宽度和高度。

### 示例

```html
<!DOCTYPE html>
<html>
<head>
  <title>Block Elements Example</title>
  <style>
    div {
      background-color: lightblue;
      width: 300px;
      height: 100px;
      margin: 20px;
      padding: 10px;
    }
  </style>
</head>
<body>

  <p>This is a paragraph.</p>

  <div>
    This is a div element.
  </div>

</body>
</html>
```

### 总结

HTML 区块元素是构建网页结构的重要组成部分。了解常用的区块元素及其特点可以帮助你更好地组织和布局网页内容。 

**选择合适的区块元素:**

*   使用 `<p>` 元素来定义段落。
*   使用 `<h1>` - `<h6>` 元素来定义标题。
*   使用 `<div>` 元素来对网页内容进行分组和布局。
*   使用其他的区块元素来定义特定的内容区域，例如页眉、页脚、导航、文章等等。

通过使用 CSS，你可以自定义区块元素的样式，例如背景颜色、宽度、高度、边距、内边距等等，使你的网页更具吸引力。 
