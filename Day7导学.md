# 每日导学 - Day7

> If you don’t like where you are , change it. You’re not a tree.

Hi，各位同学们，今天是7天试学的最后一天啦，还没提交项目的同学抓紧抓紧抓紧！！！今天我们学一下选修：**函数和标准库**

**注意**：

- 请使用Chrome或者火狐浏览器。
- 选修的话，都可以在正式班课程中学习，而且曲线更平滑，如果项目通过的话可以先了解下。

**如何提问**：

在课程学习中难免会遇到问题，请按照以下流程进行问题提问：

- **课程知识问题**：

  - 先自行查找问题答案，参考：谷歌/必应搜索、[菜鸟教程](http://www.runoob.com/sql/sql-tutorial.html)、[CSDN](https://www.csdn.net/)、[stack**overflow**](https://stackoverflow.com/)
  - 若问题未解决，请将**问题**及其**所在课程章节**发送至微信群，并@助教-Allen即可

- **非课程知识问题**：

  比如账号登录、课程加载等问题，请详细描述问题，反馈给班主任即可；

  有关于后续正式课程、服务的疑问和选课建议，联系你的学习规划师就行~

# 今日目标

- 函数及定义
- 标准库的调用

# 知识清单

## 1.函数

### 定义函数

- 其一般格式为：

  ```
  def 函数名(参数):
  '''
  函数说明
  '''
  	函数语句
  ```

  - 函数说明是建议非必需
  - 函数语句最后以return(表达式)结尾，则返回值；若不带表达式，则返回None

### 参数

默认参数和关键字参数不在赘述，在此只讲述一种**不定长参数**。

- 若在参数前面加一个星号`*`，则将所有未命名的参数以元组的形式导入；
- 若在参数前面加两个星号`**`，则参数会以字典的形式导入。

示例：

```
#定义函数
def tupleprint(a, *tupleb ):
'''
打印任何传入的参数
'''
   print ("输出: ")
   print (a)
   print (tupleb)
   
#调用函数
tupleprint(1,2,3)
```

执行代码，输出结果为：

```
输出: 
1
(2, 3)
```

### 变量作用域

变量的作用域就是能访问该变量的程序部分。

- 在python中，只有模块（module），类（class）以及函数（def、lambda）才会引入新的作用域 ，而其他如if/for/while等是不会引入新的作用域的。

- 全局变量即可以在整个程序范围内都可以访问；局部变量只能在其被定义的函数内调用。

  示例：

  ```
  global_a = 0 # 这是一个全局变量
  # 定义函数
  def sum( a, b ):
      global_a = a + b # global_a在这里是局部变量.
      print ("局部变量为: ", global_a)
      return global_a
     
  #调用函数
  sum(1,2)
  print ("全局变量为: ", global_a)
  ```

  执行代码，输出结果为：

  ```
  局部变量为:  3
  全局变量为:  0
  ```

- na当局部代码想要修改全局变量时，就会用到global和nonlocal关键字了 。

  示例：

  ```
  num = 1
  def fun1():
      global num  # 需要使用 global 关键字声明
      print(num) 
      num = 123
      print(num)
  fun1()
  print(num)
  ```

  执行代码，输出结果为：

  ```
  1
  123
  123
  ```

  nonlocal的用法类似，用在嵌套函数中，当只想修改嵌套作用域的变量而非全局变量时使用。

### 可更改对象与不可更改对象

在数据类型中也提到过，python中的可变类型（列表、字典和集合）与不可变类型（数字，字符串和元组），那在函数中作为变量进行传递时会是怎样呢？

示例1：

```
#定义函数
def fun1(a):
	a = 2
	print(a)
	
b = 1
fun1(b)
print(b)
```

示例2：

```
def fun2(list_a):
	list_a.append(2)
	print(list_a)
	
list_b = [0,1]
fun2(list_b)
print(list_b)
```

尝试下，上面这两个示例的输出结果，有什么区别？

## 2.标准库调用

调用库要使用函数`import`，主要有以下几种形式，掌握就好：

```python
import pandas #调用pandas
import pandas as pd #设置别名
import matplotlib.pyplot as plt #调用库中的某一个包，并设置别名
from matplotlib import pyplot as plt #跟上一条功能一样
```

# 最后

这些内容在正式班都可以学到，大家不要急~