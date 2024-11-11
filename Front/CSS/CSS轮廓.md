# CSS 边框

CSS 边框属性允许您自定义 HTML 元素的边框样式、宽度、颜色等。您可以为元素的每个边设置不同的边框，或者为所有边设置相同的边框。


### 边框样式属性

以下是一些常用的边框样式属性：

* **`border-width`:** 设置边框的宽度。 可以使用像素 (px)、em、百分比 (%) 等单位。
* **`border-style`:** 设置边框的样式。 常用的样式包括 `solid` (实线)、`dotted` (点线)、`dashed` (虚线)、`double` (双线)、`groove` (凹槽)、`ridge` (凸脊)、`inset` (内嵌) 和 `outset` (外凸)。
* **`border-color`:** 设置边框的颜色。 可以使用颜色名称、十六进制代码、RGB 值等。

### 简写属性

`border` 属性是一个简写属性，可以同时设置 `border-width`、`border-style` 和 `border-color`。

#### 示例：

```css
p {
  border: 2px solid red; /* 设置边框为 2px 宽的红色实线 */
}
```


### 单边边框

您可以使用 `border-top`、`border-right`、`border-bottom` 和 `border-left` 属性分别设置元素的四个边的边框。

#### 示例：

```css
div {
  border-top: 1px solid blue;
  border-right: 2px dashed green;
  border-bottom: 3px dotted yellow;
  border-left: 4px double orange;
}
```

### 圆角边框

`border-radius` 属性可以用来创建圆角边框。

#### 示例：

```css
button {
  border: 2px solid gray;
  border-radius: 5px; /* 设置圆角半径为 5px */
}
```

### 边框图片

`border-image` 属性可以用来使用图片作为边框。

#### 示例：

```css
div {
  border-image: url("border.png") 30 30 round;
}
```

### 边框阴影

`box-shadow` 属性可以用来为元素添加阴影效果。

#### 示例：

```css
h1 {
  box-shadow: 2px 2px 5px gray;
}
```

### 总结

CSS 边框属性提供了丰富的功能来定制元素的边框样式。 通过使用不同的边框属性，您可以创建各种各样的边框效果，使您的网页设计更加丰富多彩。
