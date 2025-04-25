[toc]



# Learn LaTeX in 30 minutes 在 30 分钟内学习 LaTeX

This introductory tutorial does not assume any prior experience of LaTeX but, hopefully, by the time you are finished, you will not only have written your first LaTeX document but also acquired sufficient knowledge and confidence to take the next steps toward LaTeX proficiency.
本入门教程不假定您之前有任何 LaTeX 经验，但希望当您完成时，您不仅已经编写了您的第一个 LaTeX 文档，而且还获得了足够的知识和信心，可以采取下一步的措施来熟练掌握 LaTeX。

## Contents 内容

- [1 What is LaTeX?
  1什么是 LaTeX？](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#What_is_LaTeX?)
- [2 Why learn LaTeX?
  2为什么要学习 LaTeX？](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Why_learn_LaTeX?)
- [3 Writing your first piece of LaTeX
  3写你的第一篇 LaTeX](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Writing_your_first_piece_of_LaTeX)
- [4 The preamble of a document
  4文档的序言](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#The_preamble_of_a_document)
- [5 Including title, author and date information
  5包括标题、作者和日期信息](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Including_title,_author_and_date_information)
- [6 Adding comments
  6添加评论](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_comments)
- [7 Bold, italics and underlining
  7粗体、斜体和下划线](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Bold,_italics_and_underlining)
- [8 Adding images
  8添加图片](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_images)
- [9 Captions, labels and references
  9标题、标签和参考](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Captions,_labels_and_references)
- 10 Creating lists in LaTeX
  10在 LaTeX 中创建列表
  - [10.1 Unordered lists
    10.1无序列表](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Unordered_lists)
  - [10.2 Ordered lists
    10.2有序列表](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Ordered_lists)
- 11 Adding math to LaTeX
  11向 LaTeX 添加数学运算
  - [11.1 Inline math mode
    11.1内联数学模式](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Inline_math_mode)
  - [11.2 Display math mode
    11.2显示数学模式](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Display_math_mode)
  - [11.3 More complete examples
    11.3更完整的示例](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#More_complete_examples)
- 12 Basic document structure
  12基本文档结构
  - [12.1 Abstracts
    12.1摘要](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Abstracts)
  - [12.2 Paragraphs and new lines
    12.2段落和换行符](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Paragraphs_and_new_lines)
  - [12.3 Chapters and sections
    12.3章节](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Chapters_and_sections)
- 13 Creating tables
  13创建表格
  - [13.1 Creating a basic table in LaTeX
    13.1在 LaTeX 中创建基本表](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Creating_a_basic_table_in_LaTeX)
  - [13.2 Adding borders
    13.2添加边框](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_borders)
  - [13.3 Captions, labels and references
    13.3标题、标签和引用](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Captions,_labels_and_references_2)
- [14 Adding a Table of Contents
  14添加目录](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_a_Table_of_Contents)
- [15 Downloading your finished document
  15下载完成的文档](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Downloading_your_finished_document)
- 16 Finding and using LaTeX packages
  16查找和使用 LaTeX 包
  - [16.1 Loading packages
    16.1加载软件包](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Loading_packages)
  - [16.2 Finding information about packages: CTAN
    16.2查找有关软件包的信息：CTAN](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_information_about_packages:_CTAN)
  - [16.3 Packages available on Overleaf: Introducing TeX Live
    16.3Overleaf 上可用的软件包：TeX Live 简介](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Packages_available_on_Overleaf:_Introducing_TeX_Live)

## What is LaTeX? 什么是 LaTeX？

LaTeX (pronounced “*LAY*-tek” or “*LAH*-tek”) is a tool for typesetting professional-looking documents. However, LaTeX’s mode of operation is quite different to many other document-production applications you may have used, such as Microsoft Word or LibreOffice Writer: those “[WYSIWYG](https://en.wikipedia.org/wiki/WYSIWYG)” tools provide users with an interactive page into which they type and edit their text and apply various forms of styling. LaTeX works very differently: instead, your document is a plain text file interspersed with LaTeX *commands* used to express the desired (typeset) results. To produce a visible, typeset document, your LaTeX file is processed by a piece of software called a *TeX engine* which uses the commands embedded in your text file to guide and control the typesetting process, converting the LaTeX commands and document text into a professionally typeset PDF file. This means you only need to focus on the *content* of your document and the computer, via LaTeX commands and the TeX engine, will take care of the *visual appearance* (formatting).
LaTeX（发音为“*LAY-tek*”或“*LAH-tek*”）是一种用于排版具有专业外观的文档的工具。但是，LaTeX 的操作模式与您可能使用过的许多其他文档制作应用程序（例如 Microsoft Word 或 LibreOffice Writer）完全不同：这些“[所见即所得](https://en.wikipedia.org/wiki/WYSIWYG)”工具为用户提供了一个交互式页面，他们可以在其中键入和编辑文本并应用各种形式的样式。LaTeX 的工作方式非常不同：相反，你的文档是一个纯文本文件，其中穿插着用于表达所需（排版）结果的 LaTeX *命令*。为了生成可见的排版文档，您的 LaTeX 文件由一个称为 *TeX 引擎*的软件处理，该软件使用嵌入在文本文件中的命令来指导和控制排版过程，将 LaTeX 命令和文档文本转换为专业排版的 PDF 文件。这意味着您只需关注文档*的内容*，计算机通过 LaTeX 命令和 TeX 引擎将负责*视觉外观*（格式）。

## Why learn LaTeX? 为什么要学习 LaTeX？

Various arguments can be proposed for, or against, learning to use LaTeX instead of other document-authoring applications; but, ultimately, it is a personal choice based on preferences, affinities, and documentation requirements.
可以提出各种支持或反对学习使用 LaTeX 而不是其他文档创作应用程序的论点;但是，归根结底，这是基于偏好、亲和力和文档要求的个人选择。

Arguments in favour of LaTeX include:
支持 LaTeX 的论点包括：

- support for typesetting extremely complex mathematics, tables and technical content for the physical sciences;
  支持对物理科学的极其复杂的数学、表格和技术内容进行排版;
- facilities for footnotes, cross-referencing and management of bibliographies;
  脚注、交叉引用和书目管理设施;
- ease of producing complicated, or tedious, document elements such as indexes, glossaries, table of contents, lists of figures;
  易于制作复杂或乏味的文档元素，例如索引、词汇表、目录、图表列表;
- being highly customizable for bespoke document production due to its intrinsic programmability and extensibility through thousands of [free add-on packages](https://www.ctan.org/pkg).
  由于其固有的可编程性和可扩展性，可通过数千个[免费的附加组件包](https://www.ctan.org/pkg)进行高度定制，用于定制文档制作。

Overall, LaTeX provides users with a great deal of control over the production of documents which are typeset to extremely high standards. Of course, there are types of documents or publications where LaTeX doesn’t shine, including many “free form” page designs typically found in magazine-type publications.
总体而言，LaTeX 为用户提供了对排版为极高标准的文档制作的巨大控制权。当然，有些类型的文档或出版物 LaTeX 并不闪耀，包括许多通常在杂志类型出版物中发现的 “自由格式” 页面设计。

One important benefit of LaTeX is the separation of document content from document style: once you have written the content of your document, its appearance can be changed with ease. Similarly, you can create a LaTeX file which defines the layout/style of a particular document type and that file can be used as a *template* to standardise authorship/production of additional documents of that type; for example, this allows scientific publishers to create article templates, in LaTeX, which authors use to write papers for submission to journals. Overleaf has a [gallery containing thousands of templates](https://www.overleaf.com/gallery), covering an enormous range of document types—everything from scientific articles, reports and books to CVs and presentations. Because these templates define the layout and style of the document, authors need only to open them in Overleaf—creating a new project—and commence writing to add their content.
LaTeX 的一个重要好处是将文档内容与文档样式分离：一旦你编写了文档的内容，就可以轻松更改其外观。同样，您可以创建一个 LaTeX 文件来定义特定文档类型的布局/样式，并且该文件可以用作*模板*来标准化该类型其他文档的作者身份/制作;例如，这允许科学出版商在 LaTeX 中创建文章模板，作者可以使用该模板撰写论文以提交给期刊。Overleaf 有一个[包含数千个模板的画廊](https://www.overleaf.com/gallery)，涵盖了大量的文档类型——从科学文章、报告和书籍到简历和演示文稿，应有尽有。由于这些模板定义了文档的布局和样式，因此作者只需在 Overleaf 中打开它们（创建新项目）并开始编写以添加其内容。

## Writing your first piece of LaTeX 编写你的第一篇 LaTeX

The first step is to create a new LaTeX project. You can do this on your own computer by creating a new `.tex` file; alternatively, you can [start a new project in Overleaf](https://www.overleaf.com/learn/latex/Creating_a_document_in_Overleaf).
第一步是创建一个新的 LaTeX 项目。您可以通过创建新的 `.tex` 文件在自己的计算机上执行此操作;或者，您可以在 [Overleaf 中启动一个新项目](https://www.overleaf.com/learn/latex/Creating_a_document_in_Overleaf)。

Let’s start with the simplest working example, which can be opened directly in Overleaf:
让我们从最简单的工作示例开始，可以直接在 Overleaf 中打开：



```
\documentclass{article}
\begin{document}
First document. This is a simple example, with no 
extra parameters or packages included.
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Simplest+working+example+LaTeX+document&snip=\documentclass{article} \begin{document} First+document.+This+is+a+simple+example%2C+with+no+ extra+parameters+or+packages+included. \end{document})



This example produces the following output:
此示例生成以下输出：

![Example document](https://images.ctfassets.net/nrgyaltdicpt/5oBbZABsWEnHZpwhfvV2PD/95ba7d5496616b4f10dffe6fb90f578a/LL30Fig1-plain.svg)



You can see that LaTeX has automatically indented the first line of the paragraph, taking care of that formatting for you. Let’s have a closer look at what each part of our code does.
你可以看到 LaTeX 已经自动缩进了段落的第一行，为你处理了该格式。让我们仔细看看代码的每个部分都做了什么。

The first line of code, `\documentclass{article}`, declares the document type known as its *class*, which controls the overall appearance of the document. Different types of documents require different classes; i.e., a CV/resume will require a different class than a scientific paper which might use the standard LaTeX `article` class. Other types of documents you may be working on may require different classes such as `book` or `report`. To get some idea of the many LaTeX class types available, [visit the relevant page on CTAN (Comprehensive TeX Archive Network)](https://www.ctan.org/topic/class).
第一行代码 `\documentclass{article}` 声明称为*其类*的文档类型，它控制文档的整体外观。不同类型的文档需要不同的类;即，简历/简历需要与可能使用标准 LaTeX`文章`类的科学论文不同的类。您可能正在处理的其他类型的文档可能需要不同的类，例如`书籍`或`报告`。要了解许多可用的 LaTeX 类类型，[请访问 CTAN （Comprehensive TeX Archive Network） 上的相关页面](https://www.ctan.org/topic/class)。

Having set the document class, our content, known as the *body* of the document, is written between the `\begin{document}` and `\end{document}` tags. After opening the example above, you can make changes to the text and, when finished, view the resulting typeset PDF by *recompiling the document*. To do this in Overleaf, simply hit **Recompile**, as demonstrated in this brief video clip:
设置文档类后，我们的内容（称为文档*正文*）被写入 `\begin{document}` 和 `\end{document}` 标签之间。打开上面的示例后，您可以对文本进行更改，并在完成后通过*重新编译文档*来查看生成的排版 PDF。要在 Overleaf 中执行此操作，只需点击 **Recompile**，如以下简短视频剪辑所示：



<video controls="" width="100%" height="100%" src="https://videos.ctfassets.net/nrgyaltdicpt/6yo2PA5aMV3OEZl5NtZKWu/54395f569b830b8183b5e0058d5bc0cc/LL30recompile.mp4" type="video/mp4" data-immersive-translate-walked="aafa2316-ff14-4d3d-9e7a-98c009c61058" style="box-sizing: border-box; display: inline-block; vertical-align: baseline;"></video>



Any Overleaf project can be configured to recompile automatically each time it is edited: click the small arrow next to the **Recompile** button and set **Auto Compile** to **On**, as shown in the following screengrab:
任何 Overleaf 项目都可以配置为在每次编辑时自动重新编译：单击 **Recompile** 按钮旁边的小箭头，并将 **Auto Compile** 设置为 **On**，如下面的屏幕截图所示：

![Screengrab showing how to set Auto Compile to On or Off](https://sharelatex-wiki-cdn-671420.c.cdn77.org/learn-scripts/images/7/77/LL30autocompile.png)

Having seen how to add content to our document, the next step is to give it a title. To do this, we must talk briefly about the **preamble**.
在了解了如何向文档添加内容后，下一步是给它一个标题。要做到这一点，我们必须简要地谈谈**序言**。

## The preamble of a document 文档的序言

The screengrab above shows Overleaf storing a LaTeX document as a file called `main.tex`: the `.tex` file extension is, by convention, used when naming files containing your document’s LaTeX code.
上面的屏幕截图显示了 Overleaf 将 LaTeX 文档存储为名为 `main.tex` 的文件：按照惯例，在命名包含文档 LaTeX 代码的文件时，会使用 `.tex` 文件扩展名。

The previous example showed how document content was entered after the `\begin{document}` command; however, everything in your `.tex` file appearing *before* that point is called the *preamble*, which acts as the document’s “setup” section. Within the preamble you define the document class (type) together with specifics such as languages to be used when writing the document; loading *packages* you would like to use (more on this [later](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages)), and it is where you’d apply other types of configuration.
前面的示例显示了如何在 `\begin{document}` 命令之后输入文档内容;但是，`.tex` 文件中出现在该点*之前*的所有内容都称为 *preamble*，它充当文档的 “setup” 部分。在序言中，定义文档类（类型）以及具体信息，例如编写文档时要使用的语言;loading 你想使用的*包*（[稍后](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages)会详细介绍），这是你将应用其他类型配置的地方。

A minimal document preamble might look like this:
最小文档序言可能如下所示：



```
\documentclass[12pt, letterpaper]{article}
\usepackage{graphicx}
```



where `\documentclass[12pt, letterpaper]{article}` defines the overall class (type) of document. Additional parameters, which must be separated by commas, are included in square brackets (`[...]`) and used to configure this instance of the article class; i.e., settings we wish to use for this particular `article`-class-based document.
其中 `\documentclass[12pt, letterpaper]{article}` 定义 document 的整体类 （类型）。其他参数（必须用逗号分隔）包含在方括号 （`[...]`） 中，用于配置 article 类的此实例;即，我们希望用于这个特定的`基于文章`类的文档的设置。

In this example, the two parameters do the following:
在此示例中，这两个参数执行以下操作：

- `12pt` sets the font size
  `12pt` 设置字体大小
- `letterpaper` sets the paper size
  `letterpaper` 设置纸张大小

Of course other font sizes, `9pt`, `11pt`, `12pt`, can be used, but if none is specified, the default size is `10pt`. As for the paper size, other possible values are `a4paper` and `legalpaper`. For further information see the article about [page size and margins](https://www.overleaf.com/learn/latex/Page_size_and_margins).
当然，也可以使用其他字体大小，`9pt`、`11pt`、`12pt`，但如果未指定，则默认大小为 `10pt`。至于纸张大小，其他可能的值是 `a4paper` 和 `legalpaper`。有关更多信息，请参阅有关[页面大小和边距的](https://www.overleaf.com/learn/latex/Page_size_and_margins)文章。

The preamble line  序言行



```
\usepackage{graphicx}
```



is an example of loading an external package (here, [`graphicx`](https://ctan.org/pkg/graphicx?lang=en)) to extend LaTeX’s capabilities, enabling it to import external graphics files. LaTeX packages are discussed in the section [Finding and using LaTeX packages](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages).
是加载外部包（此处为 [`graphicX`](https://ctan.org/pkg/graphicx?lang=en)）以扩展 LaTeX 功能的示例，使其能够导入外部图形文件。LaTeX 包在 查找和使用 LaTeX 包一节中讨论。

## Including title, author and date information 包括标题、作者和日期信息

Adding a title, author and date to our document requires three more lines in the *preamble* (*not* the main body of the document). Those lines are:
向文档添加标题、作者和日期需要在*序言*中再添加三行（*不是*文档的主体）。这些行是：

- `\title{My first LaTeX document}`: the document title
  `\title{My first LaTeX document}` ：文档标题

- ```
  \author{Hubert Farnsworth}
  ```

  : here you write the name of the author(s) and, optionally, the

   

  ```
  \thanks
  ```

   

  command within the curly braces:

  
  `\author{Hubert Farnsworth}`：在这里，您可以写下作者的姓名，也可以选择在大括号内写下 `\thank` 命令：

  - `\thanks{Funded by the Overleaf team.}`: can be added after the name of the author, inside the braces of the `author` command. It will add a superscript and a footnote with the text inside the braces. Useful if you need to thank an institution in your article.
    `\thanks{Funded by the Overleaf team.}` ：可以添加到作者姓名之后，在 `author` 命令的大括号内。它将添加一个上标和一个脚注，并在大括号内添加文本。如果您需要在文章中感谢某个机构，这很有用。

- `\date{August 2022}`: you can enter the date manually or use the command `\today` to typeset the current date every time the document is compiled
  `\date{2022 年 8 月}`：您可以手动输入日期，也可以在每次编译文档时使用命令 `\today` 排版当前日期

With these lines added, your preamble should look something like this:
添加这些行后，您的序言应如下所示：



```
\documentclass[12pt, letterpaper]{article}
\title{My first LaTeX document}
\author{Hubert Farnsworth\thanks{Funded by the Overleaf team.}}
\date{August 2022}
```



To typeset the title, author and date use the `\maketitle` command within the *body* of the document:
要排版标题、作者和日期，请在文档*正文*中使用 `\maketitle` 命令：



```
\begin{document}
\maketitle
We have now added a title, author and date to our first \LaTeX{} document!
\end{document}
```



The preamble and body can now be combined to produce a complete document which can be opened in Overleaf:
序言和正文现在可以组合起来生成一个完整的文档，可以在 Overleaf 中打开：



```
\documentclass[12pt, letterpaper]{article}
\title{My first LaTeX document}
\author{Hubert Farnsworth\thanks{Funded by the Overleaf team.}}
\date{August 2022}
\begin{document}
\maketitle
We have now added a title, author and date to our first \LaTeX{} document!
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=My+first+LaTeX+document&snip=\documentclass[12pt%2C+letterpaper]{article} \title{My+first+LaTeX+document} \author{Hubert+Farnsworth\thanks{Funded+by+the+Overleaf+team.}} \date{August+2022} \begin{document} \maketitle We+have+now+added+a+title%2C+author+and+date+to+our+first+\LaTeX{}+document! \end{document})



This example produces the following output:
此示例生成以下输出：

![Image of a simple document produced in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/3WzMd0bx2zlj3zLTKS8SxT/dc2b7c16adbc96bdd750b6d2c8b4227e/LL30Fig2r-plain.svg)



## Adding comments 添加评论

LaTeX is a form of “program code”, but one which specializes in document typesetting; consequently, as with code written in any other programming language, it can be very useful to include comments within your document. A LaTeX comment is a section of text that will not be typeset or affect the document in any way—often used to add “to do” notes; include explanatory notes; provide in-line explanations of tricky macros or comment-out lines/sections of LaTeX code when debugging.
LaTeX 是 “程序代码” 的一种形式，但专门用于文档排版;因此，与用任何其他编程语言编写的代码一样，在文档中包含注释可能非常有用。LaTeX 注释是一段不会排版或以任何方式影响文档的文本——通常用于添加“待办事项”注释;包括解释性说明;在调试时提供 LaTeX 代码的棘手宏或注释掉行/部分的内联解释。

To make a comment in LaTeX, simply write a `%` symbol at the beginning of the line, as shown in the following code which uses the example above:
要在 LaTeX 中进行注释，只需在行的开头写一个 `%` 符号，如下面的代码所示，该代码使用了上面的示例：



```
\documentclass[12pt, letterpaper]{article}
\title{My first LaTeX document}
\author{Hubert Farnsworth\thanks{Funded by the Overleaf team.}}
\date{August 2022}
\begin{document}
\maketitle
We have now added a title, author and date to our first \LaTeX{} document!

% This line here is a comment. It will not be typeset in the document.
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=My+first+LaTeX+document+with+a+comment&snip=\documentclass[12pt%2C+letterpaper]{article} \title{My+first+LaTeX+document} \author{Hubert+Farnsworth\thanks{Funded+by+the+Overleaf+team.}} \date{August+2022} \begin{document} \maketitle We+have+now+added+a+title%2C+author+and+date+to+our+first+\LaTeX{}+document! %+This+line+here+is+a+comment.+It+will+not+be+typeset+in+the+document. \end{document})



This example produces output that is identical to the previous LaTeX code which did not contain the comment.
此示例生成的输出与前面的 LaTeX 代码相同，该代码不包含注释。

## Bold, italics and underlining 粗体、斜体和下划线

Next, we will now look at some text formatting commands:
接下来，我们现在将查看一些文本格式化命令：

- **Bold**: bold text in LaTeX is typeset using the `\textbf{...}` command.
  **粗体**：LaTeX 中的粗体文本使用 `\textbf{...}` 命令进行排版。
- *Italics*: italicised text is produced using the `\textit{...}` command.
  *斜体*：使用 `\textit{...}` 命令生成斜体文本。
- Underline: to underline text use the `\underline{...}` command.
  Underline：要使用 `\underline{...}` 命令为文本添加下划线。

The next example demonstrates these commands:
下一个示例演示了这些命令：



```
Some of the \textbf{greatest}
discoveries in \underline{science} 
were made by \textbf{\textit{accident}}.
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=First+example+with+formatted+text&snip=\documentclass[12pt%2C+letterpaper]{article} \title{My+first+LaTeX+document} \author{Hubert+Farnsworth\thanks{Funded+by+the+Overleaf+team.}} \date{August+2022} \begin{document} \maketitle Some+of+the+\textbf{greatest} discoveries+in+\underline{science}+ were+made+by+\textbf{\textit{accident}}. \end{document})



This example produces the following output:
此示例生成以下输出：

![Imate showing text formatted in a LaTeX document](https://images.ctfassets.net/nrgyaltdicpt/6vo15r0tLCByTpcvn1w2E8/8f14edc7ece1f10ce4ba2c76e1e58a56/LL30Fig3r-plain.svg)



Another very useful command is `\emph{*argument*}`, whose effect on its `*argument*` depends on the context. Inside normal text, the emphasized text is italicized, but this behaviour is reversed if used inside an italicized text—see the next example:
另一个非常有用的命令是 `\emph{*argument*}`，它对其`*参数*`的影响取决于上下文。在普通文本中，强调的文本是斜体的，但如果在斜体文本中使用，则此行为将相反 - 请参阅下一个示例：



```
Some of the greatest \emph{discoveries} in science 
were made by accident.

\textit{Some of the greatest \emph{discoveries} 
in science were made by accident.}

\textbf{Some of the greatest \emph{discoveries} 
in science were made by accident.}
```

[ Open this `**\emph**` example in Overleaf.
在 Overleaf 中打开这个 `**\emph**` 示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Using+the+emph+command&snip=\documentclass[12pt%2C+letterpaper%2C+twoside]{article} \title{My+first+LaTeX+document} \author{Hubert+Farnsworth\thanks{Funded+by+the+Overleaf+team.}} \date{August+2022} \begin{document} \parindent0pt%+To+remove+the+paragraph+indentation \maketitle Some+of+the+greatest+\emph{discoveries}+in+science+ were+made+by+accident. \textit{Some+of+the+greatest+\emph{discoveries}+ in+science+were+made+by+accident.} \textbf{Some+of+the+greatest+\emph{discoveries}+ in+science+were+made+by+accident.} \end{document})



This example produces the following output:
此示例生成以下输出：

![Image demonstrating use of the LaTeX \emph command](https://images.ctfassets.net/nrgyaltdicpt/1K0A8RXXOomakJBAr2usmp/62d0e8b5275092dd0b1b4a59c745b632/LL30Fig4r-plain.svg)



- **Note:** some packages, such as [Beamer](https://www.overleaf.com/learn/latex/Beamer), change the behaviour of the `\emph` command.
  **注意：**某些软件包（例如 [Beamer](https://www.overleaf.com/learn/latex/Beamer)）会更改 `\emph` 命令的行为。

## Adding images 添加图片

In this section we will look at how to add images to a LaTeX document. Overleaf supports three ways to insert images:
在本节中，我们将了解如何向 LaTeX 文档添加图像。Overleaf 支持三种插入图像的方式：

1. Use the [**Insert Figure** button](https://learn.overleaf.com/learn/Kb/How_to_insert_figures_in_Overleaf#Using_Insert_Figure_to_add_a_figure_to_your_project)(![The Insert Figure button on the editor toolbar](https://sharelatex-wiki-cdn-671420.c.cdn77.org/learn-scripts/images/a/a8/InsertFigureButton.png)), located on the editor toolbar, to insert an image into **Visual Editor** or **Code Editor**.
   使用编辑器工具栏上的 [**Insert Figure** button](https://learn.overleaf.com/learn/Kb/How_to_insert_figures_in_Overleaf#Using_Insert_Figure_to_add_a_figure_to_your_project)（ ![The Insert Figure button on the editor toolbar](https://sharelatex-wiki-cdn-671420.c.cdn77.org/learn-scripts/images/a/a8/InsertFigureButton.png) ） 将图像插入**到可视编辑器**或**代码编辑器中**。
2. [Copy and paste an image](https://www.overleaf.com/learn/how-to/How_to_paste_formatted_content_into_Overleaf%23Pasting_images_into_your_Overleaf_project) into **Visual Editor** or **Code Editor**.
   [将图像复制并粘贴到](https://www.overleaf.com/learn/how-to/How_to_paste_formatted_content_into_Overleaf%23Pasting_images_into_your_Overleaf_project) **Visual Editor** 或 **Code Editor** 中。
3. Use **Code Editor** to write LaTeX code that inserts a graphic.
   使用 **Code Editor** 编写插入图形的 LaTeX 代码。

Options 1 and 2 automatically generate the LaTeX code required to insert images, but here we introduce option 3—note that you will need to [upload those images](https://www.overleaf.com/learn/how-to/Including_images_on_Overleaf) to your Overleaf project. The following example demonstrates how to include a picture:
选项 1 和 2 自动生成插入图像所需的 LaTeX 代码，但这里我们介绍选项 3 — 请注意，您需要[将这些图像上传到](https://www.overleaf.com/learn/how-to/Including_images_on_Overleaf) Overleaf 项目。以下示例演示如何包含图片：



```
\documentclass{article}
\usepackage{graphicx} %LaTeX package to import graphics
\graphicspath{{images/}} %configuring the graphicx package
 
\begin{document}
The universe is immense and it seems to be homogeneous, 
on a large scale, everywhere we look.

% The \includegraphics command is 
% provided (implemented) by the 
% graphicx package
\includegraphics{universe}  
 
There's a picture of a galaxy above.
\end{document}
```



[ Open this image example in Overleaf.
在 Overleaf 中打开此图像示例。](https://www.overleaf.com/project/new/template/25686?id=107971142&templateName=Example+using+images+in+LaTeX&latexEngine=pdflatex&texImage=texlive-full%3A2022.1&mainFile=)

This example produces the following output:
此示例生成以下输出：

![Graphic showing an image imported into a LaTeX document](https://images.ctfassets.net/nrgyaltdicpt/4p5toat08FUgehv4yuNwXS/efc9e75e4342c9caeec94f26627fa337/LL30Fig5v2-plain.svg)



Importing graphics into a LaTeX document needs [an add-on *package*](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages) which provides the commands and features required to include external graphics files. The above example loads the [`graphicx` package](https://ctan.org/pkg/graphicx?lang=en) which, among many other commands, provides `\includegraphics{...}` to import graphics and `\graphicspath{...}` to advise LaTeX where the graphics are located.
将图形导入 LaTeX 文档需要一个[附加*包*](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages)，该包提供包含外部图形文件所需的命令和功能。上面的示例加载了 [`graphicx` 包](https://ctan.org/pkg/graphicx?lang=en)，除了许多其他命令外，它还提供 `\includegraphics{...}` 来导入图形，并提供 `\graphicspath{...}` 来告知 LaTeX 图形的位置。

To use the `graphicx` package, include the following line in your Overleaf document preamble:
要使用 `graphicx` 包，请在 Overleaf 文档序言中包含以下行：



```
\usepackage{graphicx}
```



In our example the command `\graphicspath{{images/}}` informs LaTeX that images are kept in a folder named `images`, which is contained in the current directory:
在我们的示例中，命令 `\graphicspath{{images/}}` 通知 LaTeX 图像保存在名为 `images` 的文件夹中，该文件夹包含在当前目录中：

![Image showing LaTeX accessing images stored in a folder](https://sharelatex-wiki-cdn-671420.c.cdn77.org/learn-scripts/images/1/17/ImagesInAFolder.png)

The `\includegraphics{universe}` command does the actual work of inserting the image in the document. Here, `universe` is the name of the image file but without its extension.
`\includegraphics{universe}` 命令执行在文档中插入图像的实际工作。此处，`universe` 是图像文件的名称，但没有其扩展名。

**Note**:  **注意**：

- Although the full file name, including its extension, is allowed in the `\includegraphics` command, it’s considered best practice to omit the file extension because it will prompt LaTeX to search for all the supported formats.
  尽管 `\includegraphics` 命令允许使用完整的文件名，包括其扩展名，但省略文件扩展名被认为是最佳实践，因为它会提示 LaTeX 搜索所有支持的格式。
- Generally, the graphic’s file name should not contain white spaces or multiple dots; it is also recommended to use lowercase letters for the file extension when uploading image files to Overleaf.
  通常，图形的文件名不应包含空格或多个点;此外，还建议在将图像文件上传到 Overleaf 时使用小写字母作为文件扩展名。

More information on LaTeX packages can be found at the end of this tutorial in the section [Finding and using LaTeX packages](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages).
有关 LaTeX 包的更多信息，请参阅本教程末尾的 [查找和使用 LaTeX 包](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Finding_and_using_LaTeX_packages)部分。

## Captions, labels and references 标题、标签和引用

Images can be captioned, labelled and referenced by means of the `figure` environment, as shown below:
可以通过 `figure` 环境对图像进行标题、标记和引用，如下所示：



```
\documentclass{article}
\usepackage{graphicx}
\graphicspath{{images/}}
 
\begin{document}

\begin{figure}[h]
    \centering
    \includegraphics[width=0.75\textwidth]{mesh}
    \caption{A nice plot.}
    \label{fig:mesh1}
\end{figure}
 
As you can see in figure \ref{fig:mesh1}, the function grows near the origin. This example is on page \pageref{fig:mesh1}.

\end{document}
```



[ Open this image example in Overleaf.
在 Overleaf 中打开此图像示例。](https://www.overleaf.com/project/new/template/25519?id=107980830&templateName=Example+using+image+captions+in+LaTeX&latexEngine=pdflatex&texImage=texlive-full%3A2022.1&mainFile=)

This example produces the following output:
此示例生成以下输出：

![Graphic showing use of figure captions in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/4DkAWWkQqZP6QHU2EErogQ/9aa2371f2cde0f3f8bf22aa1c0b91789/LL30Fig6r-plain.svg)



There are several noteworthy commands in the example:
示例中有几个值得注意的命令：

- **`\includegraphics[width=0.75\textwidth]{mesh}`**: This form of `\includegraphics` instructs LaTeX to set the figure’s width to 75% of the text width—whose value is stored in the `\textwidth` command.
  **`\includegraphics[width=0.75\textwidth]{mesh}`** ： 这种形式的 `\includegraphics` 指示 LaTeX 将图形的宽度设置为文本宽度的 75%，其值存储在 `\textwidth` 命令中。

- **`\caption{A nice plot.}`**: As its name suggests, this command sets the figure caption which can be placed above or below the figure. If you create a list of figures this caption will be used in that list.
  **`\caption{A nice plot.}`**： 顾名思义，此命令设置可以放置在图形上方或下方的图形标题。如果您创建一个图表列表，则此标题将在该列表中使用。

- **`\label{fig:mesh1}`**: To reference this image within your document you give it a label using the `\label` command. The label is used to generate a number for the image and, combined with the next command, will allow you to reference it.
  **`\label{fig：mesh1}`**： 要在文档中引用此图像，请使用 `\label` 命令为其指定标签。标签用于为图像生成一个数字，并与下一个命令结合使用，将允许您引用它。

- **`\ref{fig:mesh1}`**: This code will be substituted by the number corresponding to the referenced figure.
  **`\ref{fig：mesh1}`**： 此代码将被与引用图对应的数字替换。

Images incorporated in a LaTeX document should be placed inside a `figure` environment, or similar, so that LaTeX can automatically position the image at a suitable location in your document.
包含在 LaTeX 文档中的图像应放置在`图形`环境或类似环境中，以便 LaTeX 可以自动将图像放置在文档中的适当位置。

Further guidance is contained in the following Overleaf help articles:
以下 Overleaf 帮助文章中包含进一步的指导：

- [Positioning of Figures 图形的定位](https://www.overleaf.com/learn/latex/Positioning_of_Figures)
- [Inserting Images 插入图像](https://www.overleaf.com/learn/latex/Inserting_Images)

## Creating lists in LaTeX 在 LaTeX 中创建列表

You can create different types of list using *environments*, which are used to encapsulate the LaTeX code required to implement a specific typesetting feature. An environment starts with `\begin{*environment-name*}` and ends with `\end{*environment-name*}` where `*environment-name*` might be `figure`, `tabular` or one of the list types: `itemize` for unordered lists or `enumerate` for ordered lists.
您可以使用环境创建不同类型的列表，这些*环境*用于封装实现特定排版功能所需的 LaTeX 代码。环境以 `\begin{*environment-name*}` 开头，以 `\end{*environment-name*}` 结尾，其中 `*environment-name*` 可以是`数字`、`表格`或列表类型之一：`itemize` 表示无序列表，枚举 （`enumerate`） 表示有序列表。

### Unordered lists 无序列表

Unordered lists are produced by the `itemize` environment. Each list entry must be preceded by the `\item` command, as shown below:
无序列表由 `itemize` 环境生成。每个列表条目前面必须有 `\item` 命令，如下所示：



```
\documentclass{article}
\begin{document}
\begin{itemize}
  \item The individual entries are indicated with a black dot, a so-called bullet.
  \item The text in the entries may be of any length.
\end{itemize}
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Example+of+a+LaTeX+unordered+list&snip=\documentclass{article} \begin{document} \begin{itemize} ++\item+The+individual+entries+are+indicated+with+a+black+dot%2C+a+so-called+bullet. ++\item+The+text+in+the+entries+may+be+of+any+length. \end{itemize} \end{document})



This example produces the following output:
此示例生成以下输出：

![An example of bulleted lists in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/1lDj29Mg9ZuLNHXwZrTJew/cd7d950c65fd05b251c4aa55746f4eb7/LL30Fig7-plain.svg)



You can also open this [ larger Overleaf project](https://www.overleaf.com/project/new/template/25521?id=107987258&templateName=Demonstrating+various+types+of+LaTeX+list&latexEngine=pdflatex&texImage=texlive-full%3A2022.1&mainFile=) which demonstrates various types of LaTeX list.
你也可以打开这个[ 更大的 Overleaf 项目](https://www.overleaf.com/project/new/template/25521?id=107987258&templateName=Demonstrating+various+types+of+LaTeX+list&latexEngine=pdflatex&texImage=texlive-full%3A2022.1&mainFile=) 它演示了各种类型的 LaTeX 列表。

### Ordered lists 有序列表

Ordered lists use the same syntax as unordered lists but are created using the `enumerate` environment:
有序列表使用与无序列表相同的语法，但使用 `enumerate` 环境创建：



```
\documentclass{article}
\begin{document}
\begin{enumerate}
  \item This is the first entry in our list.
  \item The list numbers increase with each entry we add.
\end{enumerate}
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Example+of+the+enumerate+environment&snip=\documentclass{article} \begin{document} \begin{enumerate} ++\item+This+is+the+first+entry+in+our+list. ++\item+The+list+numbers+increase+with+each+entry+we+add. \end{enumerate} \end{document})



This example produces the following output:
此示例生成以下输出：

![An example numbered list produced in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/2vkfa7RiAIJxv5wIZbg9UK/530c384f159d091a587de279d13fefec/LL30Fig8-plain.svg)



As with `unordered` lists, each entry must be preceded by the `\item` command which, here, automatically generates the numeric ordered-list label value, starting at 1.
与`无序列`表一样，每个条目前面都必须有 `\item` 命令，该命令在这里自动生成数字有序列表标签值，从 1 开始。

For further information you can open this [ larger Overleaf project](https://www.overleaf.com/project/new/template/25521?id=107987258&templateName=Demonstrating+various+types+of+LaTeX+list&latexEngine=pdflatex&texImage=texlive-full%3A2022.1&mainFile=) which demonstrates various types of LaTeX list or visit our dedicated [help article on LaTeX lists](https://www.overleaf.com/learn/latex/Lists), which provides many more examples and shows how to create customized lists.
有关更多信息，您可以打开这个[ 更大的 Overleaf 项目](https://www.overleaf.com/project/new/template/25521?id=107987258&templateName=Demonstrating+various+types+of+LaTeX+list&latexEngine=pdflatex&texImage=texlive-full%3A2022.1&mainFile=) ，该列表演示了各种类型的 LaTeX 列表，或者访问我们关于 LaTeX 列表的专门帮助文章，该文章提供了更多示例并展示了如何创建自定义列表。

## Adding math to LaTeX 向 LaTeX 添加数学运算

One of the main advantages of LaTeX is the ease with which mathematical expressions can be written. LaTeX provides two writing modes for typesetting mathematics:
LaTeX 的主要优点之一是可以轻松编写数学表达式。LaTeX 提供了两种排版数学的书写模式：

- *inline* math mode used for writing formulas that are part of a paragraph
  *内联*数学模式，用于编写属于段落的公式
- *display* math mode used to write expressions that are not part of a text or paragraph and are typeset on separate lines
  *显示*数学模式，用于编写不属于文本或段落且排版在单独行上的表达式

### Inline math mode 内联数学模式

Let’s see an example of inline math mode:
让我们看一个内联数学模式的例子：



```
\documentclass[12pt, letterpaper]{article}
\begin{document}
In physics, the mass-energy equivalence is stated 
by the equation $E=mc^2$, discovered in 1905 by Albert Einstein.
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Inline+LaTeX+maths+example&snip=\documentclass[12pt%2C+letterpaper]{article} \begin{document} In+physics%2C+the+mass-energy+equivalence+is+stated+ by+the+equation+%24E%3Dmc^2%24%2C+discovered+in+1905+by+Albert+Einstein. \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing math typeset in inline math mode](https://images.ctfassets.net/nrgyaltdicpt/77oK8pfew1B1VvxiBtALag/15714f2da4e469bbb8cf70a0d3733e5d/LL30Fig9-plain.svg)



To typeset inline-mode math you can use one of these delimiter pairs: `\( ... \)`, `$ ... $` or `\begin{math} ... \end{math}`, as demonstrated in the following example:
要对内联模式数学进行排版，您可以使用以下分隔符对之一：\`（ ... \）`、`$ ... $` 或 `\begin{math} ... \end{math}`，如以下示例所示：



```
\documentclass[12pt, letterpaper]{article}
\begin{document}
\begin{math}
E=mc^2
\end{math} is typeset in a paragraph using inline math mode---as is $E=mc^2$, and so too is \(E=mc^2\).
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Demonstrating+inline+math+mode&snip=\documentclass[12pt%2C+letterpaper]{article} \begin{document} \begin{math} E%3Dmc^2 \end{math}+is+typeset+in+a+paragraph+using+inline+math+mode---as+is+%24E%3Dmc^2%24%2C+and+so+too+is+\(E%3Dmc^2\). \end{document})



This example produces the following output:
此示例生成以下输出：

![Image demonstrating content produced using LaTeX inline math mode](https://images.ctfassets.net/nrgyaltdicpt/46VPfEGxYJ3di18TLzaLo9/ed67df07532c52b6543fd2bae7cb7c04/LL30Fig10r-plain.svg)



### Display math mode 显示数学模式

Equations typeset in display mode can be numbered or unnumbered, as in the following example:
在显示模式下排版的方程式可以是编号的，也可以是未编号的，如以下示例所示：



```
\documentclass[12pt, letterpaper]{article}
\begin{document}
The mass-energy equivalence is described by the famous equation
\[ E=mc^2 \] discovered in 1905 by Albert Einstein. 

In natural units ($c = 1$), the formula expresses the identity
\begin{equation}
E=m
\end{equation}
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Display+math+mode+example&snip=\documentclass[12pt%2C+letterpaper]{article} \begin{document} The+mass-energy+equivalence+is+described+by+the+famous+equation \[+E%3Dmc^2+\]+discovered+in+1905+by+Albert+Einstein.+ In+natural+units+(%24c+%3D+1%24)%2C+the+formula+expresses+the+identity \begin{equation} E%3Dm \end{equation} \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing display mode math in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/6n1FPYFzmzCHPpWoEoYQZM/79b33f1096be06326bff7d2e1976c67c/LL30Fig11-plain.svg)



To typeset display-mode math you can use one of these delimiter pairs: `\[ ... \]`, `\begin{displaymath} ... \end{displaymath}` or `\begin{equation} ... \end{equation}`. Historically, typesetting display-mode math required use of `$$` characters delimiters, as in `$$ *... display math here ...*$$`, but this method [is no longer recommended](https://texfaq.org/FAQ-dolldoll): use LaTeX’s delimiters `\[ ... \]` instead.
要对显示模式数学进行排版，可以使用以下分隔符对之一：\`[ ... \]` `\begin{displaymath} ... \end{displaymath}` 或 `\begin{equation} ... \end{equation}` .从历史上看，排版显示模式数学需要使用 `$$` 个字符的分隔符，如 `$$ *... display math here ...*$$` ，但现在[不再推荐](https://texfaq.org/FAQ-dolldoll)这种方法：改用 LaTeX 的分隔符 `\[ ... \]。`

### More complete examples 更完整的示例

The following examples demonstrate a range of mathematical content typeset using LaTeX.
以下示例演示了使用 LaTeX 的一系列数学内容排版。



```
\documentclass{article}
\begin{document}
Subscripts in math mode are written as $a_b$ and superscripts are written as $a^b$. These can be combined and nested to write expressions such as

\[ T^{i_1 i_2 \dots i_p}_{j_1 j_2 \dots j_q} = T(x^{i_1},\dots,x^{i_p},e_{j_1},\dots,e_{j_q}) \]
 
We write integrals using $\int$ and fractions using $\frac{a}{b}$. Limits are placed on integrals using superscripts and subscripts:

\[ \int_0^1 \frac{dx}{e^x} =  \frac{e-1}{e} \]

Lower case Greek letters are written as $\omega$ $\delta$ etc. while upper case Greek letters are written as $\Omega$ $\Delta$.

Mathematical operators are prefixed with a backslash as $\sin(\beta)$, $\cos(\alpha)$, $\log(x)$ etc.
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=More+advanced+LaTeX+math+example&snip=\documentclass{article} \begin{document} Subscripts+in+math+mode+are+written+as+%24a_b%24+and+superscripts+are+written+as+%24a^b%24.+These+can+be+combined+and+nested+to+write+expressions+such+as \[+T^{i_1+i_2+\dots+i_p}_{j_1+j_2+\dots+j_q}+%3D+T(x^{i_1}%2C\dots%2Cx^{i_p}%2Ce_{j_1}%2C\dots%2Ce_{j_q})+\] + We+write+integrals+using+%24\int%24+and+fractions+using+%24\frac{a}{b}%24.+Limits+are+placed+on+integrals+using+superscripts+and+subscripts%3A \[+\int_0^1+\frac{dx}{e^x}+%3D++\frac{e-1}{e}+\] Lower+case+Greek+letters+are+written+as+%24\omega%24+%24\delta%24+etc.+while+upper+case+Greek+letters+are+written+as+%24\Omega%24+%24\Delta%24. Mathematical+operators+are+prefixed+with+a+backslash+as+%24\sin(\beta)%24%2C+%24\cos(\alpha)%24%2C+%24\log(x)%24+etc. \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing a range of math typeset in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/5xfm4NybWckHL5ndpdnBRq/bc0b5e27044820ea5cdd11648a68f543/LL30Fig12r-plain.svg)



The next example uses the `equation*` environment which is provided by the `amsmath` package, so we need to add the following line to our document preamble:
下一个示例使用 `amsmath` 包提供的 `equation*` 环境，因此我们需要将以下行添加到文档序言中：



```
\usepackage{amsmath}% For the equation* environment
```



For further information on using `amsmath` see [our help article](https://www.overleaf.com/learn/latex/Aligning_equations).
有关使用 `amsmath` 的更多信息，请参阅[我们的帮助文章](https://www.overleaf.com/learn/latex/Aligning_equations)。



```
\documentclass{article}
\usepackage{amsmath}% For the equation* environment
\begin{document}
\section{First example}

The well-known Pythagorean theorem \(x^2 + y^2 = z^2\) was proved to be invalid for other exponents, meaning the next equation has no integer solutions for \(n>2\):

\[ x^n + y^n = z^n \]

\section{Second example}

This is a simple math expression \(\sqrt{x^2+1}\) inside text. 
And this is also the same: 
\begin{math}
\sqrt{x^2+1}
\end{math}
but by using another command.

This is a simple math expression without numbering
\[\sqrt{x^2+1}\] 
separated from text.

This is also the same:
\begin{displaymath}
\sqrt{x^2+1}
\end{displaymath}

\ldots and this:
\begin{equation*}
\sqrt{x^2+1}
\end{equation*}
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=More+math+content+typeset+in+LaTeX&snip=\documentclass{article} \usepackage{amsmath}%+For+the+equation*+environment \begin{document} \section{First+example} The+well-known+Pythagorean+theorem+\(x^2+%2B+y^2+%3D+z^2\)+was+proved+to+be+invalid+for+other+exponents%2C+meaning+the+next+equation+has+no+integer+solutions+for+\(n>2\)%3A \[+x^n+%2B+y^n+%3D+z^n+\] \section{Second+example} This+is+a+simple+math+expression+\(\sqrt{x^2%2B1}\)+inside+text.+ And+this+is+also+the+same%3A+ \begin{math} \sqrt{x^2%2B1} \end{math} but+by+using+another+command. This+is+a+simple+math+expression+without+numbering \[\sqrt{x^2%2B1}\]+ separated+from+text. This+is+also+the+same%3A \begin{displaymath} \sqrt{x^2%2B1} \end{displaymath} \ldots+and+this%3A \begin{equation*} \sqrt{x^2%2B1} \end{equation*} \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing a range of math typeset in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/hT85gkewCDlxCHeNU5slE/9256c129b25bec7a93dcfe9e44b0654a/LL30Fig13r-plain.svg)



The possibilities with math in LaTeX are endless so be sure to visit our help pages for advice and examples on specific topics:
LaTeX 中的数学可能性是无穷无尽的，因此请务必访问我们的帮助页面以获取有关特定主题的建议和示例：

- [Mathematical expressions 数学表达式](https://www.overleaf.com/learn/latex/Mathematical_expressions)
- [Subscripts and superscripts
  下标和上标](https://www.overleaf.com/learn/latex/Subscripts_and_superscripts)
- [Brackets and Parentheses 方括号和括号](https://www.overleaf.com/learn/latex/Brackets_and_Parentheses)
- [Fractions and Binomials 分数和二项式](https://www.overleaf.com/learn/latex/Fractions_and_Binomials)
- [Aligning Equations 对齐方程](https://www.overleaf.com/learn/latex/Aligning_equations_with_amsmath)
- [Operators 运营商](https://www.overleaf.com/learn/latex/Operators)
- [Spacing in math mode 数学模式下的间距](https://www.overleaf.com/learn/latex/Spacing_in_math_mode)
- [Integrals, sums and limits
  积分、和极限](https://www.overleaf.com/learn/latex/Integrals%2C_sums_and_limits)
- [Display style in math mode
  数学模式下的显示样式](https://www.overleaf.com/learn/latex/Display_style_in_math_mode)
- [List of Greek letters and math symbols
  希腊字母和数学符号列表](https://www.overleaf.com/learn/latex/List_of_Greek_letters_and_math_symbols)
- [Mathematical fonts 数学字体](https://www.overleaf.com/learn/latex/Mathematical_fonts)

## Basic document structure 基本文档结构

Next, we explore abstracts and how to partition a LaTeX document into different chapters, sections and paragraphs.
接下来，我们探索摘要以及如何将 LaTeX 文档划分为不同的章节、节和段落。

### Abstracts 文摘

Scientific articles usually provide an *abstract* which is a brief overview/summary of their core topics, or arguments. The next example demonstrates typesetting an abstract using LaTeX’s `abstract` environment:
科学文章通常提供*摘要*，这是其核心主题或论点的简要概述/总结。下一个示例演示了使用 LaTeX 的`抽象`环境对抽象进行排版：



```
\documentclass{article}
\begin{document}
\begin{abstract}
This is a simple paragraph at the beginning of the 
document. A brief introduction about the main subject.
\end{abstract}
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=How+to+create+a+document+abstract&snip=\documentclass{article} \begin{document} \begin{abstract} This+is+a+simple+paragraph+at+the+beginning+of+the+ document.+A+brief+introduction+about+the+main+subject. \end{abstract} \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing an abstract typeset in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/4cPu8x8ZxuDVF6efcZ03yi/91aa6aa84719613b0e25c725b70aa0b8/LL30Fig14-plain.svg)



### Paragraphs and new lines 段落和换行符

With the abstract in place, we can begin writing our first paragraph. The next example demonstrates:
摘要就位后，我们可以开始编写我们的第一段。下一个示例演示：

- how a new paragraph is created by pressing the "enter" key twice, ending the current line and inserting a subsequent blank line;
  如何通过按两次 “Enter” 键创建新段落，结束当前行并插入后续的空行;
- how to start a new line without starting a new paragraph by inserting a manual line break using the `\\` command, which is a double backslash; alternatively, use the `\newline` command.
  如何通过使用 `\\` 命令（双反斜杠）插入手动换行符来开始新行而不开始新段落;或者，使用 `\newline` 命令。

The third paragraph in this example demonstrates use of the commands `\\` and `\newline`:
此示例中的第三段演示了命令 `\\` 和 `\newline` 的用法：



```
\documentclass{article}
\begin{document}

\begin{abstract}
This is a simple paragraph at the beginning of the 
document. A brief introduction about the main subject.
\end{abstract}

After our abstract we can begin the first paragraph, then press ``enter'' twice to start the second one.

This line will start a second paragraph.

I will start the third paragraph and then add \\ a manual line break which causes this text to start on a new line but remains part of the same paragraph. Alternatively, I can use the \verb|\newline|\newline command to start a new line, which is also part of the same paragraph.
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Example+to+create+a+new+paragraph&snip=\documentclass{article} \begin{document} \begin{abstract} This+is+a+simple+paragraph+at+the+beginning+of+the+ document.+A+brief+introduction+about+the+main+subject. \end{abstract} After+our+abstract+we+can+begin+the+first+paragraph%2C+then+press+``enter''+twice+to+start+the+second+one. This+line+will+start+a+second+paragraph. I+will+start+the+third+paragraph+and+then+add+\\+a+manual+line+break+which+causes+this+text+to+start+on+a+new+line+but+remains+part+of+the+same+paragraph.+Alternatively%2C+I+can+use+the+\verb|\newline|\newline+command+to+start+a+new+line%2C+which+is+also+part+of+the+same+paragraph. \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing the creation of paragraphs in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/5DdSH06hFli8k4lR0dxw4m/a55cddf9aa10b64302ae7b72ba0c6447/LL30Fig15r-plain.svg)



Note how LaTeX automatically indents paragraphs—except immediately after document headings such as section and subsection—[as we will see](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Chapters_and_sections).
请注意 LaTeX 如何自动缩进段落——除了紧跟在文档标题之后，例如 section 和 subsection——[正如我们将看到](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Chapters_and_sections)的。

New users are advised that multiple `\\` or `\newline`s should not used to “simulate” paragraphs with larger spacing between them because this can interfere with LaTeX’s typesetting algorithms. The recommended method is to continue using blank lines for creating new paragraphs, without any `\\`, and load the [`parskip` package](https://ctan.org/pkg/parskip?lang=en) by adding `\usepackage{parskip}` to the preamble.
建议新用户不要使用多个 `\\` 或 `\newline`s 来“模拟”它们之间间距较大的段落，因为这会干扰 LaTeX 的排版算法。推荐的方法是继续使用空行创建新段落，不带任何 `\\`，并通过将 `\usepackage{parskip}` 添加到序言来加载 [`parskip` 包](https://ctan.org/pkg/parskip?lang=en)。

Further information on paragraphs can be found in the following articles:
有关段落的更多信息，请参阅以下文章：

- [Paragraphs and new lines 段落和换行符](https://www.overleaf.com/learn/latex/Paragraphs_and_new_lines)
- [How to change paragraph spacing in LaTeX
  如何在 LaTeX 中更改段落间距](https://www.overleaf.com/learn/latex/Articles/How_to_change_paragraph_spacing_in_LaTeX)
- [LaTeX Error: There's no line here to end](https://www.overleaf.com/learn/latex/Errors/LaTeX_Error%3A_There's_no_line_here_to_end) provides additional advice and guidance on using `\\`.
  [LaTeX 错误：此处没有行 提供了](https://www.overleaf.com/learn/latex/Errors/LaTeX_Error%3A_There's_no_line_here_to_end)有关使用 `\\` 的其他建议和指导。

### Chapters and sections 章节

Longer documents, irrespective of authoring software, are usually partitioned into parts, chapters, sections, subsections and so forth. LaTeX also provides document-structuring commands but the available commands, and their implementations (what they do), can depend on the document class being used. By way of example, documents created using the `book` class can be split into parts, chapters, sections, subsections and so forth but the `letter` class does not provide (support) any commands to do that.
较长的文档，无论使用何种创作软件，通常都被划分为部分、章节、节、小节等。LaTeX 也提供了文档结构命令，但可用的命令及其实现（它们的作用）可能取决于所使用的文档类。例如，使用 `book` 类创建的文档可以拆分为部分、章节、部分、小节等，但 `letter` 类不提供（支持）任何命令来执行此操作。

This next example demonstrates commands used to structure a document based on the `book` class:
下一个示例演示了用于基于 `book` 类构建文档的命令：



```
\documentclass{book}
\begin{document}

\chapter{First Chapter}

\section{Introduction}

This is the first section.

Lorem  ipsum  dolor  sit  amet,  consectetuer  adipiscing  
elit. Etiam  lobortisfacilisis sem.  Nullam nec mi et 
neque pharetra sollicitudin.  Praesent imperdietmi nec ante. 
Donec ullamcorper, felis non sodales...

\section{Second Section}

Lorem ipsum dolor sit amet, consectetuer adipiscing elit.  
Etiam lobortis facilisissem.  Nullam nec mi et neque pharetra 
sollicitudin.  Praesent imperdiet mi necante...

\subsection{First Subsection}
Praesent imperdietmi nec ante. Donec ullamcorper, felis non sodales...

\section*{Unnumbered Section}
Lorem ipsum dolor sit amet, consectetuer adipiscing elit.  
Etiam lobortis facilisissem...
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Book+class+example+document&snip=\documentclass{book} \begin{document} \chapter{First+Chapter} \section{Introduction} This+is+the+first+section. Lorem++ipsum++dolor++sit++amet%2C++consectetuer++adipiscing++ elit.+Etiam++lobortisfacilisis+sem.++Nullam+nec+mi+et+ neque+pharetra+sollicitudin.++Praesent+imperdietmi+nec+ante.+ Donec+ullamcorper%2C+felis+non+sodales... \section{Second+Section} Lorem+ipsum+dolor+sit+amet%2C+consectetuer+adipiscing+elit.++ Etiam+lobortis+facilisissem.++Nullam+nec+mi+et+neque+pharetra+ sollicitudin.++Praesent+imperdiet+mi+necante... \subsection{First+Subsection} Praesent+imperdietmi+nec+ante.+Donec+ullamcorper%2C+felis+non+sodales... \section*{Unnumbered+Section} Lorem+ipsum+dolor+sit+amet%2C+consectetuer+adipiscing+elit.++ Etiam+lobortis+facilisissem... \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing sections in LaTeX book document](https://images.ctfassets.net/nrgyaltdicpt/1A1T7YsurQdM058OwmLqd8/7f6e962c31356bafa702bab9062f6061/LL30Fig16-plain.svg)



The names of sectioning commands are mostly self-explanatory; for example, `\chapter{First Chapter}` creates a new chapter titled `First Chapter`, `\section{Introduction}` produces a section titled `Introduction`, and so forth. Sections can be further divided into `\subsection{...}` and even `\subsubsection{...}`. The numbering of sections, subsections etc. is automatic but can be disabled by using the so-called *starred version* of the appropriate command which has an asterisk (*) at the end, such as `\section*{...}` and `\subsection*{...}`.
分段命令的名称大多是不言自明的;例如，`\chapter{First Chapter}` 创建一个名为 `First Chapter` 的新章节，`\section{Introduction}` 创建一个标题为 `Introduction`的章节，依此类推。部分可以进一步分为 `\subsection{...}` 甚至 `\subsubsection{...}`。章节、小节等的编号是自动的，但可以通过使用适当命令的所谓*星标版本*来禁用，该命令的末尾有一个星号 （*），例如 `\section*{...}` 和 `\subsection*{...}`。

*Collectively*, LaTeX document classes provide the following sectioning commands, with specific classes each supporting a relevant subset:
*总的来说*，LaTeX 文档类提供以下分段命令，每个特定类都支持一个相关的子集：

- `\part{part}` `\part{部分}`
- `\chapter{chapter}`
  `\chapter{章节}`
- `\section{section}`
- `\subsection{subsection}`
  `\subsection{小节}`
- `\subsubsection{subsubsection}`
- `\paragraph{paragraph}`
  `\paragraph{段落}`
- `\subparagraph{subparagraph}`

In particular, the `\part` and `\chapter` commands are only available in the `report` and `book` document classes.
特别是，`\part` 和 `\chapter` 命令仅在 `report` 和 `book` document 类中可用。

Visit the Overleaf article [article about sections and chapters](https://www.overleaf.com/learn/latex/Sections_and_chapters) for further information about document-structure commands.
有关 document-structure 命令的更多信息，请访问 Overleaf 文章[中有关章节和章节的文章](https://www.overleaf.com/learn/latex/Sections_and_chapters)。

## Creating tables 创建表

Overleaf provides three options to create tables:
Overleaf 提供了三个选项来创建 table：

1. Using the [**Insert Table** button](https://www.overleaf.com/learn/how-to/How_to_insert_tables_in_Overleaf%23inserttable#Using_Insert_Table_to_create_a_table_in_your_project) in the **Visual Editor** (or **Code Editor**) toolbar.
   使用 **Visual Editor**（或 **Code Editor**）工具栏中的 [**Insert Table** 按钮](https://www.overleaf.com/learn/how-to/How_to_insert_tables_in_Overleaf%23inserttable#Using_Insert_Table_to_create_a_table_in_your_project)。
2. [Copying and pasting a table](https://www.overleaf.com/learn/how-to/How_to_paste_formatted_content_into_Overleaf%23pastingtables) from another document while using **Visual Editor**.
   使用**可视化编辑器**时从另一个文档[复制和粘贴表格](https://www.overleaf.com/learn/how-to/How_to_paste_formatted_content_into_Overleaf%23pastingtables)。
3. Writing the LaTeX code for the table in Code Editor.
   在 Code Editor 中为表编写 LaTeX 代码。

If you’re new to LaTeX, using the toolbar in **Visual Editor** (option 1) is a great way to get started—you can switch between **Visual Editor** and **Code Editor** to see the code behind the table.
如果您是 LaTeX 的新手，使用 **Visual Editor** 中的工具栏（选项 1）是一个很好的入门方式 — 您可以在 **Visual Editor** 和 **Code Editor** 之间切换以查看表格后面的代码。

Here, we focus on option 3—the most flexible method for creating tables—and provide examples that demonstrate how to create tables in LaTeX, including the addition of lines (rules) and captions. As you gain experience, take a look at our detailed guidance on [how to create tables using LaTeX](https://www.overleaf.com/learn/latex/Tables).
在这里，我们重点介绍选项 3（创建表格的最灵活的方法），并提供演示如何在 LaTeX 中创建表格的示例，包括添加线条（规则）和标题。随着您获得经验，请查看我们关于[如何使用 LaTeX 创建表](https://www.overleaf.com/learn/latex/Tables)的详细指南。

### Creating a basic table in LaTeX 在 LaTeX 中创建基本表

We start with an example showing how to typeset a basic table:
我们从一个例子开始，展示如何对一个基本表格进行排版：



```
\begin{center}
\begin{tabular}{c c c}
 cell1 & cell2 & cell3 \\ 
 cell4 & cell5 & cell6 \\  
 cell7 & cell8 & cell9    
\end{tabular}
\end{center}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=An+example+of+a+basic+table&snip=\documentclass{article} \begin{document} \begin{center} \begin{tabular}{c+c+c} +cell1+%26+cell2+%26+cell3+\\+ +cell4+%26+cell5+%26+cell6+\\++ +cell7+%26+cell8+%26+cell9++++ \end{tabular} \end{center} \end{document} <%2Fsource>)



This example produces the following output:
此示例生成以下输出：

![Graphic displaying a table typeset in LaTeX](https://images.ctfassets.net/nrgyaltdicpt/5K46QavbKv9vF4RI1GbUf2/f22d4f8a06d00251166f86d2c891321e/LL30Fig17-plain.svg)



The `tabular` environment is the default LaTeX method to create tables. You must specify a parameter to this environment, in this case `{c c c}` which advises LaTeX that there will be three columns and the text inside each one must be centred. You can also use `r` to right-align the text and `l` to left-align it. The alignment symbol `&` is used to demarcate individual table cells within a table row. To end a table row use the *new line* command `\\`. Our table is contained within a `center` environment to make it centred within the text width of the page.
`表格`环境是创建表的默认 LaTeX 方法。您必须为此环境指定一个参数，在本例中为 `{c c c}`，它建议 LaTeX 将有三列，并且每列中的文本必须居中。您还可以使用 `r` 将文本右对齐，使用 `l` 将其左对齐。对齐符号`&`用于在表格行内划分单个表格单元格。要结束表行，请使用*新行*命令 `\\`。我们的表格包含在`一个中心`环境中，使其在页面的文本宽度内居中。

### Adding borders 添加边框

The `tabular` environment supports horizontal and vertical lines (rules) as part of the table:
`表格`环境支持将水平线和垂直线（规则）作为表的一部分：

- to add horizontal rules, above and below rows, use the `\hline` command
  要在行的上方和下方添加水平线，请使用 `\hline` 命令
- to add vertical rules, between columns, use the vertical line parameter `|`
  要在列之间添加垂直规则，请使用 垂直线 `参数 |`

In this example the argument is `{|c|c|c|}` which declares three (centred) columns each separated by a vertical line (rule); in addition, we use `\hline` to place a horizontal rule above the first row and below the final row:
在这个例子中，参数是 `{|c|c|c|}`，它声明了三个（居中）列，每个列由一条垂直线（规则）分隔;此外，我们使用 `\hline` 在第一行的上方和最后一行的下方放置一条水平标尺：



```
\begin{center}
\begin{tabular}{|c|c|c|} 
 \hline
 cell1 & cell2 & cell3 \\ 
 cell4 & cell5 & cell6 \\ 
 cell7 & cell8 & cell9 \\ 
 \hline
\end{tabular}
\end{center}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Table+example+with+rules&snip=\documentclass{article} \begin{document} \begin{center} \begin{tabular}{|c|c|c|}+ +\hline +cell1+%26+cell2+%26+cell3+\\+ +cell4+%26+cell5+%26+cell6+\\+ +cell7+%26+cell8+%26+cell9+\\+ +\hline \end{tabular} \end{center} \end{document})



This example produces the following output:
此示例生成以下输出：

![Graphic displaying a table typeset in LaTeX containing horizontal and vertical rules](https://images.ctfassets.net/nrgyaltdicpt/5uWYGUhK1XJJJaWz5R1EmX/3ee88bf6b2eaf8d0644b57fa8064800b/LL30Fig18-plain.svg)



Here is a further example:
下面是另一个示例：



```
\begin{center}
 \begin{tabular}{||c c c c||} 
 \hline
 Col1 & Col2 & Col2 & Col3 \\ [0.5ex] 
 \hline\hline
 1 & 6 & 87837 & 787 \\ 
 \hline
 2 & 7 & 78 & 5415 \\
 \hline
 3 & 545 & 778 & 7507 \\
 \hline
 4 & 545 & 18744 & 7560 \\
 \hline
 5 & 88 & 788 & 6344 \\ [1ex] 
 \hline
\end{tabular}
\end{center}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Another+table+example+containing+rules&snip=\documentclass{article} \begin{document} \begin{center} +\begin{tabular}{||c+c+c+c||}+ +\hline +Col1+%26+Col2+%26+Col2+%26+Col3+\\+[0.5ex]+ +\hline\hline +1+%26+6+%26+87837+%26+787+\\+ +\hline +2+%26+7+%26+78+%26+5415+\\ +\hline +3+%26+545+%26+778+%26+7507+\\ +\hline +4+%26+545+%26+18744+%26+7560+\\ +\hline +5+%26+88+%26+788+%26+6344+\\+[1ex]+ +\hline \end{tabular} \end{center} \end{document})



This example produces the following output:
此示例生成以下输出：

![Graphic displaying a table typeset in LaTeX containing horizontal and vertical rules](https://images.ctfassets.net/nrgyaltdicpt/1Cy9FcRnDVDRUPQdCgaKq6/c21e5f7d9a53514756c6e1f2996e51e0/LL30Fig19-plain.svg)



### Captions, labels and references 标题、标签和引用

You can caption and reference tables in much the same way as images. The only difference is that instead of the **`figure`** environment, you use the **`table`** environment.
您可以采用与图像大致相同的方式为表格添加标题和引用表格。唯一的区别是，您使用的是 **`table`** 环境，而不是 **`figure`** 环境。



```
Table \ref{table:data} shows how to add a table caption and reference a table.
\begin{table}[h!]
\centering
\begin{tabular}{||c c c c||} 
 \hline
 Col1 & Col2 & Col2 & Col3 \\ [0.5ex] 
 \hline\hline
 1 & 6 & 87837 & 787 \\ 
 2 & 7 & 78 & 5415 \\
 3 & 545 & 778 & 7507 \\
 4 & 545 & 18744 & 7560 \\
 5 & 88 & 788 & 6344 \\ [1ex] 
 \hline
\end{tabular}
\caption{Table to test captions and labels.}
\label{table:data}
\end{table}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Table+captions+and+references&snip=\documentclass{article} \begin{document} Table+\ref{table%3Adata}+shows+how+to+add+a+table+caption+and+reference+a+table. \begin{table}[h!] \centering \begin{tabular}{||c+c+c+c||}+ +\hline +Col1+%26+Col2+%26+Col2+%26+Col3+\\+[0.5ex]+ +\hline\hline +1+%26+6+%26+87837+%26+787+\\+ +2+%26+7+%26+78+%26+5415+\\ +3+%26+545+%26+778+%26+7507+\\ +4+%26+545+%26+18744+%26+7560+\\ +5+%26+88+%26+788+%26+6344+\\+[1ex]+ +\hline \end{tabular} \caption{Table+to+test+captions+and+labels.} \label{table%3Adata} \end{table} \end{document})



This example produces the following output:
此示例生成以下输出：

![A LaTeX table with a caption](https://images.ctfassets.net/nrgyaltdicpt/1f5w74UIaTCkpApaPdVeWf/580a87c2413ddc9d6bdef3bf462689fc/LL30Fig20-plain.svg)



## Adding a Table of Contents 添加目录

Creating a table of contents is straightforward because the command `\tableofcontents` does almost all the work for you:
创建目录很简单，因为命令 `\tableofcontents` 几乎为您完成了所有工作：



```
\documentclass{article}
\title{Sections and Chapters}
\author{Gubert Farnsworth}
\date{August 2022}
\begin{document}
  
\maketitle
  
\tableofcontents

\section{Introduction}
   
This is the first section.
      
Lorem  ipsum  dolor  sit  amet,  consectetuer  adipiscing  
elit.   Etiam  lobortisfacilisis sem.  Nullam nec mi et 
neque pharetra sollicitudin.  Praesent imperdietmi nec ante. 
Donec ullamcorper, felis non sodales...
       
\section*{Unnumbered Section}
\addcontentsline{toc}{section}{Unnumbered Section}

Lorem ipsum dolor sit amet, consectetuer adipiscing elit.  
Etiam lobortis facilisissem.  Nullam nec mi et neque pharetra 
sollicitudin.  Praesent imperdiet mi necante...

\section{Second Section}
       
Lorem ipsum dolor sit amet, consectetuer adipiscing elit.  
Etiam lobortis facilisissem.  Nullam nec mi et neque pharetra 
sollicitudin.  Praesent imperdiet mi necante...
\end{document}
```

[ Open this example in Overleaf.
在 Overleaf 中打开此示例。](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Generating+a+table+of+contents&snip=\documentclass{article} \title{Sections+and+Chapters} \author{Gubert+Farnsworth} \date{August+2022} \begin{document} ++ \maketitle ++ \tableofcontents \section{Introduction} +++ This+is+the+first+section. ++++++ Lorem++ipsum++dolor++sit++amet%2C++consectetuer++adipiscing++ elit.+++Etiam++lobortisfacilisis+sem.++Nullam+nec+mi+et+ neque+pharetra+sollicitudin.++Praesent+imperdietmi+nec+ante.+ Donec+ullamcorper%2C+felis+non+sodales... +++++++ \section*{Unnumbered+Section} \addcontentsline{toc}{section}{Unnumbered+Section} Lorem+ipsum+dolor+sit+amet%2C+consectetuer+adipiscing+elit.++ Etiam+lobortis+facilisissem.++Nullam+nec+mi+et+neque+pharetra+ sollicitudin.++Praesent+imperdiet+mi+necante... \section{Second+Section} +++++++ Lorem+ipsum+dolor+sit+amet%2C+consectetuer+adipiscing+elit.++ Etiam+lobortis+facilisissem.++Nullam+nec+mi+et+neque+pharetra+ sollicitudin.++Praesent+imperdiet+mi+necante... \end{document})



This example produces the following output:
此示例生成以下输出：

![Graphic showing a table of contents produced by LaTeX](https://images.ctfassets.net/nrgyaltdicpt/MxY592Q6EGsDKMA2mZw0t/fffa41a0a0d30770526f73aff72a7be1/LL30Fig21r-plain.svg)



Sections, subsections and chapters are automatically included in the table of contents. To manually add entries, such as an unnumbered section, use the command `\addcontentsline` as shown in the example.
章节、小节和章节会自动包含在目录中。要手动添加条目（如未编号的部分），请使用命令 `\addcontentsline`，如示例中所示。

## Downloading your finished document 下载完成的文档

The following brief video clip shows how to download your project’s source code or the typeset PDF file:
以下简短的视频剪辑显示了如何下载项目的源代码或排版 PDF 文件：



<video controls="" width="100%" height="100%" src="https://videos.ctfassets.net/nrgyaltdicpt/2n6iw0AUELNtABCuva0oV5/cf27bff3a6099da94362d64645e69dfe/LL30download.mp4" type="video/mp4" data-immersive-translate-walked="aafa2316-ff14-4d3d-9e7a-98c009c61058" style="box-sizing: border-box; display: inline-block; vertical-align: baseline;"></video>



More information can be found in the Overleaf help article [Exporting your work from Overleaf](https://www.overleaf.com/learn/how-to/Exporting_your_work_from_Overleaf).
更多信息可以在 Overleaf 帮助文章 [从 Overleaf 导出你的作品](https://www.overleaf.com/learn/how-to/Exporting_your_work_from_Overleaf) 中找到。

## Finding and using LaTeX packages 查找和使用 LaTeX 包

LaTeX not only delivers significant typesetting capabilities but also provides a *framework for extensibility* through the use of add-on *packages*. Rather than attempting to provide commands and features that “try to do everything”, LaTeX is designed to be *extensible*, allowing users to load external bodies of code (packages) that provide more specialist typesetting capabilities or extend LaTeX’s built-in features—such as typesetting tables. As observed in the section [Adding images](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_images), the `graphicx` package extends LaTeX by providing commands to import graphics files and was loaded (in the preamble) by writing



```
\usepackage{graphicx}
```



### Loading packages 加载软件包

As noted above, packages are loaded in the document preamble via the `\usepackage` command but because (many) LaTeX packages provide a set of *options*, which can be used to configure their behaviour, the `\usepackage` command often looks like this:
如上所述，包是通过 `\usepackage` 命令加载到文档序言中的，但是因为（许多）LaTeX 包提供了一组选项，这些*选项*可用于配置它们的行为，`因此 \usepackage` 命令通常如下所示：



```
\usepackage[options]{somepackage}
```



The square brackets “`[...]`” inform LaTeX which set of options should be applied when it loads `somepackage`. Within the set of options requested by the user, individual options, or settings, are typically separated by a comma; for example, the [`geometry` package](https://ctan.org/pkg/geometry) provides many options to configure page layout in LaTeX, so a typical use of `geometry` might look like this:
方括号 “`[...]`” 告诉 LaTeX 在加载 `somepackage` 时应该应用哪组选项。在用户请求的选项集中，各个选项或设置通常用逗号分隔;例如， [`geometry` 包](https://ctan.org/pkg/geometry)提供了许多选项来在 LaTeX 中配置页面布局，因此 `geometry` 的典型用法可能如下所示：



```
\usepackage[total={6.5in,8.75in},
top=1.2in, left=0.9in, includefoot]{geometry}
```



The `geometry` package is one example of a package written and contributed by members of the global LaTeX community and made available, for free, to anyone who wants to use it.
`geometry` 包是由全球 LaTeX 社区成员编写和贡献的包的一个例子，任何人都可以免费使用它。

If a LaTeX package does not provide any options, or the user wants to use the default values of a package’s options, it would be loaded like this:
如果 LaTeX 包不提供任何选项，或者用户想要使用包选项的默认值，它将像这样加载：



```
\usepackage{somepackage}
```



When you write `\usepackage[...]{somepackage}` LaTeX looks for a corresponding file called `*somepackage*.sty`, which it needs to load and process—to make the package commands available and execute any other code provided by that package. If LaTeX cannot find `*somepackage*.sty` it will terminate with an error, as demonstrated in the following Overleaf example:
当你编写 `\usepackage[...] 时{somepackage}`LaTeX 会查找一个名为 `*somepackage.sty*` 的相应文件，它需要加载和处理该文件，以使包命令可用并执行该包提供的任何其他代码。如果 LaTeX 找不到 `*somepackage.sty*`，它将以错误终止，如下面的 Overleaf 示例所示：



```
\documentclass[12pt, letterpaper]{article}
\usepackage{somepackage}% a NON-EXISTENT package
\begin{document}
This will fail!
\end{document}
```

[ Open this ***error-generating example*** on Overleaf
在 Overleaf 上打开此***生成错误的示例***](https://www.overleaf.com/docs?engine=pdflatex&snip_name=Error+due+to+missing+package&snip=\documentclass[12pt%2C+letterpaper]{article} \usepackage{somepackage}%+a+NON-EXISTENT+package \begin{document} This+will+fail! \end{document})



This example produces the following output:
此示例生成以下输出：

![Image showing error causes by a missing package](https://sharelatex-wiki-cdn-671420.c.cdn77.org/learn-scripts/images/6/60/LL30packagefail.png)

### Finding information about packages: CTAN 查找有关包的信息：CTAN

Packages are distributed through the [Comprehensive TeX Archive Network](https://www.ctan.org/), usually referred to as CTAN, which, at the time of writing, hosts 6287 packages from 2881 contributors. CTAN [describes itself](https://www.ctan.org/ctan) as
包通过 [Comprehensive TeX Archive Network](https://www.ctan.org/)（通常称为 CTAN）分发，在撰写本文时，该网络托管了来自 2881 个贡献者的 6287 个包。CTAN [将自己描述](https://www.ctan.org/ctan)为

>  
>
> ... a set of Internet sites around the world that offer TEX-related material for download.
> ...世界各地的一组 Internet 站点，提供 TEX 相关材料以供下载。

You can browse CTAN to look for useful packages; for example:
您可以浏览 CTAN 以查找有用的软件包;例如：

- [by topic 按主题](https://www.ctan.org/topics/cloud)
- [alphabetically](https://www.ctan.org/pkg) (useful if you know the package name)
  [按字母顺序排列](https://www.ctan.org/pkg)（如果您知道包名称，则很有用）

You can also use the [search facility](https://www.ctan.org/pkg) (at the top of the page).
您也可以使用[搜索工具](https://www.ctan.org/pkg)（位于页面顶部）。

### Packages available on Overleaf: Introducing TeX Live Overleaf 上可用的包：TeX Live 简介

Once per year a (large) *subset* of packages hosted on CTAN, plus LaTeX-related fonts and other software, is collated and distributed as a system called [TeX Live](https://tug.org/texlive/), which can be used to install your own (local) LaTeX setup. In fact, [Overleaf’s servers also use TeX Live](https://www.overleaf.com/learn/latex/Overleaf_and_TeX_Live) and are updated when a new version of TeX Live is released. Overleaf’s TeX Live updates are not immediate but take place a few months post-release, giving us time to perform compatibility tests of the new TeX Live version with the [thousands of templates contained in our gallery](https://www.overleaf.com/gallery). For example, here is our [TeX Live 2022 upgrade announcement](https://www.overleaf.com/blog/tex-live-2022-now-available).
每年一次，一个*托管在* CTAN 上的（大部分）包子集，以及与 LaTeX 相关的字体和其他软件，作为一个名为 [TeX Live](https://tug.org/texlive/) 的系统进行整理和分发，该系统可用于安装您自己的（本地）LaTeX 设置。事实上，[Overleaf 的服务器也使用 TeX Live](https://www.overleaf.com/learn/latex/Overleaf_and_TeX_Live)，并在 TeX Live 的新版本发布时进行更新。Overleaf 的 TeX Live 更新不是立即进行的，而是在发布后几个月进行，这让我们有时间对新的 TeX Live 版本与我们[图库中包含的数千个模板](https://www.overleaf.com/gallery)进行兼容性测试。例如，这是我们的 [TeX Live 2022 升级公告](https://www.overleaf.com/blog/tex-live-2022-now-available)。

Although TeX Live contains a (large) *subset* of CTAN packages it is possible to find an interesting package, such as [`igo` for typesetting Go diagrams](https://ctan.org/pkg/igo?lang=en), which is hosted on CTAN but not included in (distributed by) TeX Live and thus unavailable on Overleaf. Some packages hosted on CTAN are not part of TeX Live due to a variety of reasons: perhaps a package is obsolete, has licensing problems, is extremely new (recently uploaded) or has platform dependencies, such as working on Windows but not Linux.
尽管 TeX Live 包含（很大）个 CTAN 包的*子集*，但还是可以找到一个有趣的包，例如[用于排版围棋图的 `igo`](https://ctan.org/pkg/igo?lang=en)，它托管在 CTAN 上，但不包含在 TeX Live 中（由其分发），因此在 Overleaf 上不可用。由于各种原因，一些托管在 CTAN 上的包不是 TeX Live 的一部分：也许一个包已过时、存在许可问题、非常新（最近上传）或具有平台依赖性，例如在 Windows 上运行而不是在 Linux 上运行。

New packages, and updates to existing ones, are uploaded to CTAN all year round but updates to TeX Live are distributed annually; consequently, packages contained in the current version of TeX Live will not be as up-to-date as those hosted on CTAN. Because Overleaf’s servers use TeX Live it is possible that packages installed on our servers—i.e., ones available to our users—might not be the very latest versions available on CTAN but, generally, this is unlikely to be problematic.
新包和现有包的更新全年上传到 CTAN，但 TeX Live 的更新每年分发一次;因此，当前版本的 TeX Live 中包含的包将不如 CTAN 上托管的包是最新的。因为 Overleaf 的服务器使用 TeX Live，所以安装在我们服务器上的包（即我们用户可用的包）可能不是 CTAN 上可用的最新版本，但一般来说，这不太可能有问题。