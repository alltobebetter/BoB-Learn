# CSS 文本

### 文本格式化

CSS 提供了丰富的属性来控制文本的格式，例如字体、颜色、大小、对齐方式、间距等等。

#### 1. 字体

* **`font-family`**: 设置字体系列，例如 Arial、Times New Roman 等。可以使用通用字体系列（例如 serif、sans-serif、monospace）作为后备选项。

##### 示例：

```css
p {
  font-family: Arial, sans-serif;
}
```

* **`font-size`**: 设置字体大小，可以使用像素 (px)、em、百分比 (%) 等单位。

##### 示例：

```css
h1 {
  font-size: 2em;
}
```

* **`font-style`**: 设置字体样式，例如 normal、italic、oblique。

##### 示例：

```css
em {
  font-style: italic;
}
```

* **`font-weight`**: 设置字体粗细，例如 normal、bold、bolder、lighter，或者使用数值 (100-900)。

##### 示例：

```css
strong {
  font-weight: bold;
}
```

#### 2. 颜色

* **`color`**: 设置文本颜色，可以使用颜色名称、十六进制代码、RGB 值等。

##### 示例：

```css
a {
  color: blue;
}
```

#### 3. 对齐方式

* **`text-align`**: 设置文本水平对齐方式，例如 left、center、right、justify。

##### 示例：

```css
h2 {
  text-align: center;
}
```

#### 4. 行高

* **`line-height`**: 设置行高，可以使用数值、百分比、em 等单位。

##### 示例：

```css
p {
  line-height: 1.5;
}
```

#### 5. 字间距和字母间距

* **`letter-spacing`**: 设置字母间距。
* **`word-spacing`**: 设置字间距。

##### 示例：

```css
h3 {
  letter-spacing: 2px;
}
```

#### 6. 文本装饰

* **`text-decoration`**: 设置文本装饰，例如 none、underline、overline、line-through。

##### 示例：

```css
a {
  text-decoration: underline;
}
```

#### 7. 文本阴影

* **`text-shadow`**: 设置文本阴影，可以使用多个阴影效果。

##### 示例：

```css
h4 {
  text-shadow: 2px 2px 5px gray;
}
```

#### 8. 文本转换

* **`text-transform`**: 设置文本大小写，例如 uppercase、lowercase、capitalize。

##### 示例：

```css
p.uppercase {
  text-transform: uppercase;
}
```

### 其他文本属性

CSS 还提供其他一些文本相关的属性，例如 `white-space`、`text-overflow`、`direction` 等，可以根据需要进行使用。

### 总结

CSS 提供了丰富的属性来控制文本的格式，可以根据设计需求灵活使用这些属性来创建美观易读的文本内容。
