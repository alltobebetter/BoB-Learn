# CSS 基础语法

CSS (Cascading Style Sheets) 是一种用于描述网页样式的语言，它可以控制网页的布局、颜色、字体等等。

### CSS 规则

CSS 规则由两部分组成：**选择器**和**声明块**。

**语法:**

```css
selector {
  property1: value1;
  property2: value2;
  /* ... */
}
```

*   **选择器**:  用于选择要应用样式的 HTML 元素。
*   **声明块**:  包含一个或多个声明，每个声明由一个属性和一个值组成。
*   **属性**:  指定要修改的样式属性，例如 `color` (颜色)、`font-size` (字体大小) 等等。
*   **值**:  指定属性的值，例如 `red` (红色)、`16px` (16 像素) 等等。

### CSS 选择器

CSS 选择器用于选择要应用样式的 HTML 元素。以下是几种常见的 CSS 选择器：

*   **元素选择器**:  根据元素名称选择元素。

```css
p {
  color: blue;
}
```

*   **类选择器**:  根据元素的 class 属性选择元素。

```css
.highlight {
  background-color: yellow;
}
```

*   **ID 选择器**:  根据元素的 id 属性选择元素。

```css
#intro {
  font-size: 20px;
}
```

*   **通配符选择器**:  选择所有元素。

```css
* {
  margin: 0;
  padding: 0;
}
```

### CSS 注释

CSS 注释用于解释代码，注释内容不会被浏览器解析。

**语法:**

```css
/* 这是一个 CSS 注释 */
```

### CSS 单位

CSS 属性的值可以使用不同的单位，例如：

*   **像素 (px)**:  绝对长度单位。
*   **百分比 (%)**:  相对于父元素的长度单位。
*   **em**:  相对于当前字体大小的长度单位。
*   **rem**:  相对于根元素字体大小的长度单位。

### CSS 颜色

CSS 颜色可以使用多种方式指定，例如：

*   **颜色名称**:  例如 `red`、`blue`、`green` 等等。
*   **RGB 值**:  例如 `rgb(255, 0, 0)` (红色)。
*   **十六进制颜色码**:  例如 `#ff0000` (红色)。

### CSS 示例

```html
<!DOCTYPE html>
<html>
<head>
  <title>CSS Example</title>
  <style>
    p {
      color: blue;
      font-size: 16px;
    }

    .highlight {
      background-color: yellow;
    }

    #intro {
      font-size: 20px;
    }
  </style>
</head>
<body>

  <p>This is a paragraph.</p>
  <p class="highlight">This is a highlighted paragraph.</p>
  <p id="intro">This is an introductory paragraph.</p>

</body>
</html>
```

### 总结

CSS 基础语法包括选择器、声明块、属性、值、注释和单位。掌握这些基础知识可以帮助你开始使用 CSS 来美化网页。 
