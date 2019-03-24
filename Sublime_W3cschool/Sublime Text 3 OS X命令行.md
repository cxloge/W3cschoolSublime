# Sublime Text 3 OS X命令行

由 marlboro90 创建，最后一次修改 2016-10-18 15:49:31
Sublime Text包括命令行工具，subl，用于在命令行上处理文件。这可以用在Sublime Text中打开文件和项目，以及用于unix工具的编辑器，例如git和subversion。

## 建立

第一个任务是建立一个符号链接到subl。假设你在应用程序文件夹中放置了Sublime Text，并且在路径中有一个〜/ bin目录，则可以运行：
```
ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" ~/bin/subl
```
## 用法
运行subl --help，

```
Usage: subl [arguments] [files]         edit the given files
   or: subl [arguments] [directories]   open the given directories
   or: subl [arguments] -               edit stdin

Arguments:
  --project <project>: Load the given project
  --command <command>: Run the given command
  -n or --new-window:  Open a new window
  -a or --add:         Add folders to the current window
  -w or --wait:        Wait for the files to be closed before returning
  -b or --background:  Don't activate the application
  -s or --stay:        Keep the application activated after closing the file
  -h or --help:        Show help (this message) and exit
  -v or --version:     Show version and exit

--wait is implied if reading from stdin. Use --stay to not switch back
to the terminal when a file is closed (only relevant if waiting for a file).

Filenames may be given a :line or :line:column suffix to open at a specific
location.
```

C:\Users\cxloge>subl -h
Sublime Text build 3126

Usage（用法）: 

| 用法                             | 描述                         | 描述      |
| ------------------------------ | -------------------------- | ------- |
| subl [arguments][files\]       | edit the given files       | 编辑给定的文件 |
| subl [arguments][directories\] | open the given directories | 打开给定的目录 |

Arguments（参数）:

| 参数                  | 描述                                       | 描述              |
| ------------------- | ---------------------------------------- | --------------- |
| --project <project> | Load the given project                   | 加载给定的项目         |
| --command <command> | Run the given command                    | 运行给定的命令         |
| -n or --new-window  | Open a new window                        | 打开一个新窗口         |
| -a or --add         | Add folders to the currenst window       | 将文件夹添加到当前窗口     |
| -w or --wait        | Wait for the files to be closed before returning | 等待文件关闭，然后返回     |
| -b or --background  | Don't activate the application           | 不要激活应用程序        |
| -s or --stay        | Keep the application activated after closing the file | 关闭文件后，保持应用程序的激活 |
| -h or --help        | Show help (this message) and exit        | 显示帮助（此消息）并退出    |
| -v or --version     | Show version and exit                    | 显示版本并退出         |

Filenames may be given a :line or :line:column suffix to open at a specific
location.（文件名可能被赋予：line或：line：column后缀以在特定的位置打开
位置。）



## 编辑

要使用Sublime Text作为许多提示输入的命令的编辑器，请设置EDITOR环境变量：
```
export EDITOR='subl -w'
```
指定-w将导致subl命令在文件关闭之前不退出。