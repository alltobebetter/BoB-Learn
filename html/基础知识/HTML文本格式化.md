# HTML 文本格式化

HTML 提供了一系列标签，用于格式化网页上的文本内容，使其更具表现力和可读性。

### 1. 加粗文本

*   `<b>` 标签：定义粗体文本，纯粹为了视觉效果，没有语义上的强调。
*   `<strong>` 标签：定义重要的文本，表示内容的重要性，既有视觉效果，也有语义上的强调。

#### 示例：

```html
<b>This text is bold.</b><br>
<strong>This text is strong.</strong>
```

### 2. 斜体文本

*   `<i>` 标签：定义斜体文本，纯粹为了视觉效果，没有语义上的强调。
*   `<em>` 标签：定义强调的文本，表示内容的强调，既有视觉效果，也有语义上的强调。

#### 示例：

```html
<i>This text is italic.</i><br>
<em>This text is emphasized.</em>
```

### 3. 标记文本

*   `<mark>` 标签：定义标记文本，高亮显示文本内容，用于吸引用户的注意力。

#### 示例：

```html
<p>Do not forget to buy <mark>milk</mark> today.</p>
```

### 4. 删除文本和插入文本

*   `<del>` 标签：定义删除文本，表示文本内容已被删除。
*   `<ins>` 标签：定义插入文本，表示文本内容是新插入的。

#### 示例：

```html
<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
```

### 5. 下标和上标

*   `<sub>` 标签：定义下标文本，例如 H<sub>2</sub>O。
*   `<sup>` 标签：定义上标文本，例如 x<sup>2</sup> + y<sup>2</sup> = z<sup>2</sup>。

#### 示例：

```html
<p>The chemical formula for water is H<sub>2</sub>O.</p>
<p>Einstein's famous equation is E=mc<sup>2</sup>.</p>
```

### 6. 预格式化文本

*   `<pre>` 标签：定义预格式化文本，保留文本中的空格和换行符，常用于显示代码或诗歌等需要保留格式的文本。

#### 示例：

```html
<pre>
  This is 
  preformatted 
  text.
</pre>
```

### 7. 换行

*   `<br>` 标签：插入换行符，用于强制换行。

#### 示例：

```html
This is the first line.<br>
This is the second line.
```

### 8. 其他文本格式化标签

*   `<small>`: 定义小号文本。
*   `<big>`: 定义大号文本 (已弃用)。
*   `<q>`: 定义短文本引用。
*   `<blockquote cite="url">`: 定义长文本引用。
*   `<abbr title="abbreviation">`: 定义缩写。
*   `<dfn>`: 定义术语定义。
*   `<address>`: 定义联系信息。

### 总结

HTML 提供了丰富的文本格式化标签，可以使网页内容更具表现力和可读性。选择合适的标签可以使文本更易于理解，并提高网页的用户体验。
