# 每日一题&答案 - Day3

1. Pandas 的 read_csv 函数作用是什么？

  city_data = pd.read_csv('BeijingPM20100101_20151231.csv')
  此模块的作用是将文件读入DataFrame,还支持可选地将文件迭代或者分割成块。个人觉
  得是将csv文件加载入pandas,使其具有各种属性，更容易地被编辑和操作。具体文档参考
  http://pandas.pydata.org/pandas-docs/version/0.18.1/generated/pandas.read_cs
  v.html

2. 如何查看一个dataframe里面有多少条数据？

  使用 len() 函数或者 describe() 函数

3. pandas 取出df数据中字段名为‘city’的这一列？

  df['city']

4. df_all_cities.head(10)会显示几行数据，如果想要显示5行数据，应该怎么写？

  10行， df_all_cities.head(5)

5. info()是干什么用的

  info函数可以看到数据的信息，比如总的数量，有多少是空的，等等

6. python 当中的out_columns = ['No', 'year', 'month', 'day']，请问我打印out_columns，接
    下来会显示什么内容？

  ['No', 'year', 'month', 'day']

7. pandas的dataframe有很多方法的参数都有axis这一项，比如dropna，sum等，axis可
    以为1或者0。你是如何理解axis=1和axis=0的？（提示：从列和行的方向考虑）

  使用0值表示沿着每一列或行标签向下执行方法，使用1值表示沿着每一行或者列标签模向
  执行对应的方法。

8. pandas 中的series和dataframe有什么区别和联系？

  Series相当于数组。DataFrame相当于表格，有行表头和列表头。DataFrame可以看作是
  由一列列Series组成的，如果要这么生成DataFrame的话，需要采用字典模式的参数。
  Series也可以有index，但没有columns。

9. 假设有一列‘PM_US Post ’，df[‘PM_US Post ’].sum()的输出是什么值

  PM_US Post这一列数值的求和

10. Shanghai_data里面的'season'这一列是1,2,3,4的取值，请问Shanghai_data['season'] =
    Shanghai_data['season'].map({1:'Spring', 2:'Summer', 3:'Autumn', 4: 'Winter'})这里的
    map方法做了什么事情？

    Shanghai_data中season列中的值是1,2,3,4.但是我们不知道1,2,3,4所代表的具体含义。
    map()函数将season列中的1,2,3,4进行映射，从而使1,2,3,4具体转换为字符串“Spring”,
    “Summer”, “Autumn”, “Winter”.

11. print('Hellow'.upper()) 会输出什么？

    HELLOW 因为.upper()就是把输出转为大写字母

12. copy.copy() 能够实现什么功能？

    copy是python中用于复制的标准库。用于复制列表（这样再修改新的列表，原列表不会
    改变）

13. Python 的 strip 方法是做什么用的？

    Python strip() 方法用于移除字符串头尾指定的字符（默认为空格或换行符）。

14. 如何查看dataframe df的列名和索引名字？(提示：列和索引的英文单词)

    df.columns和df.index，可以用这个来对列名和索引名字进行修改。比如
    df.columns=['a','b','c']

15. python 代码里面文本注释前面要加什么符号？

    #

16. pandas中的isnull()函数是什么意思？

    查看缺失数据

17. pandas中的duplicated()函数是什么意思？

    查看重复数据