# CSS Display 与 Visibility

CSS 的 `display` 和 `visibility` 属性都用于控制元素的可见性，但它们的工作方式有所不同。

### Display 属性

`display` 属性用于控制元素的显示类型，它不仅可以隐藏元素，还可以改变元素的布局方式。

#### 常用取值

* **`none`:** 隐藏元素，并且元素不占据任何空间。
* **`block`:** 将元素显示为块级元素，独占一行，可以设置宽度和高度。
* **`inline`:** 将元素显示为行内元素，与其他行内元素在一行显示，不能设置宽度和高度。
* **`inline-block`:** 将元素显示为行内块级元素，可以设置宽度和高度，并且与其他行内元素在一行显示。
* **`flex`:** 将元素显示为弹性容器，用于弹性布局。
* **`grid`:** 将元素显示为网格容器，用于网格布局。
* **`table`、`table-row`、`table-cell` 等:** 用于创建表格布局。


#### 示例

```css
.hidden {
  display: none; /* 隐藏元素 */
}

.block-element {
  display: block;
  width: 200px;
  height: 100px;
  background-color: lightblue;
}

.inline-element {
  display: inline;
  background-color: yellow;
}

.inline-block-element {
  display: inline-block;
  width: 150px;
  height: 50px;
  background-color: lightgreen;
}
```

### Visibility 属性

`visibility` 属性用于控制元素的可见性，它只会隐藏元素，但元素仍然占据原来的空间。

#### 常用取值

* **`visible`:** 元素可见。
* **`hidden`:** 隐藏元素，但元素仍然占据原来的空间。
* **`collapse`:**  用于表格元素，隐藏行或列，并且不占据空间。

#### 示例

```css
.invisible {
  visibility: hidden; /* 隐藏元素，但保留空间 */
}

.visible {
  visibility: visible; 
}

table tr.collapsed {
  visibility: collapse; 
}
```

### Display 与 Visibility 的区别

| 特性 | display: none | visibility: hidden |
|---|---|---|
| **可见性** | 隐藏元素 | 隐藏元素 |
| **空间占用** | 不占据空间 | 占据空间 |
| **布局影响** | 影响布局 | 不影响布局 |
| **子元素可见性** | 子元素也会被隐藏 | 子元素可以使用 `visibility: visible;` 来显示 |


### 使用场景

* **`display: none;`:** 
    * 当您希望完全移除元素及其占据的空间时。
    * 用于创建动态显示和隐藏的内容，例如通过 JavaScript 控制元素的显示状态。
* **`visibility: hidden;`:**
    * 当您希望隐藏元素但保留其占据的空间时。
    * 例如，您可以使用它来创建占位符，或者在加载内容时暂时隐藏元素。


### 总结

`display` 和 `visibility` 属性都用于控制元素的可见性，但它们的工作方式有所不同。 选择使用哪个属性取决于您希望如何处理元素的空间和布局。 
