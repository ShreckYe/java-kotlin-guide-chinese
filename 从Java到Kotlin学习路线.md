# 从Java到Kotlin学习路线
本文是我个人总结的在已经学会C或Python的基础上的从Java到Kotlin的学习路线。在按照本文学习之前，请确保你已至少熟悉C或Python其中一门编程语言。本文会略去一些已经过时的Java知识点（如Applet、JSP），这些知识点不推荐学习但你可以自己去了解；本文不包含Java企业框架和一些传统的企业Java库的知识点（如Spring、Tomcat相关知识等），这些框架国内很大部分软件公司Java开发使用较多、但国外厂商使用较少并有其他技术可以替代，作者不是很喜欢这些框架因为较多使用字符串反射而不方便混淆也不易阅读源码、内容太多较为臃肿、相关开发软件很多收费这些特点，同时Kotlin有更简洁的替代方案，因此本文不包含这些内容，若你工作方向与这些相关且想要了解，请自行查阅相关资料。

## 入门Java
### 知识点（C和Python均涉及的基本知识点已省略）
理解入门知识：
1. 基本类型与引用类型
1. 类与对象
1. 局部变量、成员变量与成员函数、静态变量与静态函数、常量
1. 访问控制修饰符（看懂就行，不用记忆）
1. 控制语句：两种for循环、switch、三元运算符

理解面向对象编程（OOP）与其三大特征继承、多态、封装：
1. 继承：子类继承父类
1. 多态：重载、重写、用父类/接口变量存储子类/接口对象
1. 封装：重点理解private与protected访问控制修饰符
1. 接口与抽象类

理解进阶实战知识：
1. 常用数据结构：Iterator、List、Set、Map、ArrayList、HashSet、TreeSet、HashMap、TreeMap、AbstractList、AbstractSet、AbstractMap等（哪些是接口、抽象类、非抽象类？每一个又继承/实现了哪些类/接口？）
1. 泛型
1. Java8的lambda表达式

上文未涉及的其他知识可以现学现用，与实战相结合更合适，不需要在没有实际项目经验和项目需求的时候提前盲目学习。

### 环境配置
安装JDK，最新版本为14：http://jdk.java.net/14/
安装IDE，推荐IntelliJ IDEA Community：https://www.jetbrains.com/idea/download/

### 推荐入门教程
1. 英文交互式APP教程：[Java Tutorial | SoloLearn: Learn to code for FREE!](https://www.sololearn.com/Course/Java/)
1. 中文教程：[Java 教程 | 菜鸟教程](https://www.runoob.com/java/java-tutorial.html)中的以上知识点相关内容

### 进阶教程
1. 系统理解Java的每一个细节：《Java编程思想》
1. 从软件工程和编程语言理论的角度了解Java的常用设计模式、常见错误、语言设计的利与弊等，高效编码：《Effective Java》
1. 理解JVM（Java虚拟机）并联系操作系统、编译器等知识

## 学习Kotlin
Kotlin基本可以实现Java能实现的所有功能，可以与Java相互调用、语法更加简洁、更好地支持函数式编程与DSL、并且拥有强大的跨平台性除兼容JVM生态外可兼容JavaScript生态、Android生态、iOS生态和LLVM支持的原生生态。

详细内容未完待续。

### 推荐教程
详细内容未完待续。

## Scala
Scala是JVM上的以函数式编程为主的多范式语言，很好地结合了面向对象编程（代表语言：Java）与函数式编程（代表语言：Haskell）两种范式，常用于并行计算、大数据处理等。由于出自学术界，此门语言难度较大，基本入门需要一定的数据结构与算法、操作系统的计算机科学知识基础，而进阶理解需要一定的编译原理、编程语言理论、计算模型、类型系统的理论计算机科学知识基础和线性代数、抽象代数和范畴论的数学知识基础。

若你想要学习Scala，可以：
1. 参考知乎上诸多大神对于这个语言的评价
1. 通过Spark等大相关数据处理框架入门
1. 学习作者推荐的Coursera上由EPFL开设、Scala创始人Martin Odersky教授等主讲的[Functional Programming in Scala](https://www.coursera.org/specializations/scala)专辑
1. 购买Scala相关书籍