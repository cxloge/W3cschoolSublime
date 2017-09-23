# Sublime Text 3 拼写检查

由 marlboro90 创建，marlboro90最后一次修改 2016-10-18 14:59:57

Sublime Text使用Hunspell的拼写检查支持。 可以从OpenOffice.org扩展列表中获取其他字典。

可以通过Sublime Text使用的格式的字典可在<https://github.com/titoBouzout/Dictionaries>获取。

## 词典

------

Sublime Text目前只支持UTF-8编码的字典。 大多数字典不是以UTF-8编码的，而是对所讨论的语言使用更紧凑的编码。 要使用带有Sublime Text的词典，首先需要将其转换为UTF-8。

一旦您有一个UTF-8编码词典，它可以通过将它放在一个package，例如`Packages / User`，您可以从**首选项/浏览插件**菜单项访问安装。 一旦文件就位，您可以从**查看/词典**菜单中选择字典。

## 设置

------

有两个影响拼写检查的设置：拼写检查，启用拼写检查的控制，以及词典，它提供要使用的词典文件的路径。 例如：

```
"spell_check": true,
"dictionary": "Packages/Language - English/en_US.dic"

```

添加和忽略的单词存储在用户设置下添加的单词和忽略单词的键。

## 命令

------

- `next_misspelling`：选择下一个拼写错误
- `prev_misspelling`：选择上一个拼写错误
- `add_word`：将单词参数给出的单词添加到添加列表
- `ignore_word`：将单词参数给出的单词添加到忽略列表中

