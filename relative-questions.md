# 相关题目
## 入门Java
javac把Java程序编译成什么？

完成一个把布尔类型转换为整型的函数，尽量简洁高效。
```java
int booleanToInt(boolean b) {
    // TODO
}
```

以下代码中除main函数里面的外哪个是类、对象、局部变量、成员变量、类变量/静态变量？这几个变量分别初始化了多少次？
```java
public class C {
    public static final boolean constant = true;
    private int member;

    public C(int member) {
        this.member = member;
    }

    public void fun() {
        int memberTimes2 = member * 2;
        System.out.println(memberTimes2);
    }

    public static void main(String[] args) {
        C[] cArray = new C[10];
        for (int i = 0; i < 10; i++) 
            cArray[i] = new C(i);
        for (int i = 0; i < 20; i++)
            cArray[i % 10].fun();
    }
}
```

Python的int类型对应Java的什么类型？

&&与&的区别是什么？

以下说法是否正确？  
“因为类里面的成员方法是一个对象的方法，所以每多一个这个类的对象，就需要为这个方法分配新的内存。”

以下描述分别对应着哪种Throwable？（原句中出现的用“它”替换）
1. 最具代表的“它”是用户错误或问题引起的异常，这是程序员无法预见的。例如要打开一个不存在文件时，一个异常就发生了，这些异常在编译时不能被简单地忽略。
1. “它”是可能被程序员避免的异常。与“第一条异常”相反，“它”可以在编译时被忽略。
1. “它”不是异常，而是脱离程序员控制的问题。“它”在代码中通常被忽略。例如，当栈溢出时，一个“它”就发生了，它们在编译也检查不到的。

用“父类（子类，子类（子类的子类，子类的子类，……），……）”这种形式写出Throwable、Exception、RuntimeException、IOException、Error的继承关系。

Java是否允许多继承（一个子类继承多个父类）？

重载和重写体现了面向对象编程的什么特征？

以下以Main.main函数为入口的代码会输出什么结果？
```java
public class Person {
    public void introduce() {
        System.out.println("I am a person.");
    }
}
```
```java
public class Man extends Person {
    @Override
    public void introduce() {
        System.out.println("I am a man.");
    }
}
```
```java
public class Main {
    public static void main(String[] args) {
        Person p = new Man();
        p.introduce();
    }
}
```

填空：Java中的普通函数就相当于C++的\_\_\_\_函数，动态绑定是Java的默认行为。如果Java中不希望某个函数具有此特性，可以加上\_\_\_\_关键字变成非虚函数。

写一个标准的数据类/POJO类/JavaBean，名字为C，只含有一个类型为T的成员变量f，有getter和setter。

抽象类和接口：
1. 哪一个可以写构造方法？
1. 哪一个没有成员变量？
1. 哪一个的抽象方法可以省略abstract关键字并且默认是public的？
1. 怎么用匿名内部类的方式实例化？

用“父类（子类，子类（子类的子类，子类的子类，……），……）”这种形式写出Iterable、Collection、List、Set、Map、ArrayList、LinkedList、HashSet、TreeSet、HashMap、TreeMap、AbstractList、AbstractSet、AbstractMap的继承关系，若是抽象类在后面加a，若是接口在后面加i。

下面代码是否能通过编译？如果不行，分别使用强制类型转换和泛型的方式修改它让它通过编译。
```java
ArrayList ss = new ArrayList();
ss.add("s");
String s = ss.get(0);
```

使用Lambda表达式和方法引用的方式改写以下代码（ss类型为`List<String>`）：
```java
Collections.sort(ss, new Comparator<String>() {
    @Override
    public int compare(String s1, String s2) {
        return s1.compareTo(s2);
    }
});
```

思考题：`List<Integer>`是否是`List<Number>`的子类型？为什么？换言之：泛型参数为子类型的类型是否是泛型参数为父类型的类型的子类型？

## 入门Kotlin
修改下面代码中的错误：
```kotiln
fun printDouble(d: Double) { print(d) }
val i = 1
printDouble(i)
```

完成以下代码将 `Char` 转换位它所表示的 `Int`：
```kotlin
fun decimalDigitValue(c: Char): Int {
    if (c !in '0'..'9')
        throw IllegalArgumentException("Out of range")
    return TODO()
}
```

请完成以下代码输出 `i` 和 `s.length` 的值：
```kotlin
val i = 10
println(TODO()) // 输出“i = 10”
```
```kotlin
val s = "abc"
println(TODO()) // 输出“abc.length is 3”
```

填空：在导入时，如果出现名字冲突，可以使用\_\_\_\_关键字在本地重命名冲突项来消歧义？

填空：在 Kotlin 中，if 是一个\_\_\_\_，即它会返回一个值。 因此就不需要\_\_\_\_，因为普通的 if 就能胜任这个角色。

填空：\_\_\_\_表达式取代了类 C 语言的 switch 语句。

写代码遍历并输出一个元素集合 `collection` 的所有元素。

填空：在 Kotlin 中任何表达式都可以用标签（label）来标记，标签的格式为标识符后跟\_\_\_\_符号。

填空：在 Kotlin 中的一个类可以有一个\_\_\_\_构造函数以及一个或多个\_\_\_\_构造函数。

填空：初始化的代码可以放到以\_\_\_\_关键字作为前缀的初始化块（initializer blocks）中。

填空：类也可以声明前缀有\_\_\_\_的次构造函数

填空：在 Kotlin 中所有类都有一个共同的超类\_\_\_\_。

填空：默认情况下，Kotlin 类（和其中的函数）是\_\_\_\_的：它们不能被继承。要使一个类可继承，请用\_\_\_\_关键字标记它。

填空：Kotlin 类中的属性既可以用关键字\_\_\_\_声明为可变的，也可以用关键字\_\_\_\_声明为只读的。

将下列 Java 代码翻译成最简洁的 Kotlin 代码：
```java
public class Person {
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}
```

（暂无自定义 getter 与 setter、`lateinit` 知识点相关题目。）

填空：如果只读属性的值在编译期是已知的，那么可以使用\_\_\_\_修饰符将其标记为编译期常量。

Kotlin 的接口可以既包含抽象方法的声明，是否也可以包含实现？

填空：可以用\_\_\_\_修饰符在 Kotlin 中声明一个函数式接口。

填空：  
函数、属性和类、对象和接口可以在顶层声明，即直接在包内：
* 如果你不指定任何可见性修饰符，默认为\_\_\_\_，这意味着你的声明将随处可见；
* 如果你声明为\_\_\_\_，它只会在声明它的文件内可见；
* 如果你声明为\_\_\_\_，它会在相同模块内随处可见；
* \_\_\_\_不适用于顶层声明。

对于类内部声明的成员：
* \_\_\_\_意味着只在这个类内部（包含其所有成员）可见；
* \_\_\_\_—— 和以上一样 + 在子类中可见。

写出代码为 `MutableList<Int>` 添加一个 `swap` 拓展函数，交换位于 `index1` 和 `index2` 处的元素。

扩展是\_\_\_\_解析的。