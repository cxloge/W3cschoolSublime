# Sublime Text编辑

由 425389019 创建，最后一次修改 2016-02-24 15:49:27

## 编辑（Editing）

Sublime Text的编辑十分人性化——它不像Vim那样反人类（尽管我也用Vim但我还是要说Vim的快捷键设定绝壁连代谢产物都不如），少量的快捷键就可以完成绝大多数编辑任务。

### 基本编辑（Basic Editing）

↑↓←→就是↑↓←→，不是KJHL，（没错我就是在吐槽Vim，尼玛设成WSAD也比这个强啊），粘贴剪切复制均和系统一致。

Ctrl + Enter在当前行下面新增一行然后跳至该行；Ctrl + Shift + Enter在当前行上面增加一行并跳至该行。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea6fe6e46c6.gif)

Ctrl + ←/→进行逐词移动，相应的，Ctrl + Shift + ←/→进行逐词选择。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea6fe73cbed.gif)

Ctrl + ↑/↓移动当前显示区域，Ctrl + Shift + ↑/↓移动当前行。

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea6fe7e74dc.gif)

### 选择（Selecting）

Sublime Text的一大亮点是支持多重选择——同时选择多个区域，然后同时进行编辑。

Ctrl + D选择当前光标所在的词并高亮该词所有出现的位置，再次Ctrl + D选择该词出现的下一个位置，在多重选词的过程中，使用Ctrl + K进行跳过，使用Ctrl + U进行回退，使用Esc退出多重编辑。

多重选词的一大应用场景就是重命名——从而使得代码更加整洁。尽管Sublime Text无法像IDE（例如Eclipse）那样进行自动重命名，但我们可以通过多重选词+多重编辑进行直观且便捷的重命名：

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea6fe878084.gif)

有时我们需要对一片区域的所有行进行同时编辑，Ctrl + Shift + L可以将当前选中区域打散，然后进行同时编辑：

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea6fe901984.gif)

有打散自然就有合并，Ctrl + J可以把当前选中区域合并为一行：

![img](https://img.w3cschool.cn/attachments/image/cimg/2015-09-05_55ea6fe9640b1.gif)