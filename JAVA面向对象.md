**1、java语言发展史**

计算机语言：人与计算机之间进行信息交流沟通的一种特殊语言

java之父：詹姆斯。高斯林

**2、java语言跨平台原理**

jvm：java虚拟机实现跨平台

**3、jre和jdk**

jre：java runtime environment  

java程序的运行时环境，包含JVM和运行时所需要的核心类库。

jdk：java development kit 

java程序开发工具包，包含JRE和开发人员使用的工具

开发工具包含：javac.exe（编译工具），java.exe（运行工具）

![5.6 (13)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (13).png)

**4、jdk的下载和安装**

针对不同操作系统，下载对应JDK，目前已出到版本16

![5.6 (14)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (14).png)

**6、常用DOS命令**

win+R 打开运行窗口

![5.6 (15)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (15).png)

**7、Path环境变量的配置**

为了方便使用javac和java命令

**8、java程序开发运行流程**

编写程序（Java源程序），编译程序（编译器编译成java字节码文件），运行程序

编译：javac helloworld.java java文件名

执行：java helloworld 类名

**9、常见BUG**

非法字符报错：中英文符号问题

单词拼写（大小写）问题

## **基础语法**

**10、注释**

单行//、多行/**/、文档注释 

**11、关键字**

关键字的字母全部小写，有特殊颜色标记

**12、常量**

在程序运行过程中，其值不可以发生改变的值

final修饰为常量

![5.8](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8.png)

**13、数据类型**

![5.8 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (1).png)

![5.8 (6)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (6).png)

![5.8 (5)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (5).png)

![5.8 (4)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (4).png)

![5.8 (3)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (3).png)

**14、变量**

程序运行过程中，其值可以发生改变的值。

从本质上说，变量是内存中一小块区域。

变量名+数据类型+变量值 int a=10

变量的使用：取值和修改值

**15、变量使用的注意事项**

变量名不能重复；

定义变量要给值；

long l = 100000000L；不加L会被默认为int型；

float f = 13.14F；浮点数默认double，表示float类型要加F；

**16、标识符**

**标识符（变量、方法、类）定义规则**：

由数字、字母、下划线_和美元符$组成

不能以数字开头；

不能是关键字；

区别大小写；

![5.8](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8.png)

**17、类型转换**

自动类型转换：把一个表示数据范围小的数值或变量赋值给另一个表示数据范围大的变量。

强制类型转换：把一个表示数据范围大的数值或变量赋值给另一个表示数据范围小的变量。

格式：目标数据类型 变量名=（目标数据类型）值或变量

范例：int k =(int)88.88

![5.8 (7)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (7).png)

**18、算术运算符**

![5.8 (8)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (8).png)

**19、字符的+操作**

![5.8 (9)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (9).png)

**20、字符串的+操作**

字符串拼接字符，+从左到右执行