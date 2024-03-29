# CSS 字体属性

CSS Fonts（字体）属性用于定义**字体系列**、大小、粗细、文字样式（如斜体）

## 字体系列

CSS 使用`font-family`属性定义文本的字体系列

```css
p {
    font-family: "微软雅黑";
}

div {
    font-family: Arial, "Microsoft Yahei", "微软雅黑";
}
```

- 各种字体之间必须使用英文逗号隔开

- 一般情况下，用引号包裹由多个单词组成的一个字体系列名

- 尽量使用系统默认自带字体，保证在任何用户的浏览器中都能正确显示

- 比较常见的几个字体 `body {font-family: 'Microsoft Yahei', tahoma, arial, 'Hiragino Sans GB';}`

## 字体大小

```css
p {
    font-size: 20px;
}
```

- px（像素）大小是网页的最常用单位
- Chrome默认文字大小为16px
- 不同浏览器可能默认显示的字号大小不一致，我们尽量给一个明确大小，不要默认大小
- 可以给body指定整个页面文字的大小

## 字体粗细

CSS 使用`font-weight`属性设置文本字体的粗细

```css
p {
    font-weight: bold;
}
```

| 属性值  | 描述                                                      |
| ------- | --------------------------------------------------------- |
| normal  | 默认值（不加粗的）                                        |
| bold    | 定义粗体（加粗的）                                        |
| 100~900 | 400等同于normal，而700等同于bold 注意这个数字后面不跟单位 |

- 学会把标题等加粗的变成不加粗的，或者把normal的变成加粗的

## 文字样式

CSS 使用`font-style`属性设置文本的风格

```css
p {
    font-style: normal;
}
```

| 属性值 | 作用                               |
| ------ | ---------------------------------- |
| normal | 默认值，浏览器会显示标准的字体样式 |
| italic | 浏览器会显示斜体的字体样式         |

**注意：** 平时我们很少给文字加斜体，反而要给斜体标签（em, i）改为不倾斜字体

## 字体复合属性

字体属性可以把各种文字样式综合来写，这样更节约代码

```css
body {
    font: font-style font-weight font-size/line-height font-family;
}
```

- 使用font属性时，必须按上面语法格式中的顺序书写，**不能更换顺序**，并且各个属性之间以**空格**隔开
- 不需要设置的属性可以省略（取默认值），但是**必须保留font-size和font-family属性**，否则font属性将不起作用
