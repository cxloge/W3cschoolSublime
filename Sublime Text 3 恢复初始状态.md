# Sublime Text 3 恢复初始状态

由 marlboro90 创建，最后一次修改 2016-10-18 15:41:06

通过删除数据文件夹，Sublime Text可以恢复到新安装的状态。 根据您的操作系统，此文件夹位于：

- OS X: `~/Library/Application Support/Sublime Text 3`
- Windows: `%APPDATA%\Sublime Text 3`
- Linux: `~/.config/sublime-text-3`

要恢复到初始状态，您可以：

1. 退出升级文本
2. 将数据文件夹移动到备份位置
3. 启动Sublime文本

重新启动时，将创建一个新的数据文件夹，就像第一次运行Sublime Text时一样。 请注意，这也会移除您的所有设置和程序包。 数据文件夹的备份副本可用于检索配置或无法重新安装的自定义包。

### OS X

在OS X上，默认情况下隐藏`〜/ Library`文件夹。 要在其中导航，请在Finder中选择 转到▸转到文件夹 菜单项，然后键入`〜/ Library`。

### Windows

在Windows中，缓存文件存储在一个单独的位置`％LOCALAPPDATA％\ Sublime Text 3`，以提高漫游配置文件的性能。