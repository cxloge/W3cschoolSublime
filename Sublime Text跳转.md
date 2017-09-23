# Sublime Text跳转

由 425389019 创建，最后一次修改 2016-02-24 15:49:29

## 跳转（Jumping）

Sublime Text提供了强大的跳转功能使得我们可以在不同的文件/方法/函数中无缝切换。就我的使用经验而言，目前还没有哪一款编辑器可以在这个方面超越Sublime Text。

### 跳转到文件

Ctrl + P会列出当前打开的文件（或者是当前文件夹的文件），输入文件名然后Enter跳转至该文件。

需要注意的是，Sublime Text使用模糊字符串匹配（Fuzzy String Matching），这也就意味着你可以通过文件名的前缀、首字母或是某部分进行匹配：例如，EIS、Eclip和Stupid都可以匹配EclipseIsStupid.java。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea706204b63.gif)

### 跳转到符号

尽管是一个文本编辑器，Sublime Text能够对代码符号进行一定程度的索引。Ctrl + R会列出当前文件中的符号（例如类名和函数名，但无法深入到变量名），输入符号名称Enter即可以跳转到该处。此外，还可以使用F12快速跳转到当前光标所在符号的定义处（Jump to Definition）。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea7062680d8.gif)

比较有意思的是，对于Markdown，Ctrl + R会列出其大纲，非常实用。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea7062b816f.jpg)

### 跳转到某行

Ctrl + G然后输入行号以跳转到指定行：

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea706332bcf.gif)

### 组合跳转

在Ctrl + P匹配到文件后，我们可以进行后续输入以跳转到更精确的位置：

1. @ 符号跳转：输入@symbol跳转到symbol符号所在的位置

2. ## 关键字跳转：输入#keyword跳转到keyword所在的位置

3. : 行号跳转：输入:12跳转到文件的第12行。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea7063829b0.gif)

所以Sublime Text把Ctrl + P称之为“Go To Anything”，这个功能如此好用，以至于我认为没有其它编辑器能够超越它。