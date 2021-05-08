# CSS 字体属性

CSS Fonts（字体）属性用于定义**字体系列**、大小、粗细、文字样式（如斜体）

## 字体系列

CSS 使用**font-family**属性定义文本的字体系列

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