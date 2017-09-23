# Sublime Text前言

由 425389019 创建，最后一次修改 2016-02-24 15:49:23

## 前言（Prologue）

Sublime Text是一款跨平台代码编辑器（Code Editor），从最初的Sublime Text 1.0，到现在的Sublime Text 3.0，Sublime Text从一个不知名的编辑器演变到现在几乎是各平台首选的GUI编辑器。而这样优秀的编辑器却没有一个靠谱的中文教程，所以我试图通过本文弥补这个缺陷。

### 编辑器的选择（Editor Choices）

从初学编程到现在，我用过的编辑器有EditPlus、UltraEdit、Notepad++、Vim、TextMate和Sublime Text，如果让我从中推荐，我会毫不犹豫的推荐Vim和Sublime Text，原因有下面几点：

1. **跨平台**：Vim和Sublime Text均为跨平台编辑器（在Linux、OS X和Windows下均可使用）。作为一个程序员，切换系统是常有的事情，为了减少重复学习，使用一个跨平台的编辑器是很有必要的。
2. **可扩展**：Vim和Sublime Text都是可扩展的（Extensible），并包含大量实用插件，我们可以通过安装自己领域的插件来成倍提高工作效率。
3. **互补**：Vim和Sublime Text分别是命令行环境（CLI）和图形界面环境（GUI）下的最佳选择，同时使用两者会大大提高工作效率。

### 个人背景（Personal Background）

我是一名非常典型的程序员：平时工作主要在Linux环境下使用Java和Python，偶尔会用HTML+CSS+JavaScript编写网页；业余时会在Windows环境编写一些C#程序（包括控制台程序（Console Application）和移动应用（Mobile App），也会玩一些非主流语言（比如Haskell，ML和Ruby等）以拓展见识。

所以这篇文章会我的个人工作内容为主要使用场景（Scenario），尽管无法覆盖到所有的使用场景，但我认为依然可以覆盖到绝大部分，如果您认为我遗漏了什么内容，请在文章下面回复，我会尽量更新。

### 本文风格（Writing Style）

受益于[K&R C](http://en.wikipedia.org/wiki/The_C_Programming_Language)的写作风格，我倾向于以实际案例来讲解Sublime Text的功能，所以本文中的例子均源于我在实际开发时遇到的问题。

此外，把本文会使用大量动画（GIF）演示Sublime Text的编辑功能，因为我发现图片难以演示完整的编辑流程（Workflow），而视频又过于重量级。本文的GIF动画均使用[ScreenToGif](http://screentogif.codeplex.com/)进行录制。

### 编辑器（Editor） vs 集成开发环境（Integrated Development Environment，下文简称IDE）

我经常看到一些程序员拿编辑器和IDE进行比较，诸如Vim比Eclipse强大或是Visual Studio太慢不如Notepad++好使之类的讨论比比皆是，个人认为这些讨论没有意义，因为编辑器和IDE根本是面向两种不同使用场景的工具：

- 编辑器面向无语义的纯文本，不涉及领域逻辑，因此速度快体积小，适合编写单独的配置文件和动态语言脚本（Shell、Python和Ruby等）。
- IDE面向有语义的代码，会涉及到大量领域逻辑，因此速度偏慢体积庞大，适合编写静态语言项目（Java、C++和C#等）。

我认为应当使用正确的工具去做有价值的事情，并把效率最大化，所以我会用Eclipse编写Java项目，用Vim编写Shell，用Sublime Text编写JavaScript/HTML/Python，用Visual Studio编写C#。

前言到此结束，下面进入正题。