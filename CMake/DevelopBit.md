# 使用CMake判断当前开发环境是32位还是64位
---

这里我们主要使用**${CMAKE_SIZEOF_VOID_P}**这个**CMake内置变量**来进行判断
**${CMAKE_SIZEOF_VOID_P}**  : 变量代表了 void指针的长度

下面是一段示例：

		message(" the program is : " ${CMAKE_SIZEOF_VOID_P})
        
		if(${CMAKE_SIZEOF_VOID_P} STREQUAL 4)
			message("Current Develop Environment is 32")
		elseif(${CMAKE_SIZEOF_VOID_P} STREQUAL 8)
  			message("Current Develop Environment is 64")
		endif()

通过上述代码，可以在CMake输中看到当前的开发环境是32位的还是64位的
需要注意的是，这个判断环境的方式，是和当前系统本身位数无关，只和开发环境有关


