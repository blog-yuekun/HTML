# HTML列表

### 无序列表

无序列表是一个项目的列表，此项目使用粗体圆点进行标记。  
无序列表始于\<ul>标签。每个列表项始于\<li>。  

```html
    <ul>
        <li>Coffee</li>
        <li>Milk</li>
    </ul>
```

浏览器显示如下:
* Coffee
* Milk

#### 无序列表 type属性

__不赞成使用，请使用样式取代__

* disc - 默认属性，实心小圆点。
* circle - 空心圆点。
* square - 实心方块。

***

### 有序列表

有序列表也是一列项目，列表项目使用数字进行标记。
有序列表始于\<ol>标签。每个列表项始于\<li>标签。

```html
    <ol>
        <li>Coffee</li>
        <li>Milk</li>
    </ol>
```

浏览器显示如下：
1. Coffee
2. Milk

#### 有序列表type属性

* 1 - 默认属性
* A - 大写英文字母
* a - 小写英文字母
* I - 大写罗马字母
* i - 小写罗马字母

#### 有序列表 start属性

规定有序列表的起始值

```html
    <ol start="50">
        <li>Coffee</li>
        <li>Milk</li>
    </ol>
```

浏览器显示如下：  
50. Coffee
51. Milk

#### 有序列表的 reversed属性

规定列表顺序为降序

```html
    <ol reversed>
        <li>Coffee</li>
        <li>Milk</li>
    </ol>
```

***

### 定义列表

定义列表不仅仅是一列项目，而是项目及其注释的组合。  
\<dl>标签定义了定义列表（definition list）。
\<dl>标签用于结合\<dt>（定义列表中的项目）和\<dd>（描述列表中的项目）。

```html
    <dl>
        <dt>Coffee</dt>
        <dd>Black hot drink</dd>
        <dt>Milk</dt>
        <dd>white cold drink</dd>
    </dl>
```


