markdown简易入门参考
===


## markdown简介
百度百科是这样定义markdown的：

> Markdown 是一种轻量级标记语言。 它允许人们使用易读易写的纯文本格式编写文档，
> 然后转换成有效的 XHTML（或者HTML）文档。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。
>
> 由于 Markdown 的轻量化、易读易写特性，并且对于图片，图表、数学式都有支持，许多网站都广泛使用 
> Markdown 来撰写帮助文档或是用于论坛上发表消息。 如 GitHub、Reddit、Diaspora、Stack Exchange、
> OpenStreetMap 、SourceForge、简书等，甚至还能被使用来撰写电子书。

Markdown具有一系列衍生版本，用于扩展Markdown的功能（如表格、脚注、内嵌HTML等等），这些功能原初的Markdown尚不具备，它们能让Markdown转换成更多的格式。

较常用的格式转换为将markdown文件转换为HTML、PDF、Word等格式,也有利用markdown来制作电子书的。

## 宗旨
Markdown 的目标是实现「易读易写」。

可读性，无论如何，都是最重要的。一份使用 Markdown 格式撰写的文件应该可以直接以纯文本发布，
并且看起来不会像是由许多标签或是格式指令所构成。Markdown 语法受到一些既有 text-to-HTML 格式的影响，
包括 Setext、atx、Textile、reStructuredText、Grutatext 和 EtText，
而最大灵感来源其实是纯文本电子邮件的格式。

## 兼容 HTML
Markdown 语法的目标是：成为一种适用于网络的书写语言。

Markdown 不是想要取代 HTML，甚至也没有要和它相近，它的语法种类很少，只对应 HTML 标记的一小部分。
Markdown 的构想不是要使得 HTML 文档更容易书写。在我看来， HTML 已经很容易写了。
Markdown 的理念是，能让文档更容易读、写和随意改。HTML 是一种发布的格式，Markdown 是一种书写的格式。
就这样，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。不需要额外标注这是 HTML 或是 Markdown；
只要直接加标签就可以了。

要制约的只有一些 HTML 区块元素――比如 `<div>`、`<table>`、`<pre>`、`<p>` 等标签，
必须在前后加上空行与其它内容区隔开，还要求它们的开始标签与结尾标签不能用制表符或空格来缩进。
Markdown 的生成器有足够智能，不会在 HTML 区块标签外加上不必要的 `<p>` 标签。

例子如下，在 Markdown 文件里加上一段 HTML 表格：

---
```markdown
这是一个普通段落。

<table>
    <tr>
        <td>表格一</td>
        <td>表格二</td>
    </tr>
    <tr>
        <td>表格三</td>
        <td>表格四</td>
    </tr>
</table>

这是另一个普通段落。
```

***效果预览：***


这是一个普通段落。
<table>
    <tr>
        <td>表格一</td>
        <td>表格二</td>
    </tr>
    <tr>
        <td>表格三</td>
        <td>表格四</td>
    </tr>
</table>
这是另一个普通段落。

- - - - -

请注意，在 HTML 区块标签间的 Markdown 格式语法将不会被处理。比如，你在 HTML 区块内使用 Markdown 
样式的 *强调* 会没有效果。

HTML 的区段（行内）标签如 `<span>`、`<cite>`、`<del>` 可以在 Markdown 的段落、列表或是标题里随意使用。
依照个人习惯，甚至可以不用 Markdown 格式，而直接采用 HTML 标签来格式化。举例说明：如果比较喜欢 HTML 的 
`<a>` 或 `<img>` 标签，可以直接使用这些标签，而不用 Markdown 提供的链接或是图像标签语法。

和处在 HTML 区块标签间不同，Markdown 语法在 HTML 区段标签间是有效的。


## 常用命令

|  字体效果  |      写法      | 效果预览               |
|:------:|:------------:|:-------------------|
|   斜体   |   `* 文本 *`   | *单星号，文本斜体*         |
|   斜体   |   `_ 文本 _`   | _单下横线，也是文本斜体_      |
|   加粗   |  `** 文本 **`  | **双星号，文本加粗**       |
|   加粗   |  `__ 文本 __`  | __双下横线，也是文本加粗__    |
| 加粗+斜体  | `*** 文本 ***` | ***三星号，文本加粗+斜体***  |
| 加粗+斜体  | `___ 文本 ___` | ___三下横线，文本加粗+斜体___ |
|  删除线   |  `~~ 文本 ~~`  | ~~双波浪线，文字加删除线~~    |




## 目录
#### 区块元素
1. [段落和换行](paragraph.md)
2. [标题](headers.md)
3. [引用](blockquotes.md)
4. [列表](lists.md)
5. [代码](code.md)
6. [分割线](horizontal-rule.md)
7. [Task List](task-list.md)

#### 区段元素
1. [超链接](links.md)
2. [图片](images.md)
3. [强调](emphasis.md)
4. [字符转义](blackslash-escapes.md)
5. [删除线](strikethrougn.md)
6. [代码块和语法高亮](blocks-and-highlighting.md)
7. [表格](table.md)



_ _ _
版权所有 <http://three-corner.xyz>