# CSS ID 和 Class 选择器

ID 和 Class 选择器是 CSS 中两种常用的选择器，用于选择 HTML 元素并应用样式。它们的主要区别在于 **ID 选择器是唯一的**，而 **Class 选择器可以被多个元素共享**。

### ID 选择器

*   语法：`#idName { ... }`
*   作用：选择具有指定 ID 的 **唯一** HTML 元素。
*   示例：

```html
<p id="intro">This is an introductory paragraph.</p>
```

```css
#intro {
  font-size: 20px;
  color: blue;
}
```

### Class 选择器

*   语法：`.className { ... }`
*   作用：选择具有指定 Class 的 **所有** HTML 元素。
*   示例：

```html
<p class="highlight">This is a highlighted paragraph.</p>
<p class="highlight">This is another highlighted paragraph.</p>
```

```css
.highlight {
  background-color: yellow;
}
```

### ID 和 Class 的区别

| 特性         | ID 选择器                  | Class 选择器                  |
| ------------ | --------------------------- | ---------------------------- |
| 唯一性       | 唯一，每个页面只能使用一次 | 可以被多个元素共享          |
| 使用场景     | 针对特定元素                | 针对一组具有相同特征的元素 |
| 优先级       | 高于 Class 选择器         | 低于 ID 选择器              |
| JavaScript | 可以通过 `getElementById()` 获取 | 可以通过 `getElementsByClassName()` 获取 |


### 何时使用 ID 和 Class

*   **使用 ID 选择器**: 当你需要选择页面上的 **唯一元素** 并应用特定样式时，例如页面标题、导航栏、页脚等。
*   **使用 Class 选择器**: 当你需要选择页面上的 **多个元素** 并应用相同的样式时，例如文章标题、列表项、按钮等。


### 示例：结合 ID 和 Class

```html
<h1 id="main-title" class="important">Welcome to My Website</h1>
<p class="important">This is an important paragraph.</p>
```

```css
#main-title {
  font-size: 36px;
}

.important {
  color: red;
}
```

在这个例子中，`#main-title` 选择器会将 `<h1>` 元素的字体大小设置为 36px，而 `.important` 选择器会将 `<h1>` 元素和 `<p>` 元素的文本颜色设置为红色。

### 总结

ID 和 Class 选择器是 CSS 中两种常用的选择器，用于选择 HTML 元素并应用样式。ID 选择器是唯一的，而 Class 选择器可以被多个元素共享。选择使用哪种选择器取决于你想要选择的目标元素和应用的样式。
