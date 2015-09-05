#**Lua 基础**
---

1.  **Chunk：**

		chunk是一系列语句，Lua执行的每一块语句，比如一个文件或者交互模式下的每一行都是一个Chunk。

2.  **Block：**

		block是一列语句段；从语法上来说，一个block和一个chunk是相同的。

3.  **控制结构：**   
注意:控制结构的条件表达式结果可以是任何值，Lua认为false和nil为假，其他值为真。   
Lua选择结构
		
		选择结构if	
		stat ::= if exp then block {elseif exp then block} [else block] end

		例如：
		if a>10 then  print("超过10岁") 
			else print("小于10岁") 
   		end
Lua循环结构

		LUA的循环结构,有三种：
		（1）while exp do block end 
		（2）repeat block until exp 
		（3）for Name `=´ exp `,´ exp [`,´ exp] do block end
(1)while exp do block end

		while condition do
    		statements;
		end;
(2)repeat block until exp
		
		repeat
			statements;
		until conditions; 
(3)for   

		for在Lua中分为两种

		(1)普通数值for循环
		for var = exp1,exp2,exp3 do
			loop-part
		end
		--for将会从exp1(初始值)到exp2(终止值)结束，exp3是步长，默认exp3可以省略，步长为1
		例如：
		for i=10,1,-2 do
			print(i)
		end
		
		输出结果为10，8，6，4，2
		
		这里有几点需要注意：
		1、三个表达式只会计算一次，并且是在每次开始之前
		2、控制变量var是局部变量自动被声明，并且只在循环内有效
		3、循环过程中不要改变控制变量的值，那样做的结果是不可预知的。如果要退出循环请使用break。


		(2)泛型for循环（类似于foreach）：
		for namelist in explist do block end
		例如：
		days = {"Sundy", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"}
		for v in ipairs(days) do
			print(days[v])
		end