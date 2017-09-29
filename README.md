# ML-Perceptron
http://www.imooc.com/qa/813/t/1?page=1  机器学习-实现简单神经网络，在2.7基础上修改在3.6上完美运行，原参考链接：https://github.com/a414351664/Perceptron-sort-algorithm/blob/master/PerceptronTest.py

关于CSV文件问题：
file = 'https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'
import pandas as pd
df = pd.read_csv(file,header=None)
df.head(10)
1.网址是文件的原地址，数据是可以直接从网址上拔下来的。
2.如果运行以上代码csv的文件，网站只能下载txt需要下载txt后转化成csv。
以上运行结果一致。

file = 'https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'
df1= pd.read_csv(file,header=None)
df1.to_csv('test.csv',index=False,header=None)
这样就可以把数据保存为csv了，没有加路径，就在代码所在位置，运行一次后，注释掉就可以了

结合上述两个方法，print的格式由2.7版本的转成3.6；源代码没有修改CSV，我加入上面几行保存链接为CSV格式的代码，运行正常，直接输出结果
代码参考：
https://github.com/rasbt/pattern_classification
机器学习算法原理之人工神经元和单层神经网络
http://www.ranling.com/category/it/689240.html
