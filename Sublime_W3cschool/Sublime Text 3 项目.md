# Sublime Text 3 项目

由 marlboro90 创建，marlboro90最后一次修改 2016-10-18 14:00:15

Sublime Text中的项目由两个文件组成：.sublime项目文件（包含项目定义）和.sublime-workspace文件（包含用户特定数据，例如打开的文件和每个文件的修改）。

作为一般规则，.sublime-project文件将被检入版本控制，而.sublime-workspace文件不会。

## 项目格式

.sublime-project文件是JSON，并支持三个顶级部分：文件夹，包括文件夹，设置，文件设置覆盖和build_systems，用于特定于项目的构建系统。 一个例子：

```Json
{
    "folders":
    [
        {
            "path": "src",
            "folder_exclude_patterns": ["backup"],
            "follow_symlinks": true
        },
        {
            "path": "docs",
            "name": "Documentation",
            "file_exclude_patterns": ["*.css"]
        }
    ],
    "settings":
    {
        "tab_size": 8
    },
    "build_systems":
    [
        {
            "name": "List",
            "shell_cmd": "ls -l"
        }
    ]
}
```

## 文件夹

每个文件夹必须有一个路径，并且可以可选地具有设置file_exclude_patterns，file_include_patterns，folder_exclude_patterns，folder_include_patterns和follow_symlinks。 路径可以是相对于项目目录或完全限定路径。 文件夹也可以给出一个名称设置，以设置它们在侧栏上的显示方式。
早期版本的转换项目可能在文件夹下有一个mount_points条目。 如果您希望使用排除模式，则需要更改为上述格式。

## 设置


[设置](https://www.w3cschool.cn/sublimetext3/sublimetext3-settings.html)处可以使用`设置键`指定设置，并且将覆盖常规用户设置。 请注意，它们不会覆盖语法特定的设置。

## 构建系统

build_systems指定内联构建系统定义的列表。 除了常规构建系统设置之外，还必须为每个构建系统设置一个名称。 此处列出的构建系统将通过常规工具▸构建系统菜单提供。

