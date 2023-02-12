代码
===


如果要标记一小段行内代码，你可以用反引号把它包起来（`），例如：

```markdown
在java语言中，要打印输出内容可以使用 `system.out.print()` 来将内容输出都命令行中。 
```

会产生下面这样的html代码的效果

```html
<p>在java语言中，要打印输出内容可以使用 <code>system.out.print()</code> 来将内容输出都命令行中。 </p>
```

***效果预览：***

在java语言中，要打印输出内容可以使用 `system.out.print()` 来将内容输出都命令行中。 


如果要在代码区段内插入反引号，你可以用多个反引号来开启和结束代码区段：

```markdown
``单个反引号（`)可以在多个反引号中直接使用``
```

上面的这个代码，会生成下面这样的html

```html
<p><code>单个反引号（`)可以在多个反引号中直接使用</code></p>
```

***效果预览：***

``单个反引号（`)可以在多个反引号中直接使用``


代码区段的起始和结束端都可以放入一个空白，起始端后面一个，结束端前面一个，这样你就可以在区段的一开始就插入反引号：

```markdown
比如这样插入一个单引号: `` ` ``

或者这样插入一个短代码: `` `foo` ``
```

上面的这个代码，会生成下面这样的html代码：

```html
<p>比如这样插入一个单引号: <code>`</code></p>
<p>或者这样插入一个短代码: <code>`foo`</code></p>
```

***效果预览：***

比如这样插入一个单引号： `` ` ``
或者这样插入一个短代码： `` `foo` ``

在代码区段内，& 和方括号都会被自动地转成 HTML 实体，这使得插入 HTML 原始码变得很容易，Markdown 会把下面这段：

```markdown
Please don't use any `<blink>` tags.
```

生成下面这样的html代码:

```html
<p>Please don't use any <code><blink></code> tags.</p>
```

***效果预览：***

Please don't use any `<blink>` tags.

你也可以这样写：

```markdown
`& #8212;` is the decimal-encoded equivalent of `& mdash;`.
```

生成下面这样的html代码:

```markdown
<p><code>&amp; #8212;</code> is the decimal-encoded
equivalent of <code>&amp; mdash;</code>.</p>
```

***效果预览：***

<p><code>&amp; #8212;</code> is the decimal-encoded
equivalent of <code>&amp; mdash;</code>.</p>