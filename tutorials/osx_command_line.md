# [Sublime Merge] Mac命令行

> 在Mac系统中, Sublime Merge有一个命令行工具. 方便我们在终端模式中打开Git本地仓库.

## 设置

`ln -s "/Applications/Sublime Merge.app/Contents/SharedSupport/bin/smerge" ~/bin/sm`

## 使用

Run `sm -h`

```shell
Sublime Merge build 1075

Usage: sm path               Open the given repository
   or: sm search query       Search for commits in the current repository
   or: sm blame file [line]  Blame the given file in the current repository
   or: sm log file           Show the file history in the current repository

  -n or --new-window:      Open a new window
  -b or --background:      Don't activate the application
  -h or --help:            Show help (this message) and exit
  -v or --version:         Show version and exit
```
