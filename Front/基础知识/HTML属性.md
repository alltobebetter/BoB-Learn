# HTML 属性

HTML 属性为 HTML 元素提供附加信息。它们通常以名称/值对的形式出现，例如 `name="value"`，并且写在开始标签内。属性可以修改元素的行为或提供有关元素的元数据。

### 属性的通用语法

属性在 HTML 元素的开始标签中指定，格式如下：

```html
<elementName attributeName="attributeValue"> element content </elementName> 
```

*   `elementName` 是 HTML 元素的名称。
*   `attributeName` 是属性的名称。
*   `attributeValue` 是属性的值，用双引号或单引号括起来。

### 常见的 HTML 属性

#### 1.  `id`

*   作用：为元素定义唯一的标识符。
*   用法：`<element id="uniqueId">`
*   示例：`<p id="intro">This is an introductory paragraph.</p>`

#### 2.  `class`

*   作用：为元素分配一个或多个类名，用于 CSS 样式和 JavaScript 操作。
*   用法：`<element class="className1 className2">`
*   示例：`<div class="container main">This is a div with two classes.</div>`

#### 3. `style`

*   作用：为元素添加内联样式。
*   用法：`<element style="property:value; property:value;">`
*   示例：`<p style="color:blue; font-size:16px;">This paragraph has blue text and a font size of 16 pixels.</p>`

#### 4.  `title`

*   作用：为元素提供额外的信息，通常以工具提示的形式显示。
*   用法：`<element title="tooltip text">`
*   示例：`<a href="#" title="Learn more">Click here</a>`

#### 5.  `src`

*   作用：指定图像、视频或其他外部资源的 URL。
*   用法：`<img src="image.jpg">` 或 `<video src="video.mp4">`
*   示例：`<img src="images/logo.png" alt="Company Logo">`

#### 6. `href`

*   作用：指定链接的目标 URL。
*   用法：`<a href="url">link text</a>`
*   示例：`<a href="https://www.example.com">Visit Example</a>`

#### 7.  `alt`

*   作用：为图像提供替代文本，当图像无法显示时显示。
*   用法：`<img src="image.jpg" alt="alternative text">`
*   示例：`<img src="images/product.jpg" alt="Product Image">`

#### 8. `width` 和 `height`

*   作用：指定图像或其他元素的宽度和高度。
*   用法：`<img src="image.jpg" width="300" height="200">`
*   示例：`<iframe width="560" height="315" src="https://www.youtube.com/embed/xxxxxxxx" title="YouTube video player" frameborder="0"></iframe>`

#### 9. `disabled`

*   作用：禁用表单元素，使其无法交互。
*   用法：`<input type="text" disabled>`
*   示例：`<button type="submit" disabled>Submit</button>`


### 属性的分类

HTML 属性可以根据其功能和作用范围进行分类：

*   **全局属性**:  可以在所有 HTML 元素上使用的属性，例如 `id`、`class`、`style`、`title` 等。
*   **特定属性**: 仅适用于特定 HTML 元素的属性，例如 `src` 适用于 `<img>` 和 `<video>` 元素，`href` 适用于 `<a>` 元素等。
*   **事件属性**:  用于处理用户交互事件的属性，例如 `onclick`、`onmouseover`、`onsubmit` 等。

### 总结

HTML 属性为 HTML 元素提供了丰富的功能和控制能力。理解和使用 HTML 属性是创建结构良好、功能强大的网页的关键。
