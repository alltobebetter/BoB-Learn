# CSS 填充 (Padding)

CSS 填充 (padding) 属性用于控制元素内容与其边框之间的空白区域。 填充会增加元素的尺寸，并且填充区域会被元素的背景颜色或图像填充。

### 填充属性

可以使用以下属性来设置元素的填充：

* **`padding-top`:** 设置元素的上填充。
* **`padding-right`:** 设置元素的右填充。
* **`padding-bottom`:** 设置元素的下填充。
* **`padding-left`:** 设置元素的左填充。
* **`padding`:** 简写属性，可以同时设置所有四个方向的填充。

### 填充取值

填充属性可以接受以下几种类型的取值：

* **长度值:** 例如 `10px`、`2em`、`5%` 等。
* **`auto`:** 浏览器会自动计算填充的值。 很少使用。

### 简写属性 `padding`

`padding` 属性可以同时设置所有四个方向的填充。

#### 示例：

```css
p {
  padding: 10px; /* 所有方向的填充都设置为 10px */
}

div {
  padding: 20px 10px; /* 上下填充为 20px，左右填充为 10px */
}

h1 {
  padding: 5px 10px 15px 20px; /* 上填充为 5px，右填充为 10px，下填充为 15px，左填充为 20px */
}
```

### 填充与元素尺寸

填充会增加元素的尺寸。 例如，如果一个元素的内容宽度为 100px，并且设置了左右填充各为 10px，那么元素的总宽度将是 120px。

### `box-sizing` 属性

`box-sizing` 属性可以用来改变盒子模型的计算方式，从而影响填充对元素尺寸的影响。

* **`content-box`:** 默认值。 元素的总宽度和高度是内容宽度、填充、边框和外边距的总和。
* **`border-box`:** 元素的总宽度和高度包括内容宽度、填充和边框，但不包括外边距。

#### 示例：

```css
div {
  width: 100px;
  padding: 10px;
  box-sizing: border-box; /* 使用 border-box 模型 */
}
```

在这个例子中，即使设置了填充，div 元素的总宽度仍然是 100px，因为使用了 `border-box` 模型。

### 示例

#### 1. 设置段落的填充

```css
p {
  padding-top: 20px;
  padding-left: 10px;
}
```

#### 2. 使用填充创建按钮样式

```css
button {
  padding: 10px 20px;
  background-color: #4CAF50;
  color: white;
  border: none;
}
```


### 总结

CSS 填充属性是控制网页布局的重要工具。 通过合理设置填充，可以控制元素内容与其边框之间的距离，创建出美观且易于维护的网页布局。 
