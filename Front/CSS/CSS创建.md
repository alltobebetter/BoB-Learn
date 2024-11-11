# CSS 的创建和应用

CSS 代码可以通过三种方式创建和应用到 HTML 文档中：

## 1. 内联样式 (Inline Styles)

内联样式直接写在 HTML 元素的 `style` 属性中。

**语法:**

```html
<element style="property1: value1; property2: value2; ..."> </element>
```

**示例:**

```html
<p style="color: blue; font-size: 16px;">This is a blue paragraph.</p>
```

**优点:**

*   优先级最高，会覆盖其他样式。
*   方便快速地为单个元素应用样式。

**缺点:**

*   可维护性差，如果需要修改多个元素的样式，需要逐个修改。
*   代码冗余，不利于代码复用。

## 2. 内部样式表 (Internal Stylesheet)

内部样式表写在 HTML 文档的 `<head>` 部分的 `<style>` 标签中。

**语法:**

```html
<head>
  <style>
    /* CSS 规则 */
  </style>
</head>
```

**示例:**

```html
<!DOCTYPE html>
<html>
<head>
  <title>Internal Stylesheet Example</title>
  <style>
    p {
      color: red;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <p>This is a red paragraph.</p>
</body>
</html>
```

**优点:**

*   比内联样式更易于维护，可以集中管理当前页面的样式。
*   代码更简洁，避免了代码冗余。

**缺点:**

*   无法在多个页面之间共享样式。

## 3. 外部样式表 (External Stylesheet)

外部样式表保存在独立的 `.css` 文件中，然后通过 `<link>` 标签链接到 HTML 文档。

**语法:**

```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

**示例:**

**style.css:**

```css
p {
  color: green;
  font-size: 12px;
}
```

**HTML:**

```html
<!DOCTYPE html>
<html>
<head>
  <title>External Stylesheet Example</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <p>This is a green paragraph.</p>
</body>
</html>
```

**优点:**

*   可维护性最好，可以集中管理所有页面的样式。
*   代码复用性高，可以在多个页面之间共享样式。

**缺点:**

*   需要额外加载一个文件，可能会影响页面加载速度。


## 总结

三种创建 CSS 的方式各有优缺点，应根据实际情况选择合适的方案。

*   **内联样式:** 适用于快速修改单个元素的样式。
*   **内部样式表:** 适用于单个页面的样式管理。
*   **外部样式表:** 适用于多个页面共享样式，提高代码复用性和可维护性。 

通常情况下，建议使用外部样式表来管理 CSS 代码，以便更好地组织和维护网站的样式。 另外，如果外部样式表和内联样式表发生冲突，内联样式表的优先级更高。

如果某些属性在不同的样式表中被同样的选择器定义，那么属性值将从更具体的样式表中被继承过来。

例如，外部样式表拥有针对 `h3` 选择器的三个属性：

```css
h3 {
    color: red;
    text-align: left;
    font-size: 8pt;
}
```

而内部样式表拥有针对 `h3` 选择器的两个属性：

```css
h3 {
    text-align: right;
    font-size: 20pt;
}
```

假如拥有内部样式表的这个页面同时与外部样式表链接，那么 `h3` 得到的样式是：

- `color: red;`
- `text-align: right;`
- `font-size: 20pt;`

即颜色属性将被继承于外部样式表，而文字排列（text-alignment）和字体尺寸（font-size）会被内部样式表中的规则取代。
