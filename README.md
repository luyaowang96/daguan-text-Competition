# daguan-text-Competition  
competition link http://www.dcjingsai.com/common/cmpt/%E2%80%9C%E8%BE%BE%E8%A7%82%E6%9D%AF%E2%80%9D%E6%96%87%E6%9C%AC%E6%99%BA%E8%83%BD%E5%A4%84%E7%90%86%E6%8C%91%E6%88%98%E8%B5%9B_%E8%B5%9B%E4%BD%93%E4%B8%8E%E6%95%B0%E6%8D%AE.html  
任务要求：建立模型通过长文本数据正文(article)，预测文本对应的类别(class)   

数据集：  
》train_set.csv：此数据集用于训练模型，每一行对应一篇文章。文章分别在“字”和“词”的级别上做了脱敏处理。共有四列：
第一列是文章的索引(id)，第二列是文章正文在“字”级别上的表示，即字符相隔正文(article)；第三列是在“词”级别上的表示，即词语相隔正文(word_seg)；第四列是这篇文章的标注(class)。
注：每一个数字对应一个“字”，或“词”，或“标点符号”。“字”的编号与“词”的编号是独立的！  

》test_set.csv：此数据用于测试。数据格式同train_set.csv，但不包含class。
注：test_set与train_test中文章id的编号是独立的。  

contents：
1、读取数据及数据初识：daguan text competition -- read_data.py
