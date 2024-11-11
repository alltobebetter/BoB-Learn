# CSS 表格

CSS 表格样式允许您自定义网页上表格的外观，包括边框、颜色、间距、对齐方式等。

### 表格元素

HTML 表格由以下元素组成：

* `<table>`: 定义表格。
* `<tr>`: 定义表格行。
* `<td>`: 定义表格单元格（数据）。
* `<th>`: 定义表头单元格。
* `<caption>`: 定义表格标题。

### 表格样式属性

以下是一些常用的表格样式属性：

* **`border`:** 设置表格和单元格的边框。
* **`border-collapse`:** 设置表格边框的合并方式 (`collapse` 或 `separate`)。
* **`border-spacing`:** 设置相邻单元格之间的距离 (仅在 `border-collapse` 设置为 `separate` 时有效)。
* **`width`:** 设置表格的宽度。
* **`height`:** 设置表格的高度。
* **`padding`:** 设置单元格的内边距。
* **`text-align`:** 设置单元格中文本的对齐方式。
* **`vertical-align`:** 设置单元格中文本的垂直对齐方式。
* **`background-color`:** 设置表格或单元格的背景颜色。
* **`color`:** 设置单元格中文本的颜色。

### 示例

#### 1. 设置表格边框

```css
table {
  border: 1px solid black;
  border-collapse: collapse; /* 合并边框 */
}

td, th {
  border: 1px solid black;
  padding: 8px;
}
```

#### 2. 设置表格宽度和高度

```css
table {
  width: 100%;
  height: 300px;
}
```

#### 3. 设置单元格文本对齐方式

```css
td {
  text-align: center;
  vertical-align: middle;
}
```

#### 4. 设置表头样式

```css
th {
  background-color: #f2f2f2;
  font-weight: bold;
}
```

#### 5. 隔行变色

```css
tr:nth-child(even) {
  background-color: #f2f2f2;
}
```

#### 6. 鼠标悬停效果

```css
tr:hover {
  background-color: #ddd;
}
```

### 总结

使用 CSS 可以轻松地自定义表格的样式，以匹配您的网站设计。 通过使用不同的表格样式属性，您可以创建各种各样的表格效果，提高网站的用户体验和可读性。 

希望以上信息对您有所帮助! 
