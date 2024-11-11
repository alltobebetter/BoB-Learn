# HTML 图像

HTML 使用 `<img>` 标签来插入图像。`<img>` 是一个自闭合标签，这意味着它没有结束标签。

### 基本语法

```html
<img src="image.jpg" alt="Alternative text">
```

*   **`src` 属性**:  指定图像文件的 URL。可以是绝对 URL 或相对 URL。
*   **`alt` 属性**:  指定图像的替代文本。当图像无法显示时，替代文本会显示在图像的位置。替代文本也有利于 SEO 和网页的可访问性。

### 示例

```html
<img src="images/logo.png" alt="Company Logo">
```

### 图像格式

常见的图像格式包括：

*   **JPEG (`.jpg` 或 `.jpeg`):**  适用于照片和复杂的图像，支持有损压缩。
*   **PNG (`.png`):**  适用于图标、图形和需要透明背景的图像，支持无损压缩。
*   **GIF (`.gif`):**  适用于动画和简单的图形，支持无损压缩和透明背景。
*   **SVG (`.svg`):**  适用于矢量图形，可以无限缩放而不失真。

### 图像尺寸

可以使用 `width` 和 `height` 属性来指定图像的宽度和高度。

**示例:**

```html
<img src="image.jpg" alt="Image" width="300" height="200">
```

**注意:** 

*   如果只指定 `width` 或 `height`，浏览器会自动调整另一个维度以保持图像的纵横比。
*   建议使用 CSS 来控制图像尺寸，以便更好地控制图像的布局和响应式设计。

### 响应式图像

为了使图像在不同尺寸的屏幕上都能良好地显示，可以使用 `srcset` 和 `sizes` 属性来指定不同尺寸的图像文件。

**示例:**

```html
<img src="image.jpg" 
     alt="Image" 
     srcset="image-small.jpg 300w, image-medium.jpg 600w, image-large.jpg 900w" 
     sizes="(max-width: 600px) 100vw, (max-width: 900px) 50vw, 33vw">
```

*   **`srcset` 属性**:  指定不同尺寸的图像文件和它们的宽度。
*   **`sizes` 属性**:  指定浏览器应该根据屏幕宽度选择哪个图像文件。

### 图片地图

图片地图允许你在图像的不同区域定义可点击的链接。

**示例:**

```html
<img src="image.jpg" alt="Image Map" usemap="#mymap">

<map name="mymap">
  <area shape="rect" coords="0,0,100,100" href="link1.html" alt="Link 1">
  <area shape="circle" coords="200,200,50" href="link2.html" alt="Link 2">
</map>
```

*   **`<map>` 元素**:  定义图片地图。
*   **`<area>` 元素**:  定义图片地图中的可点击区域。

### 总结

HTML 图像是网页的重要组成部分，可以使用 `<img>` 标签来插入图像。了解图像格式、尺寸、响应式图像和图片地图可以帮助你创建更丰富、更具吸引力的网页。
