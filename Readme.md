# 文本情感分析

本程序用来对B站评论爬虫进行文本情感分析

## 数据获取（B站爬虫）

获取评论文本，得到 Init.txt      

    python review.py 



##数据清洗

   文本替换和预处理

##中文分词 


    pip install jieba
    python wenben.py

生成

	fenci_result.txt

##去除停用词

创建停词文本   
	
	stopwords.txt

删除停用词

    python  del_word.py

生成

	fenci_qutingyongci.txt

##词频统计

    python sta_word.py

生成词频统计,可生成词云 

	fenci_qutingyongci_cipin.txt


## 情感分析

导入 SnowNLP 包：下载 SnowNLP 的 [Github](https://link.csdn.net/?target=https%3A%2F%2Fgithub.com%2Fisnowfy%2Fsnownlp) 源码并解压，在解压目录，通过下面命令安装

	python setup.py install 

将下载的文件改为 zip 格式，将解压之后的文件夹中的两个文件放到 Python 的安装目录 –> Lib –> site-packages。

对评论文本 emotion.xlsx 进行情感分析

	python emotion.py



![](https://img-blog.csdnimg.cn/05a76e5648fc4d2c886015c430739837.jpg?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5Li65LqG5piO5aSp6ICM5aWL5paX,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)

最终生成文件 qinggan.xlsx 和情绪分析图.
