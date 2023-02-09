图像
===

很明显地，要在纯文字应用中设计一个「自然」的语法来插入图片是有一定难度的。

Markdown 使用一种和链接很相似的语法来标记图片，同样也允许两种样式： 行内式和参考式。

### 行内式
行内式的图片语法看起来像是：

```markdown
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```

详细叙述如下：
- 一个惊叹号 !
- 接着一个方括号，里面放上图片的替代文字
- 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上 选择性的 'title' 文字。

```markdown
![GitHub](img/demo.jpg "GitHub,Social Coding")
```

***效果预览：***

![GitHub](img/demo.jpg "GitHub,Social Coding")


方括号中的部分是图片的替代文本，括号中的 ‘title’ 部分和链接一样，是可选的。

### 参考式
参考式的图片语法则长得像这样：
```markdown
![Alt text][id]
「id」是图片参考的名称，图片参考的定义方式则和连结参考一样：

[id]: url/to/image  "Optional title attribute"
```


```markdown
![GitHub][github]

[github]: img/demo.jpg "GitHub,Social Coding"
```

***效果预览：***

![GitHub][github]

[github]: img/demo.jpg "GitHub,Social Coding"


### 指定图片的显示大小
Markdown 暂时不支持指定图片的显示大小，不过可以通过直接插入`<img />`标签来指定相关属性：

```html
<img src="img/demo.jpg" alt="GitHub" title="GitHub,Social Coding" width="350" height="350" />
```

<img src="img/demo.jpg" alt="GitHub" title="GitHub,Social Coding" width="350" height="350" />