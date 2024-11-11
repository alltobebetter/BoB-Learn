# CSS 背景 (Background)

CSS 背景属性用于控制 HTML 元素的背景颜色、图像、重复方式、位置等等。

### 背景颜色 (background-color)

`background-color` 属性用于设置元素的背景颜色。

**语法:**

```css
background-color: color;
```

*   `color`: 可以是颜色名称、RGB 值、十六进制颜色码等等。

**示例:**

```css
body {
  background-color: lightblue;
}

.container {
  background-color: rgb(255, 255, 0); 
}

#header {
  background-color: #f0f0f0;
}
```

### 背景图像 (background-image)

`background-image` 属性用于设置元素的背景图像。

**语法:**

```css
background-image: url("image.jpg");
```

*   `url("image.jpg")`: 指定图像文件的 URL。

**示例:**

```css
body {
  background-image: url("images/background.png");
}
```

### 背景重复 (background-repeat)

`background-repeat` 属性用于控制背景图像的重复方式。

**值:**

*   `repeat`:  水平和垂直方向都重复 (默认值)。
*   `repeat-x`:  只在水平方向重复。
*   `repeat-y`:  只在垂直方向重复。
*   `no-repeat`:  不重复。

**示例:**

```css
body {
  background-image: url("images/pattern.png");
  background-repeat: repeat-x;
}
```

### 背景位置 (background-position)

`background-position` 属性用于设置背景图像的位置。

**值:**

*   可以使用关键词，例如 `top`、`bottom`、`left`、`right`、`center` 等等。
*   可以使用百分比或像素值来精确定位。

**示例:**

```css
body {
  background-image: url("images/logo.png");
  background-repeat: no-repeat;
  background-position: top right; 
}

.container {
  background-image: url("images/icon.png");
  background-repeat: no-repeat;
  background-position: 10px 20px; 
}
```

### 背景附着 (background-attachment)

`background-attachment` 属性用于控制背景图像是否随页面滚动而滚动。

**值:**

*   `scroll`:  背景图像随页面滚动而滚动 (默认值)。
*   `fixed`:  背景图像固定在视口中，不随页面滚动而滚动。

**示例:**

```css
body {
  background-image: url("images/stars.jpg");
  background-repeat: no-repeat;
  background-attachment: fixed;
}
```

### 背景简写 (background)

`background` 属性可以将多个背景属性合并为一个简写属性。

**语法:**

```css
background: color image repeat attachment position;
```

**示例:**

```css
body {
  background: lightblue url("images/background.png") no-repeat fixed center;
}
```

### 背景尺寸 (background-size)

`background-size` 属性用于控制背景图像的尺寸。

**值:**

*   `auto`:  使用图像的原始尺寸 (默认值)。
*   `cover`:  缩放图像以完全覆盖元素，可能会裁剪图像。
*   `contain`:  缩放图像以完整显示在元素内，可能会留白。
*   可以使用百分比或像素值来指定具体的宽度和高度。

**示例:**

```css
.container {
  background-image: url("images/hero.jpg");
  background-size: cover;
}
```

### 总结

CSS 背景属性可以帮助你创建丰富多彩的网页背景效果。通过灵活运用这些属性，你可以自定义背景颜色、图像、重复方式、位置、尺寸等等，使你的网页更具吸引力。
