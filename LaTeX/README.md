
## 参考资料
- [CTEX : HomePage](http://www.ctex.org/HomePage)，关于 TEX 的中文网站
    - [常见问题集 (CTeX-FAQ)](http://www.ctex.org/CTeXFAQ#)，内含详细文档
- [一份其实很短的 LaTeX 入门文档](http://liam0205.me/2014/09/08/latex-introduction/)
- [如何在 OS X 上使用 LaTeX ？](https://www.zhihu.com/question/20928639)


## TeX软件
#### TeX发行版
- [CTEX : HomePage](http://www.ctex.org/HomePage)
    - CTeX 中文套装是基于 Windows 下的 MiKTeX 系统，集成了编辑器 WinEdt 和 PostScript 处理软件 Ghostscript 和 GSview 等主要工具。 
    - CTeX 中文套装在 MiKTeX 的基础上增加了对中文的完整支持。 
- [TeXLive (Unix/Linux/Windows)](https://www.tug.org/texlive/)
- [MacTeX (Mac OSX)](https://www.tug.org/mactex/)
- [MiKTeX (Windows)](https://miktex.org/)
- [ShareLaTex](https://www.sharelatex.com/)，在线工具
- [Overleaf](https://www.overleaf.com/)，在线工具

#### 编辑器
- TeXworks: TeX Live、MiKTeX、CTeX，简洁，推荐
- WinEdt: CTeX
- TeXshop: MacTeX，推荐
- Latexian
- TeXstudio
- ...

#### 模板
- [LaTeX Templates](http://www.latextemplates.com/)
- [ShareLaTex templates](https://www.sharelatex.com/templates)
- [howtoTeX](http://www.howtotex.com/)


## TeX 家族
#### TeX - LaTeX
> TeX 是高德纳（Donald Ervin Knuth，1938年1月10日 –）教授愤世嫉俗（大雾；追求完美）做出来的排版引擎，同时也是该引擎使用的标记语言（Markup Lang）的名称。这里所谓的引擎，是指能够实现断行、分页等操作的程序（请注意这并不是定义）；这里的标记语言，是指一种将控制命令和文本结合起来的格式，它的主体是其中的文本而控制命令则实现一些特殊效果（同样请注意这并不是定义）。

> LaTeX 则是 L. Lamport （1941年2月7日 – ） 教授开发的基于 TeX 的排版系统。实际上 LaTeX 利用 TeX 的控制命令，定义了许多新的控制命令并封装成一个可执行文件。这个可执行文件会去解释 LaTeX 新定义的命令成为 TeX 的控制命令，并最终交由 TeX 引擎进行排版。

总结：
- 最终进行断行、分页等操作的，是 TeX 引擎；
- LaTeX 实际上是一个工具，它将用户按照它的格式编写的文档解释成 TeX 引擎能理解的形式并交付给 TeX 引擎处理，再将最终结果返回给用户。

#### pdfTeX - pdfLaTeX
> TeX 系统生成的文件是 dvi 格式，虽然可以用其他程序将其转换为例如 pdf 等更为常见的格式，但是毕竟不方便。

> Hàn Thế Thành 博士在他的博士论文中提出了 pdfTeX 这个对 TeX 引擎的扩展。二者最主要的差别就是 pdfTeX 直接输出 pdf 格式文档，而 TeX 引擎则输出 dvi 格式的文档。

总结：
- pdfTeX：输出pdf
- pdfLaTeX：解释LaTeX，交由pdfTeX处理，生成pdf

#### XeTeX - XeLaTeX
> 高德纳教授在实现 TeX 的当初并没有考虑到中日韩等字符的处理，而只支持 ASCII 字符。这并不是说中日韩字符就无法使用 TeX 引擎排版了，事实上 TeX 将每个字符用一个框包括起来（这被称为盒子）然后将一个个的盒子按照一定规则排列起来，因而 TeX 的算法理论上适用于任何字符。ASCII 字符简单理解，就是在半角模式下你的键盘能直接输出的字符。

> XeTeX 引擎直接支持 Unicode 字符。

总结：
- XeLaTeX 和 XeTeX 的关系与 pdfLaTeX 和 pdfTeX 的关系类似
- 使用 XeTeX 引擎需要使用 UTF-8 编码

#### LuaTeX
> LuaTeX 是正在开发完善的一个 TeX引擎，相对它的前辈们还相当的不完善，这里不赘述。

#### CTeX-MiKTeX-TeX Live
> 之前介绍了 TeX, LaTeX, pdfTeX, pdfLaTeX, XeTeX, XeLaTeX, LuaTeX 等，他们都是 TeX 家族的一部分。但是作为一个能够使用的 TeX 系统，仅仅有他们还是不够的。

> CTeX, MiKTeX, TeX Live 都是被称为「发行」的软件合集。他们包括了上述各种引擎的可执行程序，以及一些文档类、模板、字体文件、辅助程序等等。其中 CTeX 是建立在 MiKTeX 的基础之上的。

#### 总结
> TeX - pdfTeX - XeTeX - LuaTeX 都是排版引擎，按照先进程度递增（LuaTeX 尚未完善）。

> LaTeX 是一种格式，基于 TeX 格式定义了很多更方便使用的控制命令。上述四个引擎都有对应的程序将 LaTeX 格式解释成引擎能处理的内容。

> CTeX, MiKTeX, TeX Live 都是 TeX 的发行，他们是许许多多东西的集合。



