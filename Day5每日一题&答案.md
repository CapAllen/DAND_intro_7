# 每日一题&答案 - Day5

1. 现在有一个文本字符串是s='string'，请问s.split('i')返回的结果是什么？s.split('i')[0]呢？

  s.split('i')返回的结果是['str', 'ng']; s.split('i')[0]返回的结果是str ; 语法：
  str.split(str="",num=string.count(str))[n] 参数说明：str表示为分隔符，默认为空格，但是
  不能为空('')。若字符串中没有分隔符，则把整个字符串作为列表的一个元素;num表示分割
  次数。如果存在参数num，则仅分隔成 num+1 个子字符串，并且每一个子字符串可以赋
  给新的变量;[n]表示选取第n个分片

2. print 'hello\n'，这个语句显示的结果中\n有没有显示出来？\n是普通的文本吗？

  \n没有显示，它表示换行 不是普通文本 ，\是转义

3. 集合里面的元素是唯一的吗？

  集合里面的元素是唯一的

4. 假如你不知道pandas如何去除一列里面的重复值，你会如何在谷歌搜索这个方法？(用英
  文)

  python pandas remove duplicate value in column

5. dewp=20 print 'The missing number of DEWP is %d'%20。显示的结果是什么？如何用
  format和{}实现相同的显示结果？

  显示的结果为 The missing number of DEWP is 20;等价写法: print("The missing number
  od DEWP is {}".format(20))

6. python的模块是什么后缀名的文件？我们是否也可以自己写一个模块并导入？

  .py模块可以自己编写并导入。

7. 现在有个字典phonebook = {"John" : 938477566,"Jack" : 938377264,"Jill" : 947662781}
  ，我想依次打印出每个键和对应的值，怎么写？（提示：iteritems()）

  ```python
  for key in phonebook: 
      print(key, phonebook[key])
  
  ```

8. 如何用lambda写一个将输入值x转化成x的平方的函数（了解lambda定义函数的基本语
  句）

  square=lambda x:x**2

9. python 中的控制流是什么意思

   控制流是控制代码执行顺序的语句。 Python用于流程控制的语句包括if条件语句、for和
   while循环语句、break和continue语句、列表推导（list comprehension）。

10. python 中的代码如果要在中途换行怎么办
    在行末加\

11. python 中的matlibplot库是干什么的

    用来对数据可视化的

12. 如何判断一个元素是否在列表当中？

    用 in 和 not in语句来判断

13. 概率的互斥事件是什么意思？

    事件A和B的交集为空，A与B就是互斥事件，也叫互不相容事件。即不可能同时发生的事
    件。

14. 如何查看列表中的惟一值的个数

    Set 集合里的元素都是唯一的，用 list 创建一个set，set里面的值就是 list 里的唯一元素
    值。然后用 len() 计算个数。例如len（set【list】）

15. 什么是python的生成器？

    python的生成器相当于是一个遍历列表的操作，只不过每次调用只输出一个值

16. 如何设置使用matplotlib库进行可视化图像的大小？

    使用figure函数，示例：设置一个8X6大小的图像

    ```python
    import matplotlib.pyplot as plt
    plt.figure(figsize=(8,6))
    ```

17. 如何给使用matplotlib库进行可视化图像添加标题？

    使用title函数，示例：

    ```python
    import matplotlib.pyplot as plt
    plt.title('This is the title.')
    ```
