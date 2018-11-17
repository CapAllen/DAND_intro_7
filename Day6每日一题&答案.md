# 每日一题&答案 - Day6

1. 你是如何理解matplotlib.pyplot库里面关于figure和axe的关系的？

  figure和axes是plt中的对象名称， figure一般理解为一个画板，对应的是一个对话框，
  axes一般翻译为“子图”，包含于figure

2. matplotlib.pyplot这个库生成的axe，如果我们要输入图表标题可以用plt.title('xxx')，那么如
  果我们要修改x轴的标签名字可以怎么写？你发现了设置的规律了吗？

  matplotlib.pyplot 是一个绘图框架 修改x轴标签名, plt.xlabel("x"), 与MATLAB plot 用法类
  似 xlabel('x')

3. numpy当中有时候设置了random.seed(42)，称为随机种子。你理解的随机种子的作用是
  什么？为什么很多时候看到的都是42？（提示：宇宙的终极答案）

  np.random.seed()的作用：使得随机数据可预测。当我们设置相同的seed，每次生成的随
  机数相同。如果不设置seed，则每次会生成不同的随机数；用'42'是作为种子是个人习惯,
  起源于一部科幻小说。

4. 你了解的jupyter notebook快捷键有哪三个？

  1). shift+ctrl+p 调出命令面板 2). Esc+F 在代码中查找内容 3). Ctrl-Enter : 运行本单元

5. python定义函数用什么语句开头。

  def function1(): 

  看到def 就知道定义了一个函数，后面是函数的名字。函数是写好的一段
  代码。需要执行的时候只用调用就行： function1（）

6. 对于正态分布，有哪几个重要的变量？

  均值和方差， 一般正态分布：均值为μ、方差为σ²

7. 常用的编辑器有哪些？

  常用的代码编辑器： atom（开源/免费/跨平台，推荐）, sublime, vim, notepad++
  python集成开发环境(IDE): PyCharm
  python包管理工具：Anaconda（win平台强烈建议使用）

8. 什么是矩阵？你能用Python的列表随便写一个简单的2*2矩阵吗？

  在数学中，矩阵（Matrix）是一个按照长方阵列排列的复数或实数集合。

  ```python
  from numpy import
  import numpy as np
  data1=mat(zeros((2,2)))
  
  print(data1)
  matrix([[ 0., 0.], [ 0., 0.]])
  ```

9. python的条件语句应该用"=="还是"="？\

  Python条件语句是使用if else来表示，变量设定初始值时是用“=”，在判断条件时用“==”给
  变量赋值。

10. 你会如何向一个门外汉介绍朴素贝叶斯的原理？

    朴素贝叶斯是一个基于贝叶斯定理的比较简单的概率分类器。举个例子，用于垃圾邮件分
    类，朴素贝叶斯分类通过选择，通常是邮件中的单词来得到垃圾邮件和非垃圾邮件间的关
    联，比如‘drug’这个词语在垃圾邮件和正常邮件中，原本出现的概率各为50%。通过贝叶
    斯法则计算可能会得到‘drug’在垃圾邮件中的概率为99%，那说明‘drug’的判断力很强，将
    50%的先验概率提高到了99％的后验概率，使得预估的概率更接近真实。但这个假设得基
    于邮件中的单词是独立的事件，实际这种条件一般不被满足，所以称为朴素贝叶斯。

11. Python 当中遍历(loop)是什么意思？

    遍历就是依次取出列表，元组，集合里面的元素做一些事

12. Python 代码里面文本注释前面要加什么符号？

    #常被用作单行注释符号，多行注释是用三引号''' '''包含。

13. markdown语法跟普通文本有哪几点区别？

    普通文本要在富文本编辑器里加样式，而markdown可以直接用特殊符号加样式，一边写
    一边排版，更流畅。另外普通文本编辑好样式不容易分享，但markdown一处书写，随处
    打开

14. 你是如何理解matplotlib.pyplot库里面关于figure和axe的关系的？

    figure和axes是plt中的对象名称， figure一般理解为一个画板，对应的是一个对话框，
    axes一般翻译为“子图”，包含于figure

15. matplotlib.pyplot这个库生成的axe，如果我们要输入图表标题可以用plt.title('xxx')，那么如
    果我们要修改x轴的标签名字可以怎么写？你发现了设置的规律了吗？

    matplotlib.pyplot 是一个绘图框架 修改x轴标签名, plt.xlabel("x"), 与MATLAB plot 用法类
    似 xlabel('x')

16.