# HTML 表格

HTML 表格用于以表格形式组织和展示数据。它们由行和列组成，可以用于显示各种类型的信息，例如产品列表、价格表、时间表等等。

### 创建表格

HTML 表格使用 `<table>` 标签创建。表格中的每一行使用 `<tr>` 标签表示，每一列使用 `<td>` 标签表示。

**基本语法:**

```html
<table>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

### 表格标题

可以使用 `<th>` 标签来定义表格标题 (表头)。表头通常显示在表格的第一行或第一列。

**示例:**

```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>John Doe</td>
    <td>30</td>
  </tr>
  <tr>
    <td>Jane Doe</td>
    <td>25</td>
  </tr>
</table>
```

### 表格结构

表格可以分为以下几个部分：

*   **表头 (<thead>):**  包含表格的标题行。
*   **表身 (<tbody>):**  包含表格的数据行。
*   **表尾 (<tfoot>):**  包含表格的总结行，例如总计或平均值。

**示例:**

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>John Doe</td>
      <td>30</td>
    </tr>
    <tr>
      <td>Jane Doe</td>
      <td>25</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Total</td>
      <td>55</td>
    </tr>
  </tfoot>
</table>
```

### 单元格跨行和跨列

可以使用 `rowspan` 和 `colspan` 属性来使单元格跨越多行或多列。

*   **`rowspan`:** 指定单元格跨越的行数。
*   **`colspan`:** 指定单元格跨越的列数。

**示例:**

```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td rowspan="2">John Doe</td>
    <td>30</td>
    <td>New York</td>
  </tr>
  <tr>
    <td>25</td>
    <td>London</td>
  </tr>
</table>
```

### 表格标题 (<caption>)

可以使用 `<caption>` 标签来为表格添加标题。标题通常显示在表格的上方。

**示例:**

```html
<table>
  <caption>Employee Information</caption>
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>John Doe</td>
    <td>30</td>
  </tr>
</table>
```

### 表格样式

可以使用 CSS 来控制表格的样式，例如边框、颜色、字体等等。

**示例:**

```css
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  border: 1px solid black;
  padding: 8px;
  text-align: left;
}
```

### 总结

HTML 表格用于以表格形式组织和展示数据。了解表格的基本结构、标题、单元格跨行和跨列、标题和样式可以帮助你创建清晰易懂的表格。 
