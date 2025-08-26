* Headings
  * `<h1>-<h6>`
  
* Paragraphs
  * `<p>`
  
* Lists
  * `<ul>`
  * `<ol>`
    * `<li>`
  
* Links
  * `<a href="">`
  
* Embedding images
  * `<img src="" alt=""/>`

* 基本语法

  * 元素 (Element)

    * 开始标签（Opening tag）：`<element name>`

    * 结束标签（Closing tag）：`</element name>`

      > 有一些元素为**空元素**即只有开始标签，但无结束标签，eg.`<img />`
      > 不需要通过内容来产生效果

    * 内容（Content）

    * 属性（Attribute）

      * `<element_name attribute_name="attribute_value">`

        > 属性包含的是不想在真正的内容中出现的和元素有关的额外信息。本例中，`class` 是属性*名*，`editor-note` 是属性*值*。`class` 属性是可以用于定位元素（以及任何其他有相同 `class` 值的元素）的标识名称，以便进一步为元素指定样式或进行其他操作时使用。
        
        > **一些属性没有值**，如 [`required`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Reference/Attributes/required)。
        
        > 不包含 [ASCII](https://developer.mozilla.org/zh-CN/docs/Glossary/ASCII) 空格（以及 `"` `'` ``` `=` `<` `>`）的简单属性值可以不使用引号，但是建议将所有属性值用引号括起来，这样的代码一致性更佳，更易于阅读。

  * 嵌套元素 (Embedded Element)

    * 一个元素置于其他元素之中——称作**嵌套**
    * 必须保证元素的嵌套次序正确

    

* 实例

  * `<!doctype html>`——[文档类型](https://developer.mozilla.org/zh-CN/docs/Glossary/Doctype)。这是必不可少的开头。混沌初分，HTML 尚在襁褓（大约是 1991/92 年）之时，这个元素用来关联 HTML 编写规范，以供自动查错等功能所用。而在当今，它作用有限，可以说仅用于保证文档正常读取。现在知道这些就足够了。
  * `<html></html>`——该元素包含整个页面的所有内容，有时候也称作根元素。它还包含 `lang` 属性，设置页面的主要语种。
  * `<head></head>`——该元素作为想在 HTML 页面中包含但不想向用户显示的内容的容器。包括想在搜索结果中显示的[关键字](https://developer.mozilla.org/zh-CN/docs/Glossary/Keyword)和页面描述、用于设置页面样式的 CSS、字符集声明等等。
  * `<meta charset="utf-8">`——该元素指明你的文档使用 UTF-8 字符编码，UTF-8 包括世界绝大多数书写语言的字符。它基本上可以处理任何文本内容。以它为编码还可以避免以后出现某些问题，没有理由再选用其他编码。
  * `<meta name="viewport" content="width=device-width">`——[视口元素](https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSSOM_view/Viewport_concepts#移动设备的视口)可以确保页面以视口宽度进行渲染，避免移动端浏览器以比视口更宽的宽度渲染内容，导致内容缩小。
  * `<title></title>`——该元素设置页面的标题，显示在浏览器标签页上，也作为收藏网页的描述文字。
  * `<body></body>`——该元素包含期望让用户在访问页面时看到的*全部*内容，包括文本、图像、视频、游戏、可播放的音轨或其他内容。


```html
<!doctype html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />
    <title>My test page</title>
  </head>
  <body>
    <img src="" alt="My test image" />
  </body>
</html>
```

* html注释
  * `<!--	-->`
