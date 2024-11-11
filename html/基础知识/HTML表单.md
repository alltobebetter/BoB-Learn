# HTML 表单

HTML 表单用于收集用户输入的信息，例如姓名、电子邮件地址、密码等等。表单数据通常会被提交到服务器进行处理。

### 创建表单

HTML 表单使用 `<form>` 标签创建。表单中的各种输入元素，例如文本框、密码框、单选按钮、复选框等等，都放置在 `<form>` 标签内部。

**基本语法:**

```html
<form action="/submit" method="post">
  <!-- 表单元素 -->
</form>
```

*   **`action` 属性:** 指定表单数据提交到的 URL。
*   **`method` 属性:** 指定表单数据提交的方式，常用的方法有 `get` 和 `post`。

### 表单元素

以下是一些常用的表单元素：

#### 1. 文本框 (`<input type="text">`)

用于输入单行文本。

**示例:**

```html
<label for="name">Name:</label>
<input type="text" id="name" name="name">
```

#### 2. 密码框 (`<input type="password">`)

用于输入密码，输入的字符会被隐藏。

**示例:**

```html
<label for="password">Password:</label>
<input type="password" id="password" name="password">
```

#### 3. 单选按钮 (`<input type="radio">`)

用于选择一个选项。

**示例:**

```html
<label for="male">Male:</label>
<input type="radio" id="male" name="gender" value="male">

<label for="female">Female:</label>
<input type="radio" id="female" name="gender" value="female">
```

#### 4. 复选框 (`<input type="checkbox">`)

用于选择多个选项。

**示例:**

```html
<label for="html">HTML:</label>
<input type="checkbox" id="html" name="skills" value="html">

<label for="css">CSS:</label>
<input type="checkbox" id="css" name="skills" value="css">
```

#### 5. 下拉列表 (`<select>`)

用于选择一个选项。

**示例:**

```html
<label for="country">Country:</label>
<select id="country" name="country">
  <option value="usa">USA</option>
  <option value="canada">Canada</option>
  <option value="uk">UK</option>
</select>
```

#### 6. 文本域 (`<textarea>`)

用于输入多行文本。

**示例:**

```html
<label for
