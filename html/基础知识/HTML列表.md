# HTML 列表

HTML 列表用于以列表形式组织和展示信息。HTML 提供了三种类型的列表：

*   **无序列表 (Unordered List):** 列表项没有顺序，通常使用项目符号标记。
*   **有序列表 (Ordered List):** 列表项有顺序，通常使用数字或字母标记。
*   **定义列表 (Definition List):**  包含一系列术语及其定义。

### 无序列表 (Unordered List)

无序列表使用 `<ul>` 标签创建，列表项使用 `<li>` 标签表示。

**基本语法:**

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

### 有序列表 (Ordered List)

有序列表使用 `<ol>` 标签创建，列表项使用 `<li>` 标签表示。

**基本语法:**

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

### 定义列表 (Definition List)

定义列表使用 `<dl>` 标签创建，术语使用 `<dt>` 标签表示，定义使用 `<dd>` 标签表示。

**基本语法:**

```html
<dl>
  <dt>Term 1</dt>
  <dd>Definition 1</dd>
  <dt>Term 2</dt>
  <dd>Definition 2</dd>
</dl>
```

### 嵌套列表

列表可以嵌套，例如在一个无序列表中嵌套一个有序列表。

**示例:**

```html
<ul>
  <li>Item 1</li>
  <li>Item 2
    <ol>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ol>
  </li>
  <li>Item 3</li>
</ul>
```

### 列表样式

可以使用 CSS 来控制列表的样式，例如项目符号类型、数字类型、缩进等等。

**示例:**

```css
ul {
  list-style-type: square; /* 设置项目符号类型为方形 */
}

ol {
  list-style-type: upper-roman; /* 设置数字类型为大写罗马数字 */
}

li {
  margin-left: 20px; /* 设置缩进 */
}
```

### 总结

HTML 列表用于以列表形式组织和展示信息。了解无序列表、有序列表和定义列表，以及嵌套列表和列表样式，可以帮助你创建清晰易懂的列表。 

**选择合适的列表类型取决于你想要表达的信息类型:**

*   **无序列表:** 适用于没有顺序的项目。
*   **有序列表:** 适用于有顺序的项目。
*   **定义列表:** 适用于术语及其定义。 

通过使用 CSS，你可以自定义列表的样式，使其更符合你的网页设计风格。 
