# 从Java到Kotlin学习路线
本文是我个人总结的在已经学会C或Python的基础上的从Java到Kotlin的学习路线。在按照本文学习之前，请确保你已至少熟悉C或Python其中一门编程语言。本文会略去一些已经过时的Java知识点（如Applet、JSP），这些知识点不推荐学习但你可以自己去了解；本文不包含Java企业框架和一些传统的企业Java库的知识点（如Spring、Tomcat相关知识等），由于Kotlin有更简洁、更符合语言习惯的的替代方案，因此本文不包含这些内容，若你工作方向与这些相关且想要了解，请自行查阅相关资料。

## 入门Java
### 知识点（C和Python均涉及的基本知识点已省略）
理解入门知识：
1. 基本类型与引用类型
1. 类与对象
1. 局部变量、成员变量与成员函数、静态变量与静态函数、常量
1. 访问控制修饰符（看懂就行，不用记忆）
1. 控制语句：两种for循环、switch、三元运算符
1. 异常处理

理解面向对象编程（OOP）与其三大特征继承、多态、封装：
1. 继承：子类继承父类
1. 多态：重载、重写（用父类/接口变量存储子类/接口对象、动态派发）
1. 封装：重点理解private与protected访问控制修饰符
1. 接口与抽象类

理解进阶实战知识：
1. 常用数据结构：Iterable（Iterator）、Collection、List、Set、Map、ArrayList、LinkedList、HashSet、TreeSet、HashMap、TreeMap、AbstractList、AbstractSet、AbstractMap等（哪些是接口、抽象类、非抽象类？每一个又继承/实现了哪些类/接口？）
1. 泛型
1. Java 8的lambda表达式

上文未涉及的其他知识可以现学现用，与实战相结合更合适，不需要在没有实际项目经验和项目需求的时候提前盲目学习。

### 环境配置
安装JDK，最新LTS版本为11：https://www.oracle.com/java/technologies/javase-jdk11-downloads.html （也可通过包管理器、AdoptJDK、Lebrica JDK等方式安装，更加方便管理）  
安装IDE，推荐IntelliJ IDEA Community：https://www.jetbrains.com/idea/download/

### 推荐入门教程
1. 英文交互式APP教程：[Java Tutorial | SoloLearn: Learn to code for FREE!](https://www.sololearn.com/Course/Java/)
1. 中文教程：[Java 教程 | 菜鸟教程](https://www.runoob.com/java/java-tutorial.html)中的以上知识点相关内容
1. Coursera上杜克大学提供的Java课程：[Java Programming and Software Engineering Fundamentals | Coursera](https://www.coursera.org/specializations/java-programming)

### 进阶教程
1. 系统理解Java的每一个细节：《Java编程思想》
1. 从软件工程和编程语言理论等的角度了解Java的常用设计模式、常见错误、语言设计的利与弊等，高效编码：《Effective Java》
1. 理解JVM（Java虚拟机）并联系操作系统、编译器等知识

## 学习Kotlin
Kotlin是由开发本文推荐的著名Java IDE即IntelliJ IDEA的JetBrains公司开发的一门开源编程语言。JetBrains公司在多年使用Java语言进行开发的过程中，意识到了Java存在的诸多软件工程层面的问题与不便，于是开发出Kotlin语言致力于解决这些问题与不便。Kotlin基本可以实现Java能实现的所有功能，可以与Java相互调用、语法更加简洁、更好地支持函数式编程与DSL、并且拥有强大的跨平台性（除兼电脑端与Andoid端JVM平台外还可兼容Web端JavaScript生态、iOS生态和LLVM支持的电脑端原生生态）。Kotlin语言吸收了在它之前推出的JVM语言如Scala等的优点，同时取舍了这些语言中一些过于复杂的功能以降低其学习门槛。

官方网站：[Kotlin Programming Language](https://kotlinlang.org/)

### 知识点（Java涉及并且语法类似的知识点已省略）
以下知识点参照官方参考。

工程实战所需常用知识点：
1. 开始（重点：通过思考与Java的异同点对比记忆）
   1. 基本语法
   1. 习惯用法
   1. 编码规范
1. 基础
   1. 基本类型（重点：首字母均为大写）
   1. 包与导入（重点：`import ... as ...`写法）
   1. 控制流（重点：if表达式、when表达式、for循环）
   1. 返回与跳转（无重点）
1. 类与对象（重点：思考与Java的异同点、属性与其JVM实现、拓展函数与拓展属性、数据类、泛型与型变、类型别名）
1. 函数与Lambda表达式
1. 集合操作与函数式编程（重点：集合高阶函数）
1. 其他零散较重要特性：空安全、操作符重载、Java互操作

进阶内容知识点：
1. 协程
1. 跨平台开发
1. DSL

根据工程需要学习的知识点：
1. 服务器端开发（Ktor、Vert.x、Spring）
1. Android开发（Kotlin已经是Android开发的官方语言之一，并且在官方的推动下有取代Java的趋势，Android相关知识点本文不详述。）
1. Web端开发（JavaScript支持与kotlinx.html等）
1. 基于LLVM的原生平台开发（相比JVM版本速度较慢暂不推荐用于大型工程）
1. iOS平台开发（可与Objective-C与Swift互操作）

### 推荐教程
1. 官方参考：[Reference - Kotlin Programming Language](https://kotlinlang.org/docs/reference/)
1. 官方参考中文版翻译：[Reference - Kotlin 语言中文站](https://www.kotlincn.net/docs/reference/)
1. SoloLearn 教程：[Learn Kotlin | SoloLearn](https://www.sololearn.com/learning/1160)
1. Coursera上JetBrains公司提供的Kotlin课程：[Kotlin for Java Developers | Coursera](https://www.coursera.org/learn/kotlin-for-java-developers)

### 更多进阶内容
1. 项目编译自动化工具Gradle
1. 函数式编程与类型系统进阶：推荐学习Scala或其他函数式编程语言

## Scala与其他函数式编程语言
Scala是JVM上的以函数式编程为主的多范式语言，很好地结合了面向对象编程（代表语言：Smalltalk、Java）与函数式编程（代表语言：Lisp、Haskell）两种范式，常用于并行计算、大数据处理等。由于出自学术界，此门语言难度较大，基本入门需要一定的数据结构与算法、操作系统的计算机科学知识基础，而进阶理解需要一定的编译原理、编程语言理论、计算模型、类型系统的理论计算机科学知识基础和线性代数、抽象代数和范畴论的理论计算机科学和数学知识基础。Kotlin的语法和Scala极为相近，并且从Scala学习到了很多特性。

若你想要学习Scala，可以：
1. 参考知乎上诸多大神对于这个语言的评价
1. 通过Spark等相关大数据处理框架入门
1. 学习Coursera上由EPFL开设、Scala创始人Martin Odersky教授等主讲的[Functional Programming in Scala](https://www.coursera.org/specializations/scala)专辑
1. 购买Scala相关书籍

Scala语言结合了两大范式，但有一些研究编程语言理论与函数式编程的专家并不认同面向对象范式，因此你也可以学习以下支持不掺杂面向对象范式的函数式编程语言：
1. Haskell
1. ML系语言（如OCaml、Standard ML等）
1. Lisp系语言（如Clojure、Common Lisp、Racket、Scheme等）
