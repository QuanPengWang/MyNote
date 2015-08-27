#**有关于windows下的命令行**
---

由于windows 10之前的命令行并不好用（win8.1没有使用过，不过好像应该也不怎么样吧？据说win 10已经对命令行进行了改进，变得很好用，谁知道呢？），这里在命令行下使用Lua不会有一个很好的体验。所以这里我个人推荐使用Cmder来代替windows系统自带的CMD。   

[**Cmder官方网站**](http://gooseberrycreative.com/cmder/)
这里我们只下载mini版本的就可以了，体积足够小巧。

安装方法：   
1.	将下载的cmder_mini.zip解压   
2.	将解压出来的文件夹写入环境变量中   
3.	通过快捷键win+alt+p:打开设置面板，去掉Monospace前面的勾选   
4.	将下面的4行命令添加到cmder/config/aliases文件末尾

		l=ls --show-control-chars 
		la=ls -aF --show-control-chars 
		ll=ls -alF --show-control-chars 
		ls=ls --show-control-chars -F
	