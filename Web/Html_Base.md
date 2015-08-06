#** HTML 基础**
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

		&lt;a href="www.baidu.com"&gt;百度&lt;/a&gt;
		
- 图片

		&lt;img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" /&gt;
		
- 给图片加超链接

		&lt;a href="http://www.codecademy.com"&gt; &lt;img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" /&gt;&lt;/a&gt;
		

- 有序列表：

		&lt;ol&gt;
    		&lt;li>Test1&lt;/li&gt;
    		&lt;li>Test2&lt;/li&gt;
    		&lt;li>Test3&lt;/li&gt;
    		&lt;li>Test4&lt;/li&gt;
		&lt;/ol&gt;


- 无序列表：

		&lt;ul&gt;
    		&lt;li&gt;Test1&lt;/li&gt;
    		&lt;li&gt;Test2&lt;/li&gt;
    		&lt;li&gt;Test3&lt;/li&gt;
    		&lt;li&gt;Test4&lt;/li&gt;
		&lt;/ul&gt;