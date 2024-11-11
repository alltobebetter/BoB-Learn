# CSS 字体

CSS 字体属性用于定义文本的字体系列、大小、样式、粗细和其他与字体相关的特征。

### 1. 字体系列 (`font-family`)

`font-family` 属性指定了用于显示文本的字体系列。 可以指定多个字体系列，浏览器会按照顺序尝试使用，直到找到可用的字体。

#### 示例:

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}
```

在这个例子中，浏览器会首先尝试使用 Arial 字体。 如果 Arial 字体不可用，它会尝试使用 Helvetica，最后尝试使用 sans-serif 通用字体系列。

### 2. 字体大小 (`font-size`)

`font-size` 属性设置字体的大小。 可以使用多种单位，例如像素 (px)、em、百分比 (%) 等。

#### 示例:

```css
h1 {
  font-size: 36px;
}

p {
  font-size: 1.2em;
}
```

### 3. 字体样式 (`font-style`)

`font-style` 属性指定字体的样式，例如正常、斜体或倾斜。

#### 示例:

```css
em {
  font-style: italic;
}

cite {
  font-style: oblique;
}
```

### 4. 字体粗细 (`font-weight`)

`font-weight` 属性指定字体的粗细。 可以使用预定义的关键字，例如 normal、bold、bolder、lighter，或者使用数值 (100-900)。

#### 示例:

```css
strong {
  font-weight: bold;
}

h2 {
  font-weight: 700;
}
```

### 5. 字体变体 (`font-variant`)

`font-variant` 属性用于指定小型大写字母的变体。

#### 示例:

```css
p.small-caps {
  font-variant: small-caps;
}
```

### 6. 字体简写 (`font`)

`font` 属性是一个简写属性，可以同时设置多个字体属性，例如 `font-style`、`font-variant`、`font-weight`、`font-size` 和 `font-family`。

#### 示例:

```css
body {
  font: italic small-caps bold 16px/1.5 Arial, sans-serif;
}
```

这个例子设置了字体样式为斜体、小型大写字母、粗体，字体大小为 16 像素，行高为 1.5，字体系列为 Arial 和 sans-serif。

### 7. Web Fonts

Web Fonts 允许您在网页上使用自定义字体，而无需依赖用户的计算机上是否安装了这些字体。 可以使用 `@font-face` 规则来定义 Web Fonts。

#### 示例:

```css
@font-face {
  font-family: 'MyCustomFont';
  src: url('mycustomfont.woff2') format('woff2'),
       url('mycustomfont.woff') format('woff');
}

body {
  font-family: 'MyCustomFont', sans-serif;
}
```

### 总结

CSS 字体属性提供了丰富的功能来控制文本的字体样式，使您可以创建具有独特外观和风格的网页。 使用 Web Fonts 可以进一步扩展您的选择，并使您的网页设计更加灵活和多样化。 
