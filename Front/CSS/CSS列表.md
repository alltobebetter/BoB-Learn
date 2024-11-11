# CSS 列表

CSS 列表样式允许您自定义网页上列表项的外观，包括项目符号类型、编号类型、位置以及其他与列表相关的特征。

### 列表类型

HTML 中主要有两种类型的列表：

* **无序列表 (`<ul>`):**  用于表示项目没有特定顺序。
* **有序列表 (`<ol>`):** 用于表示项目有特定的顺序。

### 列表样式属性

以下是一些常用的列表样式属性：

* **`list-style-type`:** 设置列表项的项目符号或编号类型。
* **`list-style-image`:** 使用图像作为列表项的项目符号。
* **`list-style-position`:** 设置列表项标记的位置 (inside 或 outside)。
* **`margin`:** 设置列表的外边距。
* **`padding`:** 设置列表的内边距。

### 示例

#### 1. 修改项目符号类型

```css
ul {
  list-style-type: square; /* 使用方形项目符号 */
}
```

#### 2. 使用自定义图像作为项目符号

```css
ul {
  list-style-image: url('images/bullet.png'); 
}
```

#### 3. 将项目符号放置在列表项内部

```css
ul {
  list-style-position: inside;
}
```

#### 4. 修改有序列表的编号类型

```css
ol {
  list-style-type: lower-roman; /* 使用小写罗马数字 */
}
```

#### 5. 移除列表项的默认样式

```css
ul, ol {
  list-style: none; /* 移除项目符号或编号 */
  margin: 0; /* 移除默认外边距 */
  padding: 0; /* 移除默认内边距 */
}
```

#### 6. 创建自定义列表样式

```css
ul {
  list-style: none;
  padding: 0;
}

li {
  padding-left: 20px;
  position: relative;
}

li::before {
  content: "-";
  position: absolute;
  left: 0;
}
```

这个例子创建了一个自定义的无序列表，使用 "-" 符号作为项目符号，并将其放置在列表项的左侧。

### 总结

使用 CSS 可以轻松地自定义列表的样式，以匹配您的网站设计。 通过使用不同的列表样式属性，您可以创建各种各样的列表效果，提高网站的用户体验。 
