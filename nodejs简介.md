### node.js简介
	1.js运行在浏览器中，nodejs运行在服务器端 
	2.js的全局对象是window,nodejs的全局对象是global
	3.当node在执行模块中的代码时，所有的代码都默认被这个构造函数所包含；在函数执行时，同时传进了5个实参
		function(exports,require,module,__filename,__dirname){}
			exports:对象，将变量或函数暴露在外部
			require:函数，引入外部模块
			module:当前模块本身，exports是module的属性 module.exports ==  exports
			__filename:文件路径，当前模块的完整路径
			__dirname:文件夹路径，当前模块所在文件夹的完整路径
		




### node.js模块
	核心模块(nodejs官方提供的)
		eg:引入fs模块	var fs = require("fs")   
			require里直接写模块的名字
	文件模块(用户自己创建的)
		eg:在mode2.js中引入同路径下的mode.js文件		var md = require("./mode.js") 或者 var md = require("./mode")
			require里写文件的相对路径或绝对路径，一般写相对路径
	第三方模块(组织或个人公开的)
		下载地址：https://www.npmjs.com
		模块引用同核心模块一样
	
