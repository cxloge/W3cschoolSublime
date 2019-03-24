# Sublime Text 3 设置

由 marlboro90 创建，marlboro90最后一次修改 2016-10-18 14:01:45

Sublime Text有许多不同的设置来自定义它的行为。 通过编辑文本文件来更改设置：虽然这比使用GUI有点棘手，但您可以获得灵活的系统。

## 设置

------

可通过**首选项▸设置**菜单项访问设置。 **左侧窗格**包含所有默认设置，以及每个的说明。 **右侧窗格**是可以保存自定义的位置。

## 设置文件

------

按照以下顺序查询设置文件：

1. Packages/Default/Preferences.sublime-settings
2. Packages/Default/Preferences (<platform>).sublime-settings
3. **Packages/User/Preferences.sublime-settings**
4. <Project Settings>
5. Packages/<syntax>/<syntax>.sublime-settings
6. **Packages/User/<syntax>.sublime-settings**
7. <Buffer Specific Settings>

## 按语法设置

------

首选项▸设置 - 语法特定菜单

## 按项目设置

设置可以基于每个项目设置，详细信息在[项目文档](https://www.w3cschool.cn/sublimetext3/sublimetext3-projects.html)中。

## 无干扰的设置

------

[无干扰模式](https://www.w3cschool.cn/sublimetext3/sublimetext3-distractionfree.html)应用了一个额外的设置文件（Distraction Free.sublime-settings）。 您可以在这里放置文件设置，以使它们只适用于无干扰模式 - 从**首选项▸设置 - 无干扰模式**的菜单项访问它。

## 用键更改设置

------

toggle设置命令可用于切换设置。 例如，要进行切换当前文件上的word_wrap设置的键绑定，可以使用（在首选项▸键绑定中）：

```
{
    "keys": ["alt+w"],
    "command": "toggle_setting",
    "args":
    {
        "setting": "word_wrap"
    }
}

```

```
{
    "keys": ["ctrl+k", "ctrl+c"],
    "command": "set_setting",
    "args":
    {
        "setting": "color_scheme",
        "value": "Packages/Color Scheme - Default/Cobalt.tmTheme"
    }
}

```

## 故障排除

------

```
view.settings().get('font_face')
```