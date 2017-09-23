# Sublime Text 3 经典模式

由 marlboro90 创建，最后一次修改 2016-10-18 11:39:36

经典模式是开放的，补丁是受欢迎的。 如果你想贡献，细节在[GitHub repo](https://github.com/sublimehq/Vintage)。

## 启用经典模式

------

经典模式是默认禁用的，通过ignored_packages设置。 如果从忽略包列表中删除“Vintage”，您可以使用vi键进行编辑：

选择**首选项▸设置菜单项**
编辑`ignored_packages`设置，将其更改为：

```
"ignored_packages": ["Vintage"]

```

```
"ignored_packages": []

```

未启用经典模式 - 您会在状态栏中看到“`INSERT MODE`”

默认在默认情况下开始插入模式。这可以通过将以下设置添加到您的用户设置来更改：

```
"vintage_start_in_command_mode": true

```

## 包含的内容

经典模式包括最基本的动作：d（删除），y（复制），c（更改），gu（小写），gU（大写），g〜 （rot13），<（unindent）和>（indent）。
它还包括许多运动，包括l，h，j，k，w，w，e，E，b，B，alt + w（通过子词移动），alt + W（通过子词向后移动） $，^，％，0，G，gg，f，F，t，T，^ f，^ b，H，M和L.
支持文本对象，包括单词，引号，括号和标签。
重复（'。'）在那里，指定命令和动作的计数。 支持寄存器，宏和书签。 还支持许多其他杂项命令，例如*，/，n，N，s，S等。

插入模式是常规的Sublime Text编辑，与通常的Sublime Text键绑定：vi插入模式键绑定不会被模拟。
Ex命令不实现，除了：w和：e，它们通过命令选项板工作。

## Under the Hood

------

经典模式完全通过键绑定和插件API实现 - 随意浏览Vintage包，看看它是如何组合在一起的。 例如，如果你想绑定“jj”退出插入模式，你可以添加这个键绑定：

```
{
    "keys": ["j", "j"],
    "command": "exit_insert_mode",
    "context":
    [
        { "key": "setting.command_mode", "operand": false },
        { "key": "setting.is_widget", "operand": false }
    ]
}

```

## OS X Lion

------

在Lion中，按住某个键不会重复，而是会显示一个弹出式菜单，在字符变体之间进行选择。 这不适用于命令模式，所以你可能要禁用它。 这可以通过在终端输入：

```
defaults write com.sublimetext.2 ApplePressAndHoldEnabled -bool false

```

## 

## Ctrl键

------

经典模式下所支持的Ctrl键绑定：

- Ctrl + [：Escape
- Ctrl + Z：重做
- Ctrl + Y：向下滚动一行
- Ctrl + E：向上滚动一行
- Ctrl + F：下一页
- Ctrl + B：Page Up

```
"vintage_ctrl_keys": true

```

## Ex模式

------

VintageEx