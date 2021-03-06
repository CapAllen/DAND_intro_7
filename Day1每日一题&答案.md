# 每日一题&答案 - Day1

> If you change nothing, nothing will change.

今天是一些针对统计学基础的题目，大家来看下答案吧~有问题及时沟通哈~

# 题目&答案

1. 什么是直方图？直方图的偏态有哪些？

     直方图是一种二维统计图表，它的两个坐标分别是统计样本和该样本对应的某个属性的度量。主要针对数值型连续变量，可以直观地观察改变量的分布情况。

     直方图有三种偏态形式：左偏态、右偏态及无偏态。一般的，均值小于中位数时为左偏态（普遍但不绝对，下同）；均值大于中位数时为右偏态；均值等于中位数时为无偏态，也就是对称分布。三种形式的示意图如下：

     ![](https://tse4.mm.bing.net/th?id=OIP.eJMf4CCd_ylkXqyGPD0NbQHaE8&pid=Api)

2. 数值变量根据取值不同可以分为哪两种？
     数值型变量根据其取值的不同，可以分为离散型变量和连续型变量。

3. 能简要描述下总体、参数、样本及统计量的概念和他们之间的关系吗？

     - **总体** —— 我们想要研究的整个群体，我们并不能获取全部的数据

     - **参数** —— 描述总体的数值摘要，可以是均值等

     - **样本** —— 总体的子集，需要我们获取全部数据

     - **统计量** —— 描述样本的数值摘要，要与参数对应，如果参数是均值，那么统计量也应该是均值。

4. 什么是定类变量?
     个体在属性上的特征或类别上的不同变量，仅仅是一种标志，没有序次关系。例如， ”性
       别“，”男“编码为1，”女“编码为2。

5. 什么是定序变量？
     用数字表示个体在某个有序状态中所处的位置，不能做四则运算。例如，“受教育程度”，
       文盲半文盲=1，小学=2，初中=3，高中=4，大学=5，硕士研究生=6，博士及其以上=7。

6. 什么是集中趋势测量？集中趋势测量包括哪几种？
     在统计学中，集中趋势（central tendency）或中央趋势，在口语上也经常被称为平均，
       表示一个机率分布的中间值。 最常见的几种集中趋势包括算数平均数、 中位数 及 众数 。

7. 我们一般会查看数值数据（也就是字段都是数字）的哪些统计学变量？比如平均值？
     平均值，最大值，最小值，中位数，众数。

8. 统计学中的‘中位数’是什么意思?
     中位数将我们的数据分为两部分，一半低于它，一半高于它。我们在课程中还学到，如何
       计算中位数取决于我们有偶数个还是奇数个观察值。

9. 可以简单描述下什么是辛普森悖论吗？我们应该怎样避免出现辛普森悖论？
     辛普森悖论是在某个条件下的两组数据，分别讨论时都会满足某种性质，可是一旦合并考虑，却可能导致相反的结论。那么如何避免辛普森悖论呢？那就要从产生它的源头——混杂因素上考虑，混杂因素就是一个与核心研究无关的变量，它会随着变量的改变而改变。所以在之后处理类似问题时就要进行多变量分析，这样才能帮助我们认清事件的本质。

10. 在进行数据分析之前，是否有必要检查我们得到的数据，怎么检查？
     非常有必要，浏览、熟悉、检查数据是分析的基础。即使分析的再好，如果原数据出现问
       题，也会影响分析结果。简单来讲，要看下数据的样本大小，分布情况（是否正态、左
       偏、右偏），是否有异常值。

11. 数据异常值通常是指哪几种情况？
      数据中的异常值种类有很多，比如人为录入错误，数据合并，单位不统一，设备错误等。
        对于数据的影响可以分为以下几类：
        ● 值异常。就是数据与实际数据不同。比如有数据输入错误，重复等等
        ● NaN值缺失。
        ● 偏见数据。在数据收集的时候已经潜在的对数据做了过滤，比如在 CBD 地区白领
        出没的地方调研路过人的英语水平。肯定会比实际值高

12. 数据当中的NaN是什么意思？
      NaN，是Not a Number的缩写，表示没有数据。也可以表示处理计算中出现的错误情况
      ，比如一个数除以0或者求负数的平方根。

13. 什么是布尔值？
      布尔值就是 True 和 False ，是一种状态标识，常与判断和循环一起使用。

14. 在计算中位数的时候，异常对结果的影响大不大？
      影响不大 中位数的优势在于它能避免数据的平均水平受到异常值的影响。

15. 什 么是箱线图？箱线图有哪些重要的度量？
      箱线图（Box-plot）又称为盒须图、盒式图或箱形图，是一种用作显示一组数据分散情况
      资料的统计图。因形状如箱子而得名。它主要用于反映原始数据分布的特征，还可以进行
      多组数据分布特征的比 较。箱线图的绘制方法是：先找出一组数据的最大值、最小值、中
      位数和两个四分位数；然后， 连接两个四分位数画出箱子；再将最大值和最小值与箱子相
      连接，中位数在箱子中间。主要包含六个数据节点，将一组数据从大到小排列，分别计算
      出他的上边缘，上 四分位数 Q3， 中位数 ，下四分位数Q1，下边缘，还有 异常值 。

16. 什么是五数概括法？
      五数概括法即用五个数来概括数据的方法。五数包括最小值；第1四分位数(Q1)；中位数
      (Q2)；第3四分位数(Q3)；最大值。

17. 什么是假设检验？
      根据一定假设条件由样本推断总体。假设检验是一种基本的统计推断形式，也是数理统计
      学的一个重要的分支，用来判断样本与样本，样本与总体的差异是由抽样误差引起还是本
      质差别造成的统计推断方法。