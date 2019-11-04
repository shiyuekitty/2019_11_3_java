### 第一章

#### 1.java语言的特点

​	平台无关性

#### 2.JDK 和 JRE 有什么区别？

- JDK：Java Development Kit 的简称，java 开发工具包，提供了 java 的开发环境和运行环境。
- JRE：Java Runtime Environment 的简称，java 运行环境，为 java 的运行提供了所需环境。

具体来说 JDK 其实包含了 JRE，同时还包含了编译 java 源码的编译器 javac，还包含了很多 java 程序调试和分析的工具。简单来说：如果你需要运行 java 程序，只需安装 JRE 就可以了，如果你需要编写 java 程序，需要安装 JDK。

### 第二章

#### 1.标识符

- 标识符由字母、狭隘化县、美元符号和数字组成，长度不受限制。

- 标识符的第一个字符不能是数字字符。

- 标识符不能是关键字。

- 标识符不能是true、false、null。

  

  #### 2.基本数据类型

  #### 整数型： byte short int long
浮点型： float double
字符型： char
布尔型： boolean

  #### 3.输入输出

Scanner reader=new Scanner(System.in);

nextBoolen();

nextByte();

......

### 第三章

for(int i:a)

### 第四章 类与对象

##### 构造方法

函数名与类名相同，默认构造方法是无参数的

##### 方法重载

一个类中可以有多个方法具有相同的名字，但参数必须不同

