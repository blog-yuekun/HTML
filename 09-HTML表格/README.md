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

### 表格的标题

表格的标题使用\<caption>标签进行定义
    
```html
    <table border="1">
        <caption>成绩表</caption>
        <tr>
            <th>姓名</th>
            <th>语文</th>
            <th>数学</th>
        </tr>
        <tr>
            <td>张三</td>
            <td>99</td>
            <td>100</td>
        </tr>
        <tr>
            <td>李四</td>
            <td>100</td>
            <td>100</td>
        </tr>
    </table>
```    
***

### 细线表格1 - border-collapse属性

border-collapse属性设置表格的边框是否被合并为一个单一的边框，还是像在HTML标准中那样分开显示。

__取值__：
1. separate - 默认值，边框被分开，不会忽略border-spacing 和 empty-cells 属性
2. collapse - 如果可能，边框会合并为一个单一的边框。会忽略border-spacing 和 empty-cells 属性
3. inherit - 规定应该从父元素继承 border-collapse 属性的值。

__注意__: 如果没有规定 !DOCTYPE，border-collapse 属性可能会引起意想不到的错误。

```html
    <table border="1" style="border-collapse: collapse">
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

### 细线表格2 - 使用cell-spacing属性和背景颜色

__注意__：打印时间可能出现表格边框打印不出来。

```html
    <table border="0" cellspacing="1" bgcolor="red">
        <tr bgcolor="#FFF">
            <td>row 1, cell 1</td>
            <td>row 2, cell 2</td>
        </tr>
        <tr bgcolor="#FFF">
            <td>row 2, cell 1</td>
            <td>row 2, cell 2</td>
        </tr>
    </table>
```
