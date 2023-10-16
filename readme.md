# 访达里新建文件
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


