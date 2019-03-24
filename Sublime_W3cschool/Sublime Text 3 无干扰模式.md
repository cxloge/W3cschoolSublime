# Sublime Text 3 无干扰模式

由 marlboro90 创建，marlboro90最后一次修改 2016-10-18 11:11:03

无干扰模式将全屏显示您的文件，只有文本显示在显示器的中心。所有UI Chrome都已隐藏，但可以访问。 无干扰模式可以通过`查看(v)`▸`进入/退出无干扰模式`项进入。

当进入无干扰模式所有UI Chrome（侧边栏，小地图，状态栏等）都将被隐藏。您可以通过“`查看（V）`”菜单选择性地启用UI的某些部分 - 下次您进入无干扰模式时，系统会记住您的设置。

## 自定义

------

当在无干扰模式时，某些设置将被应用。默认设置（located in Packages/Default/Distraction Free.sublime-settings）是：

```
{
    "line_numbers": false,
    "gutter": false,
    "draw_centered": true,
    "wrap_width": 80,
    "word_wrap": true,
    "scroll_past_end": true
}

```

您可以通过编辑`Packages / User / Distraction Free.sublime`设置来自定义这些**设置，通过首选项▸设置 - 无干扰模式**菜单项可以访问。

这是值得注意的wrap_width设置，上面。 值为80导致包装发生在80个字符。 您可能希望将它设置为一个较高的值，或者换到窗口宽度，将其设置为0。