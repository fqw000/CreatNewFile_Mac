# 访达里新建文件
- 点击即在当前文件夹新建空白文件
- 重命名修改后缀即可
- 不需要在使用终端新建文件

（MAC的希望你是使用软件管理工具，期望你打开软件新建文件而不是在访达里新建文件。）


访达-自定义工具栏-（将 [NewFile.app](https://github.com/fqw000/CreatNewFile_Mac/releases/download/mac/NewFile.app.zip) 拖入工具栏）

使用mac的 自动操作实现
代码如下：
```
on run {input, parameters}
	
	(* 实现文件夹新建文件 *)
	tell application "Finder"
	set selection to make new file at (get insertion location)
	end tell
	
	return input
end run
```


