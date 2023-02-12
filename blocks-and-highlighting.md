代码块和语法高亮
===

## 代码块

与原来使用缩进来添加代码块的语法不同，这里使用 \``` \``` 来包含多行代码：

```markdown
<p>code here</p>
```
<p>code here</p>
三个 ``` 要独占一行。

## 代码高亮
在上面的代码块语法基础上，在第一组 ``` 之后添加代码的语言，如 ‘javascript’ 或 ‘js’，即可将代码标记为 JavaScript：

code-js

window.addEventListener('load', function() {
  console.log('window loaded');
});


如果要标记一小段行内代码，你可以用反引号把它包起来（`），例如：

Use the `printf()` function.
会产生：

<p>Use the <code>printf()</code> function.</p>
如果要在代码区段内插入反引号，你可以用多个反引号来开启和结束代码区段：

``There is a literal backtick (`) here.``
这段语法会产生：

<p><code>There is a literal backtick (`) here.</code></p>
代码区段的起始和结束端都可以放入一个空白，起始端后面一个，结束端前面一个，这样你就可以在区段的一开始就插入反引号：

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``
会产生：

<p>A single backtick in a code span: <code>`</code></p>

<p>A backtick-delimited string in a code span: <code>`foo`</code></p>
在代码区段内，& 和方括号都会被自动地转成 HTML 实体，这使得插入 HTML 原始码变得很容易，Markdown 会把下面这段：

Please don't use any `<blink>` tags.
转为：

<p>Please don't use any <code><blink></code> tags.</p>
你也可以这样写：

`&#8212;` is the decimal-encoded equivalent of `&mdash;`.
以产生：

<p><code>&amp;#8212;</code> is the decimal-encoded
equivalent of <code>&amp;mdash;</code>.</p>
