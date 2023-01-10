# 《Markdown写作指南》项目

## 项目简介

### 为什么要写这本书

我希望通过这本小书来介绍一下个人对`Markdown`这种写作方式的看法和使用经验，以此来抛砖引玉，引起大家对`Markdown`更多的关注，进而将软件开源的精神推广至写作领域。毕竟，文字作品才是我们人类开发时间最长，数量最多的一种“软件”。

具体说来，写这本书的最初念头源自于一次在Facebook上的抱怨。由于我自己是一个`Markdown`的重度使用者，在日常做笔记、写文章、翻译书籍时，经常需要搜寻各种使用`Markdown`写作的解决方案。而与此同时，市面上的各种博客、论坛、云端笔记服务也都纷纷加入了对`Markdown`的支持，这说明使用这门标志语言的用户并不在少数，但我却惊讶地发现自己市场上竟然找不到一本介绍`Markdown`的专著。于是就在Facebook上分享了下面这个想法：

> 我是觉得markdown写作可以延伸出很多东西啊，写论文涉及LaTeX、Mermaid等，制作电子书涉及gitbook ，建构博客涉及Hexo，居然没人写本书！可惜了……

很自然地，这条想法分享的下面就有朋友留言建议我“不如你来写吧”。虽然当时我只是在表达自己需要这样一本书，最好请某位专业人士来写一本，但与朋友的讨论让我重新审视了自己所分享的这个想法。这个想法实际上说明了我为什么喜欢用`Markdown`来写作的原因：

- 第一，`Markdown`是开源软件，符合开放、自由、专注于任务，便于同行协作的工作哲学。
- 第二，`Markdown`符合“数据与呈现样式、用户界面分离”程序设计思维。
- 第三，`Markdown`的纯文本特性使我们可以想管理程序员源代码一样管理自己的文字作品。

总结一下，就是`Markdown`可以让人们“像写程序一样写作”，这让我意识到写这样一本书的意义已经不仅仅是介绍一门轻量级的标记语言，而是在推广一种强调自由、开放、合作的价值观和方法论了。而这种价值观和方法论原本就是我多年以来一直在坚持的，如今既然看到没有人写一本关于`Markdown`的专著，不如就自己来为它的推广做点事吧。

### 这本书写了些什么

在这本书中，我以一篇本科毕业论文的写作过程为导引，介绍了`Markdown`在完成论文的规划、撰写、修改、发布这些不同任务阶段中的应用。全书被分成了六个章节和两个附录：

- **第1章 使用Markdown写作**：在这一章中，我们介绍了`Markdown`是什么、它有什么优势和劣势以及它所倡导的写作理念。需要说明的是，这一章的内容是为对`Markdown`一无所知的朋友准备的。如果读者自认为已经对`Markdown`有所了解，或者不想纠缠于技术概念，想快点进入“如何使用`Markdown`”的议题，也可以选择跳过这一章。

- **第2章 写作的前期准备**：在这一章中，我们首先介绍了几款值得一试的`Markdown`编辑器。然后，我们以论文的前期规划为导引，带大家学习了使用`Markdown`的标记来拟定论文大纲、表列论文的参考资料、并通过设定待办事项来安排写作的进度。

- **第3章 撰写一篇论文**：在这一章中，我们继续以论文的正式写作过程为导引，逐步深入地介绍了其余主要的`Markdown`标记，以及它们的具体使用。这其中既会包含用来表示段落、强调、引用、代码这些基本元素的原生`Markdown`标记，也会涉及到与表格、图形相关的扩展标记，以及它们的基本用法。

- **第4章 谈谈数学问题**：在这一章中，我们首先介绍了如何在`Markdown`文档中插入$\LaTeX$标记，以呈现数学公式。然后，我们会具体介绍如何用$\LaTeX$标记来描述基本四则运算、二项式方程、矩阵运算以及集合运算等数学问题。

- **第5章 作品的审阅与维护**：在这一章中，我们围绕着如何”像维护程序项目一样维护`Markdown`项目“的议题展开了一系列的讨论。首先，我们介绍了一款可以让人们更专注于文字内容审阅和修改的`Markdown`编辑器。然后，考虑到`Markdown`的应用目前尚不够普及的现实问题，为了让更多的人参与作品的审阅，我们为大家介绍了一款专用于转换标记语言格式的工具。最后，为了从时间维度上对项目的修改进行管理，我们也对如何用git版本控制系统对`Markdown`项目进行管理和维护，做了一个基本介绍。

- **第6章 Markdown的其他应用**：在这一章中，我们为大家介绍了如何用`Markdown`制作演示文稿、线上电子书以及撰写博客。集中展示了`Markdown`作为一种写作方式的广泛适用性。

- **附录A Makefile简易教程**：在这篇附录中，我们为大家介绍了`Makefile`文件的基本写法，以便搭配第5章中介绍的格式转换工具批量地将`Markdown`文档转换成其他格式的文档。

- **附录B 了解一下Node.js**：考虑到本书介绍的gitbook和Hexo都要基于Node.js运行环境来部署，而这个运行环境如今已经形成了如此庞大的软件生态系统，我认为有必要用一篇附录专门介绍一下Node.js以及它的安装和配置。

## 项目结构

本项目是一个基于`Markdown`实现的自由书籍项目，其目录结构如下：

- `src`：用于存储书籍的`Markdown`源码。
- `PDF`：用于存储书籍源码输出的PDF文档。
- `docx`：用于存储书籍源码输出的Microsoft Word文档。
- `LaTeX`：用于存储书籍源码输出的$\LaTeX$文档。
- `review`：用于存储审阅者对书籍提出的批注文档。

## 审阅规则

本书审阅者需使用word审阅工具对`docx`或`PDF`目录中的章节进行审阅，并将结果保存在`review`目录中，文件名应为`[源文件名]_by_[yourID].docx`或`[源文件名]_by_[yourID].pdf`，具体可参考该目录下已有的范例。

## 版权声明

此书译稿版权由作者本人与人民邮电出版社技术分社所有，本项目的用户可阅读、讨论本项目的所有内容。但不可转载并用于商业用处。如果发现侵权行为，人民邮电出版社将视具体情况追究法律责任。另外，希望各位看官体谅创作不易，如觉得本作品值得一读，还请前往人民邮电出版社异步社区[个人专栏销售处](https://www.epubit.com/columnDetails?id=CL6c695f34d7aec)，支付一些费用，鼓励一下原创。
