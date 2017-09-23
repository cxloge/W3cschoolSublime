# Sublime Text 3 Packages

由 marlboro90 创建，最后一次修改 2016-10-18 15:25:02

Packages是Sublime Text：插件，语法高亮定义，菜单，片段等使用的资源文件的集合。 Sublime Text附带多个Packages，并且有更多的用户创建的Packages可用。

Packages存储在`.sublime-package`文件中，这是具有不同扩展名的`zip`文件。 Packages也可以解压缩存储在目录中，或者两者混合使用：Packages目录中的任何松散文件将覆盖存储在`.sublime-package`文件中的文件。

## 位置

------

Packages

压缩包可以存储在：

- `<executable_path>/Packages`
- `<data_path>/Installed Packages`

Loose packages可以存储在：

- `<data_path>/Packages`

例如，Python包存储在`<executable_path>/Packages/Python.sublime-package` 中，`<data_path> / Packages / Python`目录中的任何文件都将覆盖存储在`.sublime-package`文件中的那些文件。

一般来说，`<executable_path>/Packages`用于随Sublime Text一起提供的 packages，`<data path> / Installed Packages`用于由用户安装的packages。

## Special Packages

有两个特殊的包：默认和用户。 默认总是先排序，User总是排在最后。 软件包排序在软件包之间合并文件时生效，例如

```
Main.sublime-menu
```

。 任何包可能包含一个名为

```
Main.sublime-menu
```

的文件，但这不会覆盖主菜单，而是根据包的顺序合并文件。

`Default`和`User`之外的软件包按字母顺序排序。

## 创建一个新的包

------

要创建新包，只需在

```
<data_path> / Installed Packages
```

下创建一个新目录。 您可以从

首选项/浏览插件

菜单访问此目录。

从压缩包中覆盖文件

------

要覆盖现有包中的文件，只需在

```
Packages / <Package Name
```

\>目录下创建相同名称的文件。

例如，要覆盖Sublime Text附带的

```
Python.sublime-package
```

包中的

```
function.sublime-snippet
```

文件，在

```
<data_path> / Packages
```

目录下创建一个名为Python的目录，并将

```
function.sublime-snippet
```

文件放在那里。