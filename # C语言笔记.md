# C语言

## 01 基础语法

### C语言版本

* 1983年美国国家标准局(American National Standards Institute，简称ANSI)成立了一个委员会，开始制定C语言标准的工作
* 1989年C语言标准被批准，这个版本的C语言标准通常被称为 ANSI C
* 1999年，国际标准化组织ISO又对C语言标准进行修订，在基本保留原来C语言特征的基础上，针对应该的需要，增加了一些功能，命名为 C99
* 2011年12月8日，ISO正式公布C语言新的国际标准草案：C11

***
***

### 程序简介

* 程序是由函数组成的，程序就是指令的集合

***

* 编译：就是把代码翻译成计算机能识别的 0 和 1
* Xcode使用 LLVM编译器（前端用clang）

***

* 链接：就是把自己编写的代码翻译的二进制文件和系统的函数库组合在一起，生成可执行文件

***

* 想输入有些有特殊含义的字符可以试着在前边加上一个 `\`

***

* 编写代码注意程序的可读性
	*  JAVA程序员：
	
	```
	int main() {
	
		printf("*** main函数 ***");
		return 0;
	}
	```
	
	* 其他程序员：
	
	```
	int main() 
	{
		printf("*** main函数 ***");
		return 0;
	}
	```

***
***

### 开始学习C语言

#### 关键字

* 关键字: 特殊含义的符号（也叫保留字）
* 一共32个
* 全部都是小写
* 紫褐色

#### 标识符

* 标识符: 自定义的一些符号和名称
* 标识符是用来区分
* 命名规则（一定要遵守）
	* 只能由26个英文字母的大小写、10个阿拉伯数字0~9、下划线_组成
	* 严格区分大小写，比如test和Test是2个不同的标识符
	* 不能以数字开头
	* 不可以使用关键字作为标识符
	
* 命名规范（最好遵守）
	* 尽量起个有意义的名称，比如一个完整的英文单词，别人一看这个名称就能才能这个标识符的作用。如果不懂英文，你也可以用拼音，尽量不要起像abcde、sfsdfsdf等这类看起来没有意义的名称
	* 如果标识符中含有多个单词，可以使用驼峰标识（除开第一个单词，后面每个单词的首字母都是大写）：firstName、myFirstName，或者使用下划线_来连接：first_name、my_first_name
	
#### 注释

* 单行注释: 以两个正斜杠开头，也就是以//开头，只能注释一行
* 多行注释: 以/\*开头，以\*/结尾，/\*和\*/中间的内容都是注释
* 注释的嵌套: 
	* 单行注释可以嵌套单行注释、多行注释
	
	```
	// 哇哈哈 // 呵呵呵
	// /* fsdfsdf */  // sdfsdfsd
	```
	
	* 多行注释可以嵌套单行注释
	
	```
	/*   	// 作者：wk 	// 描述：第一个C语言程序	作用：这是一个主函数，C程序的入口点  	*/
	```
	
	* 多行注释不能嵌套多行注释

#### 数据

* 静态数据
	* 概念：静态数据是指一些永久性的数据，一般存储在硬盘中。
	* 存储的时长：计算机关闭之后再开启，这些数据依旧还在，只要你不主动删掉或者硬盘没坏，这些数据永远都在。
	* 哪些是静态数据：静态数据一般是以文件的形式存储在硬盘上，比如文档、照片、视频等。
	
* 动态数据
	* 概念：动态数据指在程序运行过程中，动态产生的临时数据，一般存储在内存中。
	* 存储的时长：计算机关闭之后，这些临时数据就会被清除。
	* 哪些是动态数据：当运行某个程序（软件）时，整个程序就会被加载到内存中，在程序运行过程中，会产生各种各样的临时数据，这些临时数据都是存储在内存中的。当程序停止运行或者计算机被强制关闭时，这个程序产生的所有临时数据都会被清除。

#### 标识符

* 标识符: 自定义的一些符号和名称
* 标识符是用来区分
* 命名规则（一定要遵守）
	* 只能由26个英文字母的大小写、10个阿拉伯数字0~9、下划线_组成
	* 严格区分大小写，比如test和Test是2个不同的标识符
	* 不能以数字开头
	* 不可以使用关键字作为标识符
	
* 命名规范（最好遵守）
	* 尽量起个有意义的名称，比如一个完整的英文单词，别人一看这个名称就能才能这个标识符的作用。如果不懂英文，你也可以用拼音，尽量不要起像abcde、sfsdfsdf等这类看起来没有意义的名称
	* 如果标识符中含有多个单词，可以使用驼峰标识（除开第一个单词，后面每个单词的首字母都是大写）：firstName、myFirstName，或者使用下划线_来连接：first_name、my_first_name



