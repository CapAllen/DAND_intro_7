# 每日导学 - Day6

> Stop being afraid of what could go wrong and start being positive about what could go right.

Hi，各位同学们，今天是7天试学的倒数第二天啦，之前进度落下的同学抓紧做项目啦，今天我们学一下选修：**数据结构和循环**

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

- 列表
- For循环    
- While循环

# 知识清单

## 1.列表

列表比较简单，这里不再赘述。

## 2.for循环

- for循环可以遍历任何序列的项目，如一个列表或者一个字符串，通俗点说，就是把这个序列中的第一个元素到最后一个元素依次访问并执行冒号后面的语句

- 其一般格式为：

  ```
  for <元素> in <序列>:
      <执行语句>
  ```

## 3.while循环

- for循环和while循环，两者的相同点在于都能循环做一件重复的事情；不同点在于，for循环是在序列穷尽时停止，while循环是在条件不成立时停止。 当这个条件永远不为False时，就会出现死循环。

- 其一般格式为：

  ```
  while <判断条件>：
      <执行语句>
  ```

## 4.break和continue

- break 语句可以跳出 for 和 while 的循环体。

  示例：

  ```
  for letter in 'Udacity':     # for实例
     if letter == 't':
        break
     print ('当前字母为 :', letter)
        
  i = 10                    # while实例
  while i > 0:              
     print ('当期变量值为 :', i)
     i -= 1
     if i == 5:
        break
  ```

  执行语句后的输出结果为：

  ```
  当前字母为 : U
  当前字母为 : d
  当前字母为 : a
  当前字母为 : c
  当前字母为 : i
  当期变量值为 : 10
  当期变量值为 : 9
  当期变量值为 : 8
  当期变量值为 : 7
  当期变量值为 : 6
  ```

- continue是跳过当前循环块中的剩余语句， 也就是跳过continue后面的语句

  示例：

  ```
  for letter in 'Udacity':     # for实例
     if letter == 't':
        continue
     print ('当前字母为 :', letter)
        
  i = 5                    # while实例
  while i > 0:              
     i -= 1
     if i == 3:
        continue
      print ('当期变量值为 :', i)
  ```

  执行代码后的输出结果为：

  ```
  当前字母为 : U
  当前字母为 : d
  当前字母为 : a
  当前字母为 : c
  当前字母为 : i
  当前字母为 : y
  当期变量值为 : 4
  当期变量值为 : 2
  当期变量值为 : 1
  当期变量值为 : 0
  ```

综上呢，for更适合可迭代情况下使用，while更适合不知道要循环多少次的时候使用。

# 最后

这些内容在正式班都可以学到，大家不要急~