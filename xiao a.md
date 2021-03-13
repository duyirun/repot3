# Java基础语法：#

#目录#

一.标识符和关键字 
   1.1标识符
   1.2关键字

二：常量和变量
   2.1常量
   2.2变量
   2.2.1局部变量和全局变量
   

三：运算符
   3.1逻辑运算符
   3.2赋值运算符
   3.2字符串连接运算符
   3.3自增,自减运算符
   3.4三目运算符
   3.5关系运算符

四：流程控制
   4.1条件、选择语句
   4.1.1 if
   4.1.2switch...case.....default
   4.2 循环语句
   4.2.1 for 循环
   4.2.2 while 循环，do while 循环;
   4.2.3 continue语句 ,break语句

五.注释和分隔符


#标识符和关键字
#1.1标识符
变量名或者函数名的命名要遵守“第一个单词以小写字母开始，从第二个单词开始以后的每个单词的首字母都要用大写字母”的规则。

eg:javaIsFunny;


#1.2关键字

1.权限修饰符关键字：public,protected,private;

2:流程关键字：if，else,switch,case,default,while,do,for,break;continue,return;

3.定义类，方法，函数的关键字：abstract,final,static;

4.类与类之间的关键字：extends;

5:接口与类之间的关系：implements;

6.新建对象关键字：new;

7.引用关键字：this,super;

#常量和变量#
#2.1常量#
常量即为表示值不可变的量；
根据数据类型的不同可分为不同类型的常量

eg:整型常量如666，实型常量6.66，字符常量’6‘，逻辑常量true false,字符串常量“666”；

#2.2变量#
变量由变量的名字和变量的值组成，是程序中最基础的存储单元。

#2.2.1局部变量和全局变量#
局部变量：方法或者语句块内部定义的变量；

全局变量：方法外部，类的内部定义的变量；

#运算符#
#3.1逻辑运算符#
！--逻辑非

&&--逻辑与

||--逻辑或

#3.2赋值运算符
+=     -=      *=     / =      %=      =

#3.3自增,自减运算符
++i  先运算再取值
       
--i  先运算再取值

i++  先取值再运算

i--  先取值再运算

#3.4三目运算符
a>b?true:false

如果a>b为真，则这个式子取值为true；如果a>b为假，则这个式子取值为false;

#3.5关系运算符

#四；流程控制
 4.1条件、选择语句
   4.1.1 if

   4.1.2switch...case.....default

   4.2 循环语句

   4.2.1 for 循环

   4.2.2 while 循环，do while 循环

   4.2.3 continue语句 ,break语句

#五.注释和分隔符
  单行注释 // 注释内容 

 多行注释 /* 注释内容 */

 文档注释 /** 注释内容 */

分号（;）：语句的分割，表示一句话结束

花括号（{}）：表示一个代码块

方括号（[]）：定义数组和访问数组元素时使用

圆点（.）：类和对象访问它的成员以及方法时使用。

#八大数据类型：
int 

byte

short

long

float

double

char

boolean













#面向对象
概念：面向对象，关注点是对象的属性和方法，而忽略事物执行的顺序或过程。

面向对象的基本特征：

1：封装

优点：安全性，复用性，简单化(仅调用方法就可以实现功能，代码维护变得简单

2：继承(extends)

使用场景：多个类中存在相同的属性和行为时，可以将这些内容提取出来放到一个新类中，让这些类与新类产生父子关系，实现代码复用；

子类继承父类之后有什么效果:子类拥有了父类的非私有成员（成员变量,成员方法）

3：多态
实现多态的步骤：
.要有继承（或者实现）关系；要有方法重写；父类引用指向子类对象；



#集合
#List
特点：有序可重复
两个常用的实现类：

ArrayList

LinkedList




#ArrayList 
概念：是java集合框架中使用最多的一个类，是一个数组对列集合

特点：动态扩容，有序集合(插入的顺序==输出的顺序)，里面元素可重复，查找的效率高，增删效率低；

#ArrayList 常用方法：
boolean   add(E e) 将e尾插到线性表中

void add(int index,E e)
 将e插入到index所在位置，index之后的所有元素，“逻辑”向后移动

E  remove(int index) 删除index位置的元素，后续元素左移，返回从列表中删除的元素

boolean remove(Object  o) 删除集合中指定元素

int   size() 元素个数

E  get(int   index) 返回index位置的元素

E   set(int  index ,E  e) 用 e 替换index 位置的元素

void  clear()  清空线性表

boolean   isEmpty() 判断线性表是否为空

boolean  contains(Object o) 判断o是否在线性表中

Object[] toArray();把集合变成数组；


#Linkedlist
既可以看作一个顺序容器，又可以看作一个队列

特点：增删效率高，查找效率低；

#Linkedlist常用方法
public void addFirst(E):将指定的元素插入此列表的开头；

public void addLast(E):将指定的元素插入此列表的结尾；

public  void push(E):将元素推入此列表所表示的堆栈；


public E getFirst():返回此列表的第一个元素；

public E Getlast():返回此列表的第最后一个元素

public E removeFirst():移除并且返回此列表的第一个元素；

public E removeLast():移除并且返回此列表的最后一个元素；

public boolean isEmpty():此列表是否为空；






#Set
特点：无序而且不重复(不重复的功能需要依赖 hashCode 与 equals 方法的重写）
常用实现类：

HashSet(不是按照存储顺序保存的，具有不确定性)

TreeSet(按照自然顺序保存)

LinkedHashSet(按照用户储存的顺序储存)

Set常用方法
和List 一致(见上文）

#Map
特点：无序、以键值对的形式添加元素，键不能重复，值可以重复

常用实现类
HashMap

LinkedMap

#常用方法
Object put(Object key,Object value) : 向map中添加键值对 

void clear(): 清空

int size() : 集合中元素的个数

boolean isEmpty() : 判断集合是否为空

Object get(Object key): 根据key获取value

Collection values() : 获取map中的所有value值,以集合形式返回

booelan containsKey(Object key) : 判断是否包含某个key

booelan containsValue(Object value) : 判断是否包含某个value

Set keySet(): 获取map中的所有key,以Set集合形式返回

Set entrySet(): 返回map中的键值对映射(key=value),以Set集合形式返回

V remove(Object key) : 根据key删除指定映射关系,返回value值

#Queue
概念；queue翻译为队列，是一个先进先出的容器

常用方法：
获取并且移除：

poll() 　　获取并移除此队列的头，如果此队列为空，则返回 null

remove()　　获取并移除此队列的头，如果此队列为空，则抛出NoSuchElementException异常

获取但是不移除：

peek()　　获取队列的头但不移除此队列的头。如果此队列为空，则返回 null

添加元素：

offer()　向有界队列中添加元素的时候，如果元素的数量超过临界值，会添加失败，但不会抛出异常

add()　　向有界队列中添加元素的时候，如果元素的数量超过临界值，会抛出异常

判断对列是否为空：

isEmpty()    判断一个队列中是否为空


#Collections工具类
常用方法：

Sort（element）：对当前集合进行升序排序

max(element)：取当前集合的最大值；

Reverse（element）：逆序排序，对当前集合的元素按照相反的顺序进行排序;

.Shuffle（element）：将当前集合内的数据进行随机排序



#泛型
概念：让数据类型变得参数化,类似于方法的参数。

特点：泛型方法被调用时，会指定具体类型，确保数据的准确性，同时泛型不接受继承关系；


#异常处理
异常主要有两类：Error(错误是不可查，不应该试图去处理它所引起的异常状况）和Exception(是程序本身可以处理的异常，可以被处理）

1. 通过try...catch语句块来处理：

手动处理：

try{
  // 程序代码
}catch(异常类型1 异常的变量名1){
  // 程序代码
}catch(异常类型2 异常的变量名2){
  // 程序代码
}finally{
  // 程序代码
}

抛出：

通过throws/throw到上层进行处理


#多线程







#IO流
概念：输入流：读数据；输出流：写数据

按数据不同分类：

字节流：二进制，可以处理一切文件，包括：纯文本、doc、音频、视频等

字符流：文本文件，只能处理纯文本

字节流：

Inputstream:字节输入流的顶层抽象类

FileInputStream：普通的字节输入流

BufferedInputStream：字节缓冲输入流

OutPutStream:字节输出流的顶层抽象类

FileInputStream：普通的字节输出流

BufferedInputStream：字节缓冲输出流


字符流：
Reader:字符输入流的顶层抽象类

FileReader:普通的字符输入流

BufferedReader:字符缓冲输入流

Writer:字符输出流的顶层抽象类

FileWriter:普通的字符输出流

BufferedWriter:字符缓冲输出流





























