# Sublime Text 3 缩进设置

由 marlboro90 创建，marlboro90最后一次修改 2016-10-18 14:47:07

缩进设置确定标签的大小将停止，并控制Tab键是否应该将选项卡或空格。 除了自动检测之外，还可以对它们进行全局自定义，每文件类型或每个文件。

## 设置

| tab_size                 | 整数。一个标签的空格数被认为是相等的                       |
| ------------------------ | ---------------------------------------- |
| translate_tabs_to_spaces | 布尔值。如果为true，则在按下标签时空格将插入到下一个标签位，而不是插入标签字符 |
| detect_indentation       | 布尔值。如果为true（默认值），则在加载文件时将自动计算标签字符大小和translate_tabs_to_spaces |
| use_tab_stops            | 布尔值。如果translate_tabs_to_spaces为true，use_tab_stops将使标签字符和退格插入/删除直到下一个标签位 |

## 设置文件

------

按照以下顺序查询设置文件：

1. Packages/Default/Preferences.sublime-settings
2. Packages/Default/Preferences (<platform>).sublime-settings
3. **Packages/User/Preferences.sublime-settings**
4. Packages/<syntax>/<syntax>.sublime-settings
5. **Packages/User/<syntax>.sublime-settings**

一般来说，您应该将您的设置放在Packages / User / Preferences.sublime-settings中。 如果要指定某个文件类型的设置（例如Python），则应将它们放在Packages / User / Python.sublime-settings中。

## 按语法设置

------

可以在每个语法的基础上指定设置。 您可以使用

首选项▸设置 - 语法特定菜单

编辑当前语法的设置。

## 缩进检测

------

加载文件时，将检查其内容，并为该文件设置tab_size和translate_tabs_to_spaces设置。 状态区将报告这种情况发生时。 虽然这通常工作很好，你可能要禁用它。 你可以使用detect_indentation设置。

缩进检测可以通过

查看▸缩进▸想设置从缓冲区

设置菜单运行detect_indentation命令手动运行。

## 在标签和空格之间转换

------

查看▸缩进菜单

具有用于转换当前文件中标签和空格之间的前导空格的命令。 这些菜单项运行展开选项卡和unexpand选项卡命令。

| auto_indent                | 布尔值，默认情况下启用。 启用自动缩排                      |
| -------------------------- | ---------------------------------------- |
| smart_indent               | 布尔值，默认情况下启用。 使自动缩进更轻松一些，例如，缩进在C语句的if语句后面的下一行。 |
| trim_automatic_white_space | 布尔值，默认情况下启用。 修剪由光标移动插入符号时由auto_indent添加的空格。 |
| indent_to_bracket          | 布尔值，默认情况下禁用。 在缩进时将空格添加到第一个打开的括号。 在缩进时使用：`use_indent_to_bracket(to_indent,                      like_this);` |