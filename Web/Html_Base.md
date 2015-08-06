#HTML 基础
- - -

- 通常我们会把<!DOCTYPE html>放在首行，用以告知浏览器我们的语言是何种编程语言，在这里当然是html啦！

- - -

##在一个html文件中，主要有两部分：head和body

- - -

###head
- head包含着html的信息，例如html的标题(title)

###body
- body中则存放text，超链接，图片等内容

- 从&lt;h1&gt;一直到&lt;h6&gt;能够显示大小不同的标题，h1标题最大，h6标题最小

- 超链接

		<a href="www.baidu.com">百度</a>
		
- 图片

		<img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" />
		
- 给图片加超链接

		<a href="http://www.codecademy.com"><img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" /></a>
		

- 有序列表：

		<ol>
    		<li>Test1</li>
    		<li>Test2</li>
    		<li>Test3</li>
    		<li>Test4</li>
		</ol>
	


- 无序列表：

		<ul>
    		<li>Test1</li>
    		<li>Test2</li>
    		<li>Test3</li>
    		<li>Test4</li>
		</ul>