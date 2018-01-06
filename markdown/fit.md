![mahua](mahua-logo.jpg)
##MaHua是什么?
    一个在线编辑markdown文档的编辑器

    向Mac下优秀的markdown编辑器mou致敬

##MaHua有哪些功能？

* 方便的`导入导出`功能# Editor.md

             ![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)

             ![](https://img.shields.io/github/stars/pandao/editor.md.svg) ![](https://img.shields.io/github/forks/pandao/editor.md.svg) ![](https://img.shields.io/github/tag/pandao/editor.md.svg) ![](https://img.shields.io/github/release/pandao/editor.md.svg) ![](https://img.shields.io/github/issues/pandao/editor.md.svg) ![](https://img.shields.io/bower/v/editor.md.svg)

             **目录 (Table of Contents)**

             [TOCM]

             [TOC]

             # Heading 1
             ## Heading 2
             ### Heading 3
             #### Heading 4
             ##### Heading 5
             ###### Heading 6
             # Heading 1 link [Heading link](https://github.com/pandao/editor.md "Heading link")
             ## Heading 2 link [Heading link](https://github.com/pandao/editor.md "Heading link")
             ### Heading 3 link [Heading link](https://github.com/pandao/editor.md "Heading link")
             #### Heading 4 link [Heading link](https://github.com/pandao/editor.md "Heading link") Heading link [Heading link](https://github.com/pandao/editor.md "Heading link")
             ##### Heading 5 link [Heading link](https://github.com/pandao/editor.md "Heading link")
             ###### Heading 6 link [Heading link](https://github.com/pandao/editor.md "Heading link")

             #### 标题（用底线的形式）Heading (underline)

             This is an H1
             =============

             This is an H2
             -------------

             ### 字符效果和横线等

             ----

             ~~删除线~~ <s>删除线（开启识别HTML标签时）</s>
             *斜体字*      _斜体字_
             **粗体**  __粗体__
             ***粗斜体*** ___粗斜体___

             上标：X<sub>2</sub>，下标：O<sup>2</sup>

             **缩写(同HTML的abbr标签)**

             > 即更长的单词或短语的缩写形式，前提是开启识别HTML标签时，已默认开启

             The <abbr title="Hyper Text Markup Language">HTML</abbr> specification is maintained by the <abbr title="World Wide Web Consortium">W3C</abbr>.

             ### 引用 Blockquotes

             > 引用文本 Blockquotes

             引用的行内混合 Blockquotes

             > 引用：如果想要插入空白换行`即<br />标签`，在插入处先键入两个以上的空格然后回车即可，[普通链接](http://localhost/)。

             ### 锚点与链接 Links

             [普通链接](http://localhost/)

             [普通链接带标题](http://localhost/ "普通链接带标题")

             直接链接：<https://github.com>

             [锚点链接][anchor-id]

             [anchor-id]: http://www.this-anchor-link.com/

             [mailto:test.test@gmail.com](mailto:test.test@gmail.com)

             GFM a-tail link @pandao  邮箱地址自动链接 test.test@gmail.com  www@vip.qq.com

             > @pandao

             ### 多语言代码高亮 Codes

             #### 行内代码 Inline code

             执行命令：`npm install marked`

             #### 缩进风格

             即缩进四个空格，也做为实现类似 `<pre>` 预格式化文本 ( Preformatted Text ) 的功能。

                 <?php
                     echo "Hello world!";
                 ?>

             预格式化文本：

                 | First Header  | Second Header |
                 | ------------- | ------------- |
                 | Content Cell  | Content Cell  |
                 | Content Cell  | Content Cell  |

             #### JS代码　

             ```javascript
             function test() {
             	console.log("Hello world!");
             }

             (function(){
                 var box = function() {
                     return box.fn.init();
                 };

                 box.prototype = box.fn = {
                     init : function(){
                         console.log('box.init()');

             			return this;
                     },

             		add : function(str) {
             			alert("add", str);

             			return this;
             		},

             		remove : function(str) {
             			alert("remove", str);

             			return this;
             		}
                 };

                 box.fn.init.prototype = box.fn;

                 window.box =box;
             })();

             var testBox = box();
             testBox.add("jQuery").remove("jQuery");
             ```

             #### HTML 代码 HTML codes

             ```html
             <!DOCTYPE html>
             <html>
                 <head>
                     <mate charest="utf-8" />
                     <meta name="keywords" content="Editor.md, Markdown, Editor" />
                     <title>Hello world!</title>
                     <style type="text/css">
                         body{font-size:14px;color:#444;font-family: "Microsoft Yahei", Tahoma, "Hiragino Sans GB", Arial;background:#fff;}
                         ul{list-style: none;}
                         img{border:none;vertical-align: middle;}
                     </style>
                 </head>
                 <body>
                     <h1 class="text-xxl">Hello world!</h1>
                     <p class="text-green">Plain text</p>
                 </body>
             </html>
             ```

             ### 图片 Images

             Image:

             ![](https://pandao.github.io/editor.md/examples/images/4.jpg)

             > Follow your heart.

             ![](https://pandao.github.io/editor.md/examples/images/8.jpg)

             > 图为：厦门白城沙滩

             图片加链接 (Image + Link)：

             [![](https://pandao.github.io/editor.md/examples/images/7.jpg)](https://pandao.github.io/editor.md/images/7.jpg "李健首张专辑《似水流年》封面")

             > 图为：李健首张专辑《似水流年》封面

             ----

             ### 列表 Lists

             #### 无序列表（减号）Unordered Lists (-)

             - 列表一
             - 列表二
             - 列表三

             #### 无序列表（星号）Unordered Lists (*)

             * 列表一
             * 列表二
             * 列表三

             #### 无序列表（加号和嵌套）Unordered Lists (+)

             + 列表一
             + 列表二
                 + 列表二-1
                 + 列表二-2
                 + 列表二-3
             + 列表三
                 * 列表一
                 * 列表二
                 * 列表三

             #### 有序列表 Ordered Lists (-)

             1. 第一行
             2. 第二行
             3. 第三行

             #### GFM task list

             - [x] GFM task list 1
             - [x] GFM task list 2
             - [ ] GFM task list 3
                 - [ ] GFM task list 3-1
                 - [ ] GFM task list 3-2
                 - [ ] GFM task list 3-3
             - [ ] GFM task list 4
                 - [ ] GFM task list 4-1
                 - [ ] GFM task list 4-2

             ----

             ### 绘制表格 Tables

             | 项目        | 价格   |  数量  |
             | --------   | -----:  | :----:  |
             | 计算机      | $1600   |   5     |
             | 手机        |   $12   |   12   |
             | 管线        |    $1    |  234  |

             First Header  | Second Header
             ------------- | -------------
             Content Cell  | Content Cell
             Content Cell  | Content Cell

             | First Header  | Second Header |
             | ------------- | ------------- |
             | Content Cell  | Content Cell  |
             | Content Cell  | Content Cell  |

             | Function name | Description                    |
             | ------------- | ------------------------------ |
             | `help()`      | Display the help window.       |
             | `destroy()`   | **Destroy your computer!**     |

             | Left-Aligned  | Center Aligned  | Right Aligned |
             | :------------ |:---------------:| -----:|
             | col 3 is      | some wordy text | $1600 |
             | col 2 is      | centered        |   $12 |
             | zebra stripes | are neat        |    $1 |

             | Item      | Value |
             | --------- | -----:|
             | Computer  | $1600 |
             | Phone     |   $12 |
             | Pipe      |    $1 |

             ----

             #### 特殊符号 HTML Entities Codes

             &copy; &  &uml; &trade; &iexcl; &pound;
             &amp; &lt; &gt; &yen; &euro; &reg; &plusmn; &para; &sect; &brvbar; &macr; &laquo; &middot;

             X&sup2; Y&sup3; &frac34; &frac14;  &times;  &divide;   &raquo;

             18&ordm;C  &quot;  &apos;

             [========]

             ### Emoji表情 :smiley:

             > Blockquotes :star:

             #### GFM task lists & Emoji & fontAwesome icon emoji & editormd logo emoji :editormd-logo-5x:

             - [x] :smiley: @mentions, :smiley: #refs, [links](), **formatting**, and <del>tags</del> supported :editormd-logo:;
             - [x] list syntax required (any unordered or ordered list supported) :editormd-logo-3x:;
             - [x] [ ] :smiley: this is a complete item :smiley:;
             - [ ] []this is an incomplete item [test link](#) :fa-star: @pandao;
             - [ ] [ ]this is an incomplete item :fa-star: :fa-gear:;
                 - [ ] :smiley: this is an incomplete item [test link](#) :fa-star: :fa-gear:;
                 - [ ] :smiley: this is  :fa-star: :fa-gear: an incomplete item [test link](#);

             #### 反斜杠 Escape

             \*literal asterisks\*

             [========]

             ### 科学公式 TeX(KaTeX)

             $$E=mc^2$$

             行内的公式$$E=mc^2$$行内的公式，行内的$$E=mc^2$$公式。

             $$x > y$$

             $$\(\sqrt{3x-1}+(1+x)^2\)$$

             $$\sin(\alpha)^{\theta}=\sum_{i=0}^{n}(x^i + \cos(f))$$

             多行公式：

             ```math
             \displaystyle
             \left( \sum\_{k=1}^n a\_k b\_k \right)^2
             \leq
             \left( \sum\_{k=1}^n a\_k^2 \right)
             \left( \sum\_{k=1}^n b\_k^2 \right)
             ```

             ```katex
             \displaystyle
                 \frac{1}{
                     \Bigl(\sqrt{\phi \sqrt{5}}-\phi\Bigr) e^{
                     \frac25 \pi}} = 1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {
                     1+\frac{e^{-6\pi}}
                     {1+\frac{e^{-8\pi}}
                      {1+\cdots} }
                     }
                 }
             ```

             ```latex
             f(x) = \int_{-\infty}^\infty
                 \hat f(\xi)\,e^{2 \pi i \xi x}
                 \,d\xi
             ```

             ### 分页符 Page break

             > Print Test: Ctrl + P

             [========]

             ### 绘制流程图 Flowchart

             ```flow
             st=>start: 用户登陆
             op=>operation: 登陆操作
             cond=>condition: 登陆成功 Yes or No?
             e=>end: 进入后台

             st->op->cond
             cond(yes)->e
             cond(no)->op
             ```

             [========]

             ### 绘制序列图 Sequence Diagram

             ```seq
             Andrew->China: Says Hello
             Note right of China: China thinks\nabout it
             China-->Andrew: How are you?
             Andrew->>China: I am good thanks!
             ```

             ### End
*  直接把一个markdown的文本文件拖放到当前这个页面就可以了
*  导出为一个html格式的文件，样式一点也不会丢失
* 编辑和预览`同步滚动`，所见即所得（右上角设置）
* `VIM快捷键`支持，方便vim党们快速的操作 （右上角设置）
* 强大的`自定义CSS`功能，方便定制自己的展示
* 有数量也有质量的`主题`,编辑器和预览区域
* 完美兼容`Github`的markdown语法
* 预览区域`代码高亮`
* 所有选项自动记忆

##有问题反馈
在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流

* 邮件(dev.hubo#gmail.com, 把#换成@)
* QQ: 287759234
* weibo: [@草依山](http://weibo.com/ihubo)
* twitter: [@ihubo](http://twitter.com/ihubo)

##捐助开发者
在兴趣的驱动下,写一个`免费`的东西，有欣喜，也还有汗水，希望你喜欢我的作品，同时也能支持一下。
当然，有钱捧个钱场（右上角的爱心标志，支持支付宝和PayPal捐助），没钱捧个人场，谢谢各位。

##感激
感谢以下的项目,排名不分先后

* [mou](http://mouapp.com/)
* [ace](http://ace.ajax.org/)
* [jquery](http://jquery.com)

##关于作者

```javascript
  var ihubo = {
    nickName  : "草依山",
    site : "http://jser.me"
  }
```