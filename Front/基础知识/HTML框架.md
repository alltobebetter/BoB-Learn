# HTML 框架 (Frames)

HTML 框架 (Frames) 是一种将网页分割成多个独立区域的技术，每个区域可以显示不同的 HTML 文档。框架主要使用 `<iframe>` 标签实现。

## `<iframe>` 标签

`<iframe>` 标签用于创建一个内联框架，可以在当前 HTML 文档中嵌入另一个 HTML 文档。

**基本语法:**

```html
<iframe src="URL" title="description"></iframe>
```

*   **`src` 属性:**  指定要嵌入的 HTML 文档的 URL。
*   **`title` 属性:**  提供框架内容的描述，对可访问性很重要。

**示例:**

```html
<iframe src="https://www.example.com" title="Example Website"></iframe>
```

## `<iframe>` 标签的常用属性

*   **`width` 和 `height`:**  设置框架的宽度和高度，可以使用像素或百分比。
*   **`frameborder`:**  设置框架的边框，`0` 表示无边框，`1` 表示有边框 (默认值)。
*   **`scrolling`:**  设置框架是否显示滚动条，`yes` 表示显示滚动条，`no` 表示不显示滚动条，`auto` 表示自动 (默认值)。
*   **`allowfullscreen`:**  允许框架内容全屏显示。
*   **`sandbox`:**  启用沙盒模式，限制框架内容的权限，例如禁止脚本执行、禁止表单提交等等。


## 框架的优缺点

**优点:**

*   可以将不同的内容整合到一个页面中。
*   可以方便地加载外部网站的内容。

**缺点:**

*   不利于 SEO，因为搜索引擎可能无法正确索引框架中的内容。
*   可能会导致用户体验下降，例如导航混乱、加载速度变慢等等。
*   在移动设备上显示效果不佳。

## 框架的应用场景

*   嵌入第三方网站的内容，例如地图、视频、社交媒体插件等等。
*   创建 Web 应用程序的界面，例如将不同的功能模块分割成不同的框架。


## 替代方案

现在，更推荐使用 CSS 布局和 JavaScript 来实现类似框架的功能，例如使用 `<div>` 元素和 CSS `position` 属性来创建布局，使用 AJAX 来加载外部内容等等。

## 示例

```html
<!DOCTYPE html>
<html>
<head>
  <title>Iframe Example</title>
</head>
<body>

  <h1>My Website</h1>

  <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3784134.153665218!2d-96.82516112131725!3d39.53675982824274!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x880b2d386f6e2619%3A0x7f158250680844e!2sUnited%20States!5e0!3m2!1sen!2s!4v1678884784105!5m2!1sen!2s" 
          width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

</body>
</html>
```


## 总结

HTML 框架可以使用 `<iframe>` 标签来实现，它允许你在当前 HTML 文档中嵌入另一个 HTML 文档。框架有一定的优缺点，现在更推荐使用 CSS 布局和 JavaScript 来实现类似的功能。 
