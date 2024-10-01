[toc]



# 换段落

1. 一次Enter（特定于Typora）
2. 多次Enter（Markdown源代码中）



# 段落内换行
1. Shrift+Enter（特定于Typora）
2. two spaces在行末（Markdown源代码中）
3. 在行末插入"</br>"



# 标题
1. 1-6个 hash 在行头代表 1-6级标题	(#)
2. 快捷键（Ctrl+Number）



# Blockquotes 块引用

1. 使用 ">" 用于块引用	(>)
2. 块引用内可以有多个段落也可以只是一个段落（多行），具体规则如上
3. 块引用内可以通过写入新的 ">" 来实现嵌套



# Lists 列表

1. 有序列表(1. )<blockquote> (Number+dot+space )	(*生效需在内容之后键入Enter键)</blockquote>
2. 无序列表(*. ) <blockquote>(\*+dot+space)	(\*可以用+或-代替)</blockquote>



# Task List 任务列表

1. 用(- [ ] content)来创建任务列表,若为[x]则代表任务已完成



# Code Blocks 代码块

1. 仅支持GitHub Flavored Markdown中的fence用法,不支持原代码块样式
2. (```+Enter)
3. 再```后键入代码语言(如html)可使代码块按照对应语言规则高亮



# Math Blocks 数学块

1. LaTex是数学表达规范,MathJax拓展是Typora用来渲染的LaTex的工具
2. 通过($$+Enter)使用



# Tables 表格

1. 输入(| First Header | Second Header |)使用
2. 后续操作通过toolbar操作,没必要知道完整的句法规则(至少在Typora中)
3. 在表格中也可以使用inline Markdown(行内标记),如links、bold、italics(斜体)、strikethrough（删除线）



# Footnotes 脚注

1. MultiMarkdown拓展提供了两种方式添加脚注
2. 脚注标记与脚注内容通过(\[^脚注名]:)使用,在中括号内无需space,文章中脚注标记无序":",脚注内容需处要":"
3. 通过(Ctrl+click)脚注标记跳转到脚注内容



# Horizontal Rules 水平分割线

1. 在blank line中使用(***/--- + Enter)



# YAML Front Matter(undone)

1. YAML(YAML Ain't Markup Language)Front Matter 是一种在文本文件（尤其是Markdown文件或静态站点生成器使用的文件中）常见的元数据组织方式。
2. 它允许作者在文档内容之前，通过特定的标记（通常是一组三个连字符 `---`）包裹一系列YAML格式的数据，来定义文档的元信息或属性，如标题、日期、分类、标签等。常用于配置文件、数据交换格式以及各类应用程序中需要存储或传输数据的场景
3. YAML使用空白（空格或制表符）缩进而不是大括号 `{}` 或者括号 `[]` 来表示数据结构的层级关系，使得文件看起来更加整洁和易于阅读。



# Table of Contents(TOC)

1. 键入([toc] + Enter)可以生成文章目录(包含所有标题),并且随改变而自动更新



# Callouts / Github Style Alerts(undone)



# Span Elements

​	span元素在键入后会立刻被解析和渲染,

## Links

1. Markdown支持两种style的link,两种类型均通过([]square brackets)分割

* inline
* reference

### Inline Links

1. 由三部分组成

   * link text:渲染后的链接呈现文本
   * URL:链接指向

   * title属性(optional):cursor悬浮在渲染后的链接上额外呈现出来的信息

2. 格式:[link text]\(URL "Title")

### Internal Links(undone)（属于Inline Links的一种）

1. 创建内部链接(bookmark)
2. 格式:[link text]\(#block-elements "Titile")
3. block-elements(undone):已知包括标题

### Reference Links

1. 使用两组square brackets,第一组设置link text,第二组设置label.由链接标记、链接内容两部分组成（类似Footnotes脚注）
2. 格式:
   * 链接标记：[link text]\[label]
   * 链接内容:[label]:URL "Title"(optional)
3. click以编辑,Ctrl + click以指向链接

* Caution：Inline Links中URL有parentheses，而Refernce Links中没有

4. 如果omit（省略）了label，即第二组square brackets为空，则默认link text作为label的值



# URLs

1. 用bracket("< >")包裹链接
2. 若链接为标准URLs,则会自动生成链接,无需bracket



# Images 图片

1. 与链接syntax相似
2. 格式:![text]\(/path/to/img.jpg "Optional title")
   * 其中text部分是图像的替代文字，如果图像无法显示或者用户禁用了图像显示
3. 在YAML Front Matter中使用typora-root-url属性可以为所有相对路径指定前缀,因而可以在网页构建时简化URL的输入



# Emphasis 

1. Markdown把一组asterisks(*)或一组underscores(_)视作\<em>标签(效果上是斜体)
2. 在代码块中,由于Typora支持GFM,而GFM会忽视underscores(在代码中下划线很常用),所以最好习惯使用asterisks



# Strong

1. double *或 _视作\<strong>标签,同样推荐使用asterisks



# Inline Code 

1. 在正常段落内嵌入代码的方式,是使用\`code`来包裹代码,效果如\<span>标签,属于行内元素,不会换行



# Strikethrough

1.  使用~~包裹文本实现删除线



# Emoji 表情符号

1. 使用:emoji:来包裹表情符号名称,在输入后会有auto-complete helper pop up
2. 使用Win + .快捷键打开



# Inline Math(undone)

1. 使用$LaTEX comman$包裹数学命令
2. 如何preview渲染后的结果(undone)



# Subscript 下标

1. 使用一组~   ~包裹下表内容



# Superscipt 上标

1. 使用一组^ ^去包裹商标内容



# Highlight

1. 用一组==   ==取包裹高亮内容



# HTML

可以使用HTML去给内容添加额外样式

## Underlines

1. 使用\<u>标签添加下划线

## Embed Contents

1. 使用\<iframe>标签来在当前网页嵌入外部网页

   - `src` 属性是必需的，它指定嵌入内容的URL。

   - `width` 和 `height` 分别用于设置iframe的宽度和高度。

   - `frameborder="0"` 用于移除iframe周围的边框（默认边框宽度为1）。

   - `scrolling="no/yes/auto"` 控制是否显示滚动条，`no` 表示不显示，`yes` 表示总是显示，`auto` 表示根据需要自动显示。

2. 全称为 **Inline Frame**（内联框架），它允许在一个HTML页面内部嵌入另一个完整的HTML文档。这意味着你可以在当前网页中嵌套显示来自不同源的网页内容，例如嵌入视频、地图、广告或者其他互动式内容，而这些内容在一个固定的框架内显示，与主页面的其余部分相对独立。



## Video

1. 使用\<video>标签嵌入视频
   * \<video src="">





- [ ] 列表中似乎不会识别很多标签
- [ ] 注意space和Enter的使用以符合语法规范从而使用功能
- [ ] 冒号不明显的解决方法
- [ ] 自动保存功能与版本管理的冲突
- [ ] block/span/inline三种元素？
- [ ] 提问格式:如何从词汇构成的角度理解“脚本”这一术语在计算机科学中的命名缘由



