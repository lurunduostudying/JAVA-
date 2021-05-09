1、**什么是面向对象，对它的理解。**

**面向对象**：注重事情有哪些参与者（对象）、及各自需要做什么（复用、扩展、维护）
**封装**：明确标识出允许外部使用的所有成员函数和数据项，内部细节对外部调用透明，外部调用无需修改或者关心内部实现。

​       1） javabean：私有，提供get、set对外访问，因为属性的赋值或者获取逻辑只能由javabean本身决定。而不能由外部胡乱修改。

​       2）orm框架：引入mybatis，调用方法即可。

**继承**：继承基类的方法，并做出自己的改变或修改。（子类共性的方法或者属性直接使用父类的，只扩展自己个性化的）
**多态**：基于对象所属类的不同，外部对同一个方法的调用，实际执行的逻辑不同。

继承，方法重写，父类引用指向子类对象。    无法调用子类特有的功能

**面向过程**：注重事情的每一个步骤及顺序（高效）

2、**JDK、JRE、JVM三者区别与联系**

**JDK**：java开发工具（jre、java工具（javac、java、jconsole））

**JRE**：java运行时环境（bin（jvm）  lib（类库））

**JVM**：java虚拟机（将class文件翻译成机器码）

![img](file:///C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\3NYQ]C7Q}3HNOLG~_L}F01J.png)

3、**==和equals**

**==**：对比的是**栈**中的值，基本数据类型是变量值，引用类型是**堆**中内存对象的地址。

**equals**：object中默认也是采用==比较，通常会**重写**（比较两个字符串的值）。

![img](file:///C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\HQK{3_{]IHU@W5WGMV]BE3P.png)

4、**简述final作用，为什么局部内部类和匿名内部类只能访问局部final变量？**

![5.3 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (1).png)

![5.3 (3)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (3).png)

![5.3 (2)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (2).png)

![5.3 (4)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (4).png)

![5.3 (5)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (5).png)

![5.3](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3.png)

**5、****String、StringBuffer、StringBuilder区别和使用场景**

![5.3 (6)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (6).png)

**6、重载和重写的区别**

**重载**：发生在同一个类中，方法名必须相同，方法名必须相同，参数类型不同、个数不同、顺序不同，方法返回值和访问修饰符可以不同，发生在编译时。

**重写**：发生在父子类中，方法名、参数列表必须相同，返回值范围小于等于父类，抛出的异常范围小于等于父类，访问修饰符范围大于等于父类；如果父类方法访问修饰符为private则子类就不能重写该方法。

**7、接口和抽象类的区别**

![5.3 (7)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (7).png)

![5.3 (10)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (10).png)

![5.3 (9)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (9).png)

![5.3 (8)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (8).png)

**8、List和Set的区别**

 List：有序，按对象进入的顺序保存对象，可重复，允许多个Null元素对象，可以使用Iterator取出所有元素，在逐一遍历，还可以使用get(int index)获取指定下标的元素。

Set：无序，不可重复，最多允许有一个Null元素对象，取元素时只能用Iterator接口取得所有元素，再逐一遍历各个元素。

**9、hashCode和equals**

![5.3 (11)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (11).png)

![5.3 (12)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (12).png)

**10、ArrayList和LinkedList区别**

![5.3 (13)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (13).png)

**11、HashMap和HashTable的区别，底层实现是什么？**

![5.3 (14)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (14).png)

**12、ConcurrentHashMap原理，jdk7和jdk8的区别**

![5.3 (15)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (15).png)

![5.3 (16)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (16).png)

**13、如何实现一个IOC容器**

![5.3 (17)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (17).png)

**14、什么是字节码？采用字节码的好处是什么？**

![5.3 (18)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (18).png)

**15、JAVA类加载器有哪些？**

![5.3 (19)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (19).png)

**16、双亲委派模型**

![5.3 (20)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (20).png)

![5.3 (21)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (21).png)

**17、JAVA中的异常体系**

![5.3 (22)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (22).png)

**18、GC如何判断对象可以被回收**

![5.3 (23)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (23).png)

**19、线程的生命周期，线程有哪些状态？**

![5.3 (24)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (24).png)

![5.3 (25)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (25).png)

**20、sleep()、wait()、join()、yield()的区别**

![5.3 (29)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (29).png)

![5.3 (28)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (28).png)

![5.3 (27)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (27).png)

![5.3 (26)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (26).png)

**21、对线程安全的理解**

![5.3 (31)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (31).png)

![5.3 (30)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (30).png)

**22、Thread、Runable的区别**

![5.3 (33)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (33).png)

![5.3 (32)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (32).png)

![5.3 (34)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (34).png)

MyThread创建了两个实例，自然会卖出两倍，属于用法错误。

**23、说说你对守护线程的理解**

![5.3 (35)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (35).png)

**24、ThreadLocal的原理和使用场景**

![5.3 (38)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (38).png)

![5.3 (37)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (37).png)

![5.3 (36)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (36).png)

**25、ThreadLocal内存泄漏原因，如何避免**

最终导致：OOM （内存不足）

![5.3 (39)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (39).png)

![5.3 (42)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (42).png)

![5.3 (41)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (41).png)

![5.3 (40)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (40).png)

**26、并发、并行、串行的区别**

**串行**在时间上不可能发生重叠，前一个任务没搞定，下一个任务就只能等着。

**并行**在时间上是重叠的，两个任务在**同一时刻互不干扰**的同时执行。

**并发**允许两个任务彼此干扰。统一时间点、只有一个任务运行，交替执行。

**27、并发的三大特性**

**原子性**

![5.3 (44)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (44).png)

**可见性**

![5.3 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (1).jpg)

**有序性**

![5.3 (43)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.3 (43).png)

**28、为什么使用线程池，参数解释** 

![5.4](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4.png)

**29、简述线程池处理流程**

![5.4 (2)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (2).png)

![5.4 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (1).png)

**30、线程池中阻塞队列的作用？为什么是先添加列队而不是先创建最大线程？**

![5.4 (4)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (4).png)

![5.4 (3)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (3).png)

**31、线程池线程复用的原理**

![5.4 (7)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (7).png)

**32、Spring是什么？**

![5.4 (8)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (8).png)

**33、对AOP的理解**

![5.4 (9)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (9).png)

**34、对IOC的理解**

![5.4 (10)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (10).png)

![5.4 (11)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (11).png)

**35、BeanFactory和Application有什么区别**

![5.4 (13)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (13).png)

![5.4 (12)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (12).png)

**36、简述spring bean的生命周期**

![5.4 (14)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (14).png)

**37、spring支持的bean作用域**

![5.4 (15)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (15).png)

**38、Spring框架中的单例Bean是线程安全的么**

![5.4 (16)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (16).png)

**39、spring框架中使用了哪些设计模式及应用场景**

![5.4 (17)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (17).png)

![5.4 (24)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (24).png)

![5.4 (23)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (23).png)

![5.4 (22)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (22).png)

![5.4 (21)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (21).png)

![5.4 (20)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (20).png)

![5.4 (19)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (19).png)

![5.4 (18)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (18).png)

**40、spring事务的实现方式原理以及隔离级别**

![5.4 (25)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (25).png)

![5.4 (27)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (27).png)

![5.4 (26)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.4 (26).png)

**41、spring的事务传播机制**

 ![5.5](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5.png)

**42、spring事务什么时候会失效**

![5.5 (2)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (2).png)

**43、什么是bean的自动装配，有哪些方式**

 ![5.5 (3)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (3).png)

![5.5 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (1).png)

![5.5 (5)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (5).png)

![5.5 (4)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (4).png)

**44、spring、springmvc、springboot的区别**

![5.5 (6)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (6).png)

**45、springmvc工作流程**

1）用户发送请求至前端控制器**DispatcherServlet**

2）DispatcherSerlet收到请求调用HandleMapping处理器映射器（接口，维护url到handle（处理器）的映射）

![5.5 (7)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (7).png)

**46、springmvc的主要组件（九个，核心两个）**

![5.5 (8)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (8).png)

**47、springboot自动配置原理**

![5.5 (9)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (9).png)

**48、如何理解springboot的starter机制**

![5.5 (10)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (10).png)

**49、什么是嵌入式服务器，为什么使用嵌入式服务器**

![5.5 (11)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (11).png)

![5.5 (12)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (12).png)

**50、mybatis的优缺点**

![5.5 (13)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (13).png)

**51、mybatis和hibernate的对比**

mybatis：是一个支持普通 SQL 查询，存储过程和高级映射的基于 Java 的优秀持久层框架。

框架：一套规范。既然是规范，你使用这个框架就要遵守这个框架所规定的约束。在Java开发中，框架是用一套规则加上一群jar包来表示的。

1、框架就是你在实际开发中，可以让使用者减少很多重复的代码、让代码的结构更加清晰，耦合度更低，后期维护方便。

1） 在javaSE中你可以使用JDBC实现数据库的操作，在不使用框架的情况下，sql语句都是写在java代码中的。而使用框架的情况下，sql语句可以写在配置文件中，甚至可以通过一些组件进行自动生成。

2）同时，在实现了servlet、jsp这个前端展示的时候，请求地址都是写在web.xml这个配置文件中的，比较繁琐，在使用springmvc框架时，定义一个url相对简单，只需要你配置一个注解。

2、java现在流行的框架有Spring、struts2、hibnate，springmvc等技术。

Hibernate：ORM框架：对象关系映射

 Mybatis：SQL使用框架

 ![5.5 (17)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (17).png)

![5.5 (16)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (16).png)

![5.5 (15)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (15).png)

![5.5 (14)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (14).png)

![5.5 (18)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (18).png)

**52、#{}和${}的区别**

![5.5 (19)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (19).png)

**53、简述mybatis插件运行原理及如何编写一个插件**

mubatis插件：拦截器

![5.5 (20)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (20).png)

![5.5 (21)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (21).png)

**54、索引的基本原理**

![5.5 (22)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (22).png)

### **55、mysql聚簇和非聚簇索引的区别**

![5.5 (24)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (24).png)

![5.5](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5.png)

![5.5 (23)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (23).png)

### **56、mysql索引结构，各自的优劣**

B+树：

Hash索引：

![5.5 (26)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (26).png)

![5.5 (25)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (25).png)

![5.5 (29)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (29).png)

![5.5 (28)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (28).png)

### **57、索引的设计原理**

索引是帮助数据库高效获取数据的数据结构。索引的实现通常使用B树及其变种B+树。 为表设置索引要付出代价的：一是增加了数据库的存储空间，二是在插入和修改数据时要花费较多的时间(因为索引也要随之变动)。

![5.5 (25)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (25).png)

### **58、mysql锁的类型有哪些**

![5.5 (38)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (38).png)

![5.5 (40)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (40).png)

![5.5 (30)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (30).png)

![5.5 (31)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (31).png)

![5.5 (32)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (32).png)

![5.5 (33)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (33).png)

![5.5 (34)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (34).png)

![5.5 (35)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (35).png)

![5.5 (36)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (36).png)

![5.5 (37)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.5 (37).png)

### **59、mysql执行计划怎么看**

![5.6 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (1).png)

![5.6](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6.png)

![5.6 (2)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (2).png)

### **60、事务的基本特性和隔离级别**

**事务**：是数据库操作的最小工作单元，是作为单个逻辑工作单元执行的一系列操作；这些操作作为一个整体一起向系统提交，要么都执行、要么都不执行；事务是一组不可再分割的操作集合（工作逻辑单元）；

![5.6 (5)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (5).png)

![5.6](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6.png)

![5.6 (3)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (3).png)

![5.6 (4)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (4).png)

**61、怎么处理慢查询**

![5.6 (6)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (6).png)

### **62、ACID靠什么保证的**

**A原子性**由undo log日志保证，它记录了需要回滚的日志信息，事务回滚时撤销已经执行成功的sql。

**C一致性**由其他三大特性保证、程序代码要保证业务上的一致性

**I隔离性**由**MVCC**来保证

**D持久性**由内存+redo log来保证，mysql修改数据同时在内存和redo log记录这次操作，宕机的时候可以从redo log恢复

`InnoDB redo log 写盘，InnoDB 事务进入 prepare 状态。` 

`如果前面 prepare 成功，binlog 写盘，再继续将事务日志持久化到 binlog，如果持久化成功，那么 InnoDB 事务则进入 commit 状态(在 redo log 里面写一个commit 记录)`

redolog的刷盘会在系统空闲时进行。

### **63、什么是MVCC**

**多版本并发控制**：读取数据时通过一种类似快照的方式将数据保存下来，这样读锁就和写锁不冲突了，不同的事务session会看到自己特定版本的数据，版本链MVCC只在**READ COMMITTED** 和 **REPEATABLE READ** 两个隔离级别下工作。其他两个隔离级别够和MVCC不兼容, 因为 READ UNCOMMITTED 总是读取最新的数据行, 而不是符合当前事务版本的数据行。而 SERIALIZABLE 则会对所有读取的行都加锁。

聚簇索引记录中有两个必要的隐藏列：

**trx_id**：用来存储每次对某条聚簇索引记录进行修改的时候的事务id。

**roll_pointer**：每次对哪条聚簇索引记录有修改的时候，都会把老版本写入undo日志中。这个**roll_pointer**就是存了一个指针，它指向这条聚簇索引记录的上一个版本的位置，通过它来获得上一个版本的记录信息。(注意插入操作的undo日志没有这个属性，因为它没有老版本)

**已提交读和可重复读的区别就在于它们生成ReadView的策略不同**。

![5.6 (7)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (7).png)

![5.6 (8)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (8).png)

### **64、mysql主从同步原理**

![5.6 (9)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (9).png)

![5.6](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6.png)

![5.6 (10)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (10).png)

### **65、简述Myisam（写）和Innodb（查询）的区别**

![5.6 (11)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (11).png)

![5.6 (12)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.6 (12).png)

### **66、简述mysql中索引类型及对数据库的性能的影响**

![5.8 (10)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (10).png)

### **67、RDB和AOF机制**

redis（内存数据库）：持久化实现

 ![5.8 (13)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (13).png)

![5.8 (12)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (12).png)

![5.8 (11)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (11).png)

### **68、Redis的过期键的删除策略**

![5.8 (14)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (14).png)

### **69、Redis线程模型，单线程为什么快**

redis单线程（请求处理时间快，请求数量多），java多线程（业务逻辑复杂。处理时间长）

![5.8 (15)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (15).png)

### **70、缓存雪崩、缓存穿透、缓存击穿**

![5.8 (16)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (16).png)

![5.8 (18)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (18).png)

![5.8 (17)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (17).png)

### **71、简述redis事务实现**

![5.8 (21)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (21).png)

![5.8 (19)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (19).png)

![5.8 (20)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.8 (20).png)

### **72、redis集群方案**

![5.9 (1)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (1).png)

![5.9 (4)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (4).png)

![5.9 (3)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (3).png)

![5.9 (2)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (2).png)

### **73、redis主从复制的核心原理**

![5.9 (5)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (5).png)

![5.9 (6)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (6).png)

### **74、CAP理论、BASE理论**

![5.9 (7)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (7).png)

![5.9 (8)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (8).png)

### **75、负载均衡算法、类型**

![5.9 (9)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (9).png)

![5.9 (11)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (11).png)

![5.9 (10)](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9 (10).png)

### **76、分布式框架下，Session共享有什么方案**

Session存在本地服务器内存中，http是有状态的。cookie客户端保存请求状态。

登录态。

![5.9](C:\Users\lurunduo\Documents\Tencent Files\1074817603\Image\C2C\5.9.png)

### **77、简述你对RPC、RMI的理解**

### **78、分布式id生成方案**

### **79、分布式锁解决方案**

### **80、分布式事务解决方案**

















