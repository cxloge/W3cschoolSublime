# Sublime Text中文输入法的问题

由 425389019 创建，最后一次修改 2016-02-24 15:49:29

## 中文输入法的问题

从Sublime Text的初版（1.0）到现在（3.0 3065），中文输入法（包括日文输入法）都有一个问题：输入框不跟随。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea708f646f9.jpg)

目前官方还没有修复这个bug，解决方法是安装IMESupport插件，之后重启Sublime Text问题就解决了。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea708fe1df6.jpg)

### 文件夹（Folders）

Sublime Text支持以文件夹做为单位进行编辑，这在编辑一个文件夹下的代码时尤其有用。在File下Open Folder：

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea70905611e.jpg)

你会发现右边多了一个侧栏，这个侧栏列出了当前打开的文件和文件夹的文件，使用Ctrl + K, Ctrl + B显示或隐藏侧栏，使用Ctrl + P快速跳转到文件夹里的文件。