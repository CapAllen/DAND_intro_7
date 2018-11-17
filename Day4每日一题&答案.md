# 每日一题&答案 - Day4

1. python当中的字符串类型的"15"和整数型的15有区别吗？

  有区别。 字符串类型的15可以进行字符串相关的操作，或者字符串相关的方法； 整形的
  15可以进行数学运算，加减乘除等。

2. python的条件语句应该用"=="还是"="？

  条件语句应该是"=="表示等于，"="在Python中表示赋值。

3. python怎么显示出Hello?

  print('Hello') 因为Hello是字符串，所以要用‘’引起来，“”也是可以的。但要注意都是英文
  符号。

4. 这里提示if count=1那一行invalid syntax，‘invalid syntax’中文意思是什么？你认为哪里
  写错了？

  def if_conditions():
  count=1
  if count==1
  return 'hello'
  invalid syntax指语法错误。应写成if count==1:，加上冒号。

5. 请问在 Python 中 and 和 & 有什么区别？

  & 是 位运算 ；and 是 逻辑运算

6. while循环中break和continue是什么意思？

  continue 用于跳过该次循环，break 则是用于退出循环。

7. 列表怎么样进行排序？

   使用.sort() 方法进行排序，其中reverse = True 是降序， reverse = False 是升序（默
   认）。

8. 列表如何追加元素，比如有个列表li=[1,2,3]，我怎么往里面加个字符串'a'？

  li.append('a')

9. [i.upper() for i in ['a', 'b', 'c']] 返回的结果是什么？你如何描述中间执行的过程？

  返回的结果是：['A', 'B', 'C']。upper() 是将对象全部大写，这个语句可以理解为大写当i为
  a,b,c

10. 尝试运行下 ['a']*10 ，返回什么？

    ['a', 'a', 'a', 'a', 'a', 'a', 'a', 'a', 'a', 'a']

11. python 中的 def 是干什么用的

    def是define的意思，在python中用来定义函数。例如 定义函数：
    def hello():
    print("hello")
    #调用函数
    hello（）

12. 关于python的赋值，左边可以不加下划线写成animal lion='lion' 这样的形式吗？

    不可以。变量名只能以字母，数字，下划线构成，中间不能出现空格。

13. pandas的dataframe某一列名为'City'，我想抽取该列，写成df['city']，返回key error:city的
    报错，请说下你理解的为什么会报这个key error这个错误？

    city和City的大小写不一样，所以会报错

14. python当中的try和except语句是什么用途？

    try/except语句用来检测try语句块中的错误，从而让except语句捕获异常信息并处理。

15. 常用的逻辑判断符号有哪些？比如"=="检验两个变量是否相等，">"表示大于

    == 等于 - 比较对象是否相等

    != 不等于 - 比较两个对象是否不相等

    <> 不等于 - 比较两个对象是否不相等

    `>`大于 - 返回x是否大于y

    < 小于 - 返回x是否小于y。所有比较运算符返回1表示真，返回0表示假。这分别与特
    殊的变量True和False等价。

    = 大于等于- 返回x是否大于等于y。

    <= 小于等于 - 返回x是否小于等于y。
16. python中的enumerate函数是什么意思？

    enumerate是枚举函数，常与for连用，输入一个可迭代对象，返回该迭代对象中的元素及元素的索引。

    使用示例：

    ```python
    for inx, val in enumerate(list_a):
        print (inx)
        print (val)
    ```

    可以通过执行如上代码，理解enumerate函数的用法。

17. 将字符串中的空格替换为下划线，应该用那个函数？

    replace函数，用法：str_a.replace(' ','_')