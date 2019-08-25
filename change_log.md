# 更新日志

### BUILD 1107    
> 12 March 2019    

- 侧边栏的'Contents'部分, 现在可以在`showing changed`和`all files`之间切换.  
> 空格键或者鼠标多点一次当前文件的标题.  
- `Sublime Merge`现在可以当成一个独立的合并工具, 通过命令行的`smerge --help`查看详情.  
- Merge tool: 改进原始文件和合并文件之间切换UI显示效果.  
- 添加`Navigate/Go to Parent`菜单项.  
> 如果分支很多, 合并线条很复杂的情况下, 这个功能可以很方便的找到当前分支当前commit的上一个commit.  
- 改进`clone`对话框.  
- 各种语法高亮的改进.  
- Merge tool now indicates which lines have been modified in the merged file  
- Merge tool: swap_line_up, swap_line_down and duplicate_line commands are now supported  
- 解决`git flow`命令显示高度不一致的bug  
- Mac: 对苹果系统`native tabs`的完全支持.  
- Mac: 确保菜单在缩放时的显示.  
- Mac: 错误信息对话框不能通过Esc键关闭.  
- Linux: Color glyphs are now drawn properly on light backgrounds  
- Windows: Fix DirectWrite handling of fonts with lineGap > 0  


### Build 1084    
> 29 October 2018    

- 搜索: 添加`contents:`操作符, 以找到提交信息或删除文本.    
- 现在可以忽略差异中的空白更改(可从上下文菜单中获得).    
- 编辑提交: 增加`Squash Selected Commits`.    
- 支持`core.worktree`.    
- 重新打开仓库时, 恢复当前的窗口状态.    
- 搜索: 当查询信息包含`path:`, `file:`, 或者`contents:`, 指定的`min-parents: 0`, 合并信息会自动的排除在外.    
- 位置栏: 如果标签的名称中有斜杠, 标签会被分组到文件夹中.    
- 调整提交视图的效果.    
- 添加新的偏好, `time_format`.    
- 偏好: 现在显示默认值, 而不是`null`.    
- 偏好: 接受不带引号的字符串.(这个比较屌orz... By Floyda)    
- 优化了因仓库文件系统而造成的网络问题.    
- 导航到提交现在可以像预期的那样进行隐藏提交    
- 解决了上下文拆分器超过hunk头部的Bug.    
- 解决了启动时, `expand_merge_commits_by_default`不能正常使用的Bug.    
- 解决了粗体字文本在侧边栏有时不能正常显示的Bug.    
- 解决了一个1079版本的回归问题.    
- Mac: 添加`gpu_window_buffer`设置, 以禁用OpenGL的使用.    
