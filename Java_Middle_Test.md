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

 ##### 整数型： byte short int long
  
 - 浮点型： float double
  
 - 字符型： char
  
 - 布尔型： boolean

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

##### this关键字

this可以出现在实例方法中，但不可以出现在类方法中。
实例方法只能通过对象来调用，不能用类名来调用。

##### 包语句
package <包名>;

##### 访问权限

- 访问权限	 本类	 本包的类	 子类	 非子类的外包类
- public	   是	    是	     是	     是
- protected	是    	是      是       否
- default	  是   	是	     否       否
- private	  是	    否	     否       否

- 1、public： 所修饰的类、变量、方法，在内外包均具有访问权限；
- 2、protected： 这种权限是为继承而设计的，protected所修饰的成员，对所有子类是可访问的，但只对同包的类是可访问的，对外包的非子类是不可以访问；
- 3、包访问权限（default）： 只对同包的类具有访问的权限，外包的所有类都不能访问；
- 4、private： 私有的权限，只对本类的方法可以使用；

##### 基本类型的类包装
- Double 类的构造方法：Double (double num)
- Float 类的构造方法：Float(float num)
- Char 的构造方法：Character(char c)

### 第五章

#### 子类的继承
- Java 不支持多继承，但支持多重继承。
- 同包中除了private不可继承，其余都可以继承
- 不同包中只有protected，public可以继承

class 父类 {
}
 
class 子类 extends 父类 {
}

#### 隐藏变量的重写
super.x ———— super.play()
访问和调用被子类隐藏的成员变量x和方法

##### 用super调用父类的构造方法
子类不继承父类的构造方法，子类在构造方法中需要使用super来调用父类的构造方法，super必须是子类构造方法中的头一句。

##### final关键字
final类不能继承

##### 上转型对象
 American是People的子类
 People people;
 American american=new American();
 people=american; people是american的上转型对象
 
##### 继承与多态
- 多态性指父类的某个实例方法被其子类重写时，可以产生自己的功能行为

##### abstract类和abstract方法
- abstract方法只允许申明，不允许实现，不允许使用final和abstract同时修饰一个方法

### 第六章——接口与多态

#### 接口申明与使用
- 申明： interface
- 接口体：接口体中只有抽象方法；常量的访问权限都是public（可以省略）
- 接口的使用：类通过使用implements申明自己实现一个或多个接口
- 如果父类实现某接口，子类不必再使用implements
注：一个类申明实现一个接口，但没有重写接口中的所有方法，这个类必须是abstract类

#### 接口回调





