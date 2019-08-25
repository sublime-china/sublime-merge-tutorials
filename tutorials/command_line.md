# 命令行  
> [原文地址](https://www.sublimemerge.com/docs/command_line)  


`Sublime Merge`包含一个命令行工具`smerge`, 用于在命令行上处理仓库(repo), 这个工具能打开仓库, 搜索, 合并文件.  


## 设置(Setup)  

- Windows  
添加`C:\Program Files\Sublime Merge`到环境变量的`%PATH%`中  

- Mac  
`ln -s "/Applications/Sublime Merge.app/Contents/SharedSupport/bin/smerge" ~/bin/smerge`  

- Linux  
`ln -s /opt/sublime_merge/sublime_merge ~/bin/smerge`  

## 使用(Usage)  

Run `smerge --help`:  

```
Usage: smerge path               Open the given repository
    or: smerge search query       Search for commits in the current repository
    or: smerge blame file [line]  Blame the given file in the current repository
    or: smerge log file           Show the file history in the current repository
    or: smerge mergetool          Opens the merge tool for the given files
        [--no-wait] [base] left right [-o merged]

    -n or --new-window:      Open a new window
    -b or --background:      Don't activate the application
    -h or --help:            Show help (this message) and exit
    -v or --version:         Show version and exit
```

## Git Merge Tool Setup  

合并工具可用于从命令行处理Git仓库中的合并冲突.  
使用上面的说明配置smerge之后，从仓库目录运行以下操作:  

```
git config mergetool.smerge.cmd 'smerge mergetool "$BASE" "$LOCAL" "$REMOTE" -o "$MERGED"'
git config mergetool.smerge.trustExitCode true
git config merge.tool smerge
```

## Git Merge Tool Usage  

调用合并工具, 运行:  
```
git mergetool
```

## mac下可以直接用brew安装(from [issues](https://github.com/sublime-china/sublime-merge-tutorials/issues/1))  

```
brew cask install sublime-merge
```
自动创建命令行smerge的软链接  
