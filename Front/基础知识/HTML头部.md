# HTML 头部 `<head>`

HTML 头部 `<head>` 元素包含了关于 HTML 文档的元信息，例如字符集、标题、样式表链接、脚本链接等等。这些信息不会直接显示在网页上，但对浏览器解析和渲染网页至关重要，也对搜索引擎优化 (SEO) 有重要影响。

### `<head>` 元素的内容

`<head>` 元素通常包含以下内容：

1.  **`<title>` 元素**: 定义 HTML 文档的标题，显示在浏览器窗口的标题栏或标签页上。
2.  **`<meta>` 元素**: 提供关于 HTML 文档的元数据，例如字符集、作者、描述、关键词等等。
3.  **`<link>` 元素**: 用于链接外部资源，例如样式表文件 (CSS)、图标文件 (favicon) 等等。
4.  **`<style>` 元素**: 包含内部样式表定义。
5.  **`<script>` 元素**: 包含 JavaScript 代码或链接外部 JavaScript 文件。
6.  **`<base>` 元素**:  指定文档中所有相对 URL 的基准 URL。
7.  **`<noscript>` 元素**:  定义在浏览器不支持 JavaScript 或禁用 JavaScript 时显示的内容。

### `<head>` 元素示例

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Website</title>
  <link rel="stylesheet" href="styles.css">
  <script src="script.js"></script>
</head>
<body>
  </body>
</html>
```

### 重要元素详解

#### 1. `<title>` 元素

`<title>` 元素定义 HTML 文档的标题，对 SEO 非常重要。

*   每个 HTML 文档都应该有一个 `<title>` 元素。
*   标题应该简洁明了地描述网页的内容。
*   标题应该包含关键词，以便搜索引擎能够理解网页的主题。

**示例:**

```html
<title>My Awesome Website - Learn About Web Development</title>
```

#### 2. `<meta>` 元素

`<meta>` 元素提供关于 HTML 文档的元数据，例如字符集、作者、描述、关键词等等。

*   `charset` 属性:  指定文档的字符编码，例如 `UTF-8`。
*   `name` 属性:  指定元数据的名称，例如 `author`、`description`、`keywords` 等等。
*   `content` 属性:  指定元数据的值。

**示例:**

```html
<meta charset="UTF-8">
<meta name="author" content="John Doe">
<meta name="description" content="This is a website about web development.">
<meta name="keywords" content="HTML, CSS, JavaScript, Web Development">
```

#### 3. `<link>` 元素

`<link>` 元素用于链接外部资源，例如样式表文件 (CSS)、图标文件 (favicon) 等等。

*   `rel` 属性:  指定链接的类型，例如 `stylesheet` (样式表)、`icon` (图标) 等等。
*   `href` 属性:  指定外部资源的 URL。

**示例:**

```html
<link rel="stylesheet" href="styles.css">
<link rel="icon" href="favicon.ico">
```

### 总结

HTML 头部 `<head>` 元素包含了关于 HTML 文档的重要元信息，对浏览器解析、渲染和 SEO 都有重要影响。了解 `<head>` 元素及其常用子元素可以帮助你创建更规范、更易于搜索引擎理解的网页。
