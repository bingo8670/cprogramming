https://www.runoob.com/cprogramming/c-tutorial.html
学习笔记

编译 & 执行 C 程序
接下来让我们看看如何把源代码保存在一个文件中，以及如何编译并运行它。下面是简单的步骤：

打开一个文本编辑器，添加上述代码。
保存文件为 hello.c。
打开命令提示符，进入到保存文件所在的目录。
键入 gcc hello.c，输入回车，编译代码。
如果代码中没有错误，命令提示符会跳到下一行，并生成 a.out 可执行文件。
现在，键入 a.out 来执行程序。
您可以看到屏幕上显示 "Hello World"。
$ gcc hello.c
$ ./a.out
Hello, World!
请确保您的路径中已包含 gcc 编译器，并确保在包含源文件 hello.c 的目录中运行它。

如果是多个 c 代码的源码文件，编译方法如下：

$ gcc test1.c test2.c -o main.out
$ ./main.out

整数常量可以是十进制、八进制或十六进制的常量。前缀指定基数：0x 或 0X 表示十六进制，0 表示八进制，不带前缀则默认表示十进制。

整数常量也可以带一个后缀，后缀是 U 和 L 的组合，U 表示无符号整数（unsigned），L 表示长整数（long）。后缀可以是大写，也可以是小写，U 和 L 的顺序任意。

使用 #define 预处理器定义常量的形式：
#define identifier value

使用 const 前缀声明指定类型的常量，如下所示：
const type variable = value;
