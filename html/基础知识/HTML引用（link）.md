# HTML 引用 (Link) - `<link>` 标签

HTML `<link>` 标签用于定义当前文档与外部资源之间的关系。它最常用于链接外部样式表 (CSS)，但也常用于链接其他类型的资源，例如图标 (favicon)、预加载资源、RSS feeds 等等。

### 基本语法

```html
<link rel="relationship" href="URL">
```

*   **`rel` 属性:**  指定链接的类型，例如 `stylesheet` (样式表)、`icon` (图标) 等等。
*   **`href` 属性:**  指定外部资源的 URL。

### 常用的 `rel` 属性值

*   **`stylesheet`:**  链接外部样式表。
*   **`icon`:**  链接图标文件，例如 favicon。
*   **`preconnect`:**  提前建立与外部服务器的连接，加快页面加载速度。
*   **`dns-prefetch`:**  提前解析外部服务器的域名，加快页面加载速度。
*   **`preload`:**  预加载重要的资源，例如字体文件、图片等等。
*   **`alternate`:**  指定替代版本的文档，例如 RSS feed、打印版本等等。

### 示例

#### 1. 链接外部样式表

```html
<link rel="stylesheet" href="style.css">
```

#### 2. 链接 favicon

```html
<link rel="icon" href="favicon.ico" type="image/x-icon">
```

#### 3. 预加载字体文件

```html
<link rel="preload" href="fonts/myfont.woff2" as="font" type="font/woff2" crossorigin>
```

#### 4. 指定 RSS feed

```html
<link rel="alternate" type="application/rss+xml" title="My Blog RSS Feed" href="/feed.xml">
```

### `<link>` 标签的放置位置

`<link>` 标签通常放置在 HTML 文档的 `<head>` 部分内部。

### 总结

HTML `<link>` 标签用于定义当前文档与外部资源之间的关系。它最常用于链接外部样式表，但也常用于链接其他类型的资源，例如图标、预加载资源、RSS feeds 等等。了解常用的 `rel` 属性值可以帮助你更好地利用 `<link>` 标签来优化你的网页。


**注意:** 

*   `<link>` 标签是一个自闭合标签，不需要结束标签。
*   `<link>` 标签的属性值应该用双引号或单引号括起来。
