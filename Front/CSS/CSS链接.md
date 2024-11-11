# CSS 链接

CSS 链接样式允许您自定义网页上链接的外观，包括颜色、下划线、悬停效果等。

### 链接状态

链接有四个不同的状态：

* **link:**  未访问过的链接
* **visited:** 访问过的链接
* **hover:** 鼠标悬停在链接上
* **active:** 链接被点击的瞬间

可以使用 CSS 的伪类选择器来针对这些不同的状态设置样式。

### 链接样式属性

以下是一些常用的链接样式属性：

* **`color`:** 设置链接的颜色。
* **`text-decoration`:** 设置链接的装饰，例如下划线 (`underline`)、上划线 (`overline`)、删除线 (`line-through`) 或无装饰 (`none`)。
* **`background-color`:** 设置链接的背景颜色。
* **`font-weight`:** 设置链接的字体粗细，例如 `normal`、`bold` 等。
* **`font-style`:** 设置链接的字体样式，例如 `normal`、`italic` 等。
* **`border`:** 设置链接的边框。
* **`padding`:** 设置链接的内边距。
* **`margin`:** 设置链接的外边距。

### 示例

#### 1. 基本链接样式

```css
a:link {
  color: blue;
  text-decoration: underline;
}

a:visited {
  color: purple;
  text-decoration: underline;
}

a:hover {
  color: red;
  text-decoration: none;
}

a:active {
  color: orange;
  text-decoration: underline;
}
```

这个例子设置了未访问链接为蓝色下划线，访问过的链接为紫色下划线，鼠标悬停时为红色无下划线，点击时为橙色下划线。

#### 2. 移除下划线

```css
a {
  text-decoration: none;
}
```

这个例子移除了所有链接的下划线。

#### 3. 添加背景颜色

```css
a:hover {
  background-color: yellow;
}
```

这个例子在鼠标悬停时为链接添加黄色背景。

#### 4. 使用类选择器

```css
a.button {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a.button:hover {
  background-color: #3e8e41;
}
```

这个例子为类名为 "button" 的链接设置了按钮样式，包括背景颜色、颜色、内边距、文本对齐、移除下划线和设置为块级元素。 鼠标悬停时，背景颜色会改变。


### 总结

使用 CSS 可以轻松地自定义链接的样式，以匹配您的网站设计。 通过使用不同的伪类选择器和样式属性，您可以创建各种各样的链接效果，提高网站的用户体验。
