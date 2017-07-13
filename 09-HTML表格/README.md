# HTML 表格

### 表格

表格由\<table>标签来定义。每个表格均有若干行（由\<tr>标签定义），每行被分割为若干单元格（由\<td>标签定义）。字母td指表格数据（table data）,即数据单元格的内容。数据单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等。

```html
    <table>
        <tr>
            <td>row 1,cell 1</td>
            <td>row 1,cell 2</td>
        </tr>
        <tr>
            <td>row 2,cell 1</td>
            <td>row 2,cell 2</td>
        </tr>
    </table>
```
***





### 边框属性

如果不定义边框属性，表格将不显示边框。有时这很有用。但是大多数时候，我们希望显示边框。
使用边框属性（border）来显示一个带有边框的表格。

```html
    <table border="1">
        <tr>
            <td>Row 1, cell 1</td>
            <td>Row 1, cell 2</td>
        </tr>
        <tr>
            <td>Row 2, cell 1</td>
            <td>Row 2, cell 2</td>
        </tr>
    </table>
```
***

### cellpadding 属性

cellpadding属性规定边沿及其内容之间的空白。
取值：pixels %

```html
    <table border="1" cellpadding="10">
        <tr>
            <td>row 1, cell 1</td>
            <td>row 1, cell 2</td>
        </tr>
    </table>
```

***

### cellspacing 属性

cellspacing属性规定单元格之间的空白。
取值：pixels %

```html
    <table border="1" cellpadding="10" cellspacing="5">
        <tr>
            <td>row 1, cell 1</td>
            <td>row 2, cell 2</td>
        </tr>
    </table>
```

***

### 表格的标题

表格的标题使用\<caption>标签进行定义

***

### 表格的表头

表格的表头使用\<th>标签进行定义。
大多数浏览器会把表头显示为粗体居中的文本：

```html
    <table border="1">
        <tr>
            <th>Heading</th>
            <th>Another Heading</th>
        </tr>
        <tr>
            <td>row 1, cell 1</td>
            <td>row 1, cell 2</td>
        </tr>
        <tr>
            <td>row 2, cell 1</td>
            <td>row 2, cell 2</td>
        </tr>
    </table>
```

***

