---
layout: single
classes: wide
title: "新生指导"
permalink: /teaching/orientation/
author_profile: false
comments: true
toc: true
toc_label: "目录"
toc_icon: "cog"
toc_sticky: false
breadcrumbs: true 
---
# 资料（及线路图） 

## 通用类
 
### 编程

#### PyTorch [PyTorch Tutorial](https://github.com/yunjey/pytorch-tutorial) [Awesome PyTorch List](https://github.com/bharathgs/Awesome-pytorch-list)
#### TensorFlow [Example](https://github.com/aymericdamien/TensorFlow-Examples)[中文Tutorial](https://github.com/czy36mengfei/tensorflow2_tutorials_chinese)

### 机器学习

#### 李宏毅机器学习课程[B站2022版](https://www.bilibili.com/video/BV1Wv411h7kN?spm_id_from=333.337.search-card.all.click) 机器学习基础，必看，可以和推荐专业知识同时推进
#### 李沐：动手学深度学习[B站](https://space.bilibili.com/1567748478/channel/seriesdetail?sid=358497)可以在上一个视频的理论知识看过了之后看所有动手部分

### 推荐专业相关

#### 教材自学（Recommender Systems Handbook）[《推荐系统 : 技术、评估及高效算法》](https://manongbook.com/download/909.html)很全面，一般读不完，看下框架了解整个领域知识结构就可以，留作参考书

#### 中文课程[推荐系统_北京大学_中国大学MOOC(慕课)](https://www.icourse163.org/course/PKU-1464038187?from=searchPage)中文，适合零基础入门

#### 英文课程[DeepRecSys Tutorial @ WWW2021](deeprs-tutorial.github.io)知识点比较新，是关于深度学习在推荐系统中的应用，必看

### 可以使用的开源工具

#### 相对较全[microsoft/recommenders: Best Practices on Recommendation Systems](https://github.com/microsoft/recommenders)
#### 只针对隐反馈[THUIR/ReChorus: “Chorus” of recommendation models](https://github.com/THUIR/ReChorus)

# 查阅文献

## 哪里找论文

### 有目的查找-做课题前必须尽量查全！！！
通过关键词查找入口[Googlescholar](scholar.google.com)全 [DBLP](https://dblp.uni-trier.de/)比较干净，但只有计算机领域论文。
记得通过*更换关键词,已有论文的引用文献和被引论文（广度优先）* 迭代搜几次，不要漏过当年顶会刚出的论文。
优先顶会、近3年、经典论文（高被引）。
如果一个课题已经有一定数量的工作了，可以通过survey（优先查顶刊、大牛写的、和老师推荐的survey）来直接获得相关工作的概貌。
**仅供查文献，下载前记得修改格式**

### 平时积累
建议通过习惯App养成每天读论文的习惯。
关注每年顶会，顶会出的时间我们组会会把相关论文过一遍[最新版《中国计算机学会推荐国际学术会议和期刊目录》](https://www.ccf.org.cn/Academic_Evaluation/By_category/)
关注公众号[PaperWeekly](https://www.jiqizhixin.com/columns/paperweekly)[智源社区](https://hub.baai.ac.cn/)[微软研究院AI头条](https://www.jiqizhixin.com/columns/Microsoft_AI)。
实验室鼓励报名参加讲座[CCF ADL](https://www.ccf.org.cn/Activities/Training/ADL/)[VLDBSschool](http://vldbss.org/)以及各种领域专会，基本都可以资助报名和差旅费用，需要先申报，并符合学校政策。

## 读论文
### 文献整理
1. 推荐使用的文献整理工具[JabRef](https://www.jabref.org/)和[Endnote](https://net.xmu.edu.cn/)。
2. 如果一篇论文有多条搜索结果，常见的是一个预印本arxiv版本，一个正式发表版，选择正式发表版本的。
3. **绝对不要从百度学术**，Google或者 Google Scholar下载bib文件，如果从DBLP下载，记得选择condensed格式。优先建议[ACM Digital Library](https://dl.acm.org/)、[IEEE Xplore](https://ieeexplore.ieee.org/Xplore/home.jsp)、[Elsevier](https://www.sciencedirect.com/)，必须从学校IP访问或者VPN(https://net.xmu.edu.cn/)或者[厦大图书馆](https://library.xmu.edu.cn/)。
4. 从推荐的源头即出版商本身下载的bib文件一般是比较少错的，删除掉doi、url。从其他源头如DBLP下载的就一定要修改。publisher这一项，除非是书（book），对于会议（inproceedings）和期刊（article）论文这一项都删除以节省空间并避免歧义。如果是arxiv论文，将journal改为arXiv Preprint，去掉volume，并加上arXiv的url。如果遇到会议名称里带数字和括号的情况，要回去会议网站查证后修改booktitle和volume等信息。最后，把期刊会议名换成缩写，可以手动，如果是JabRef，在Option-Manage Journal Abbreviations里修改。
5. 确认格式正确后，肉眼检查下结果的准确性（如姓名顺序、期刊编号、页码和会议期刊名称等），修改索引名，索引名里不能出现斜杠“/”否则在有些tex编译过程中会出错。个人建议在JabRef的Preference里改成[author][year][shortname]（完全是出于后续改论文记文献方便），也可以有自己的命名体系。

### 文献阅读
快速扩充领域知识可以用**摘要+图粗读法**。

强烈建议保持一个阅读记录如下：

|编号|方法名|类别|动机|实现|结果|开源|
|----|-----|----|---|----|----|----|
|Chen2021Adapting|IOBM|Counterfactual LTR|assumes that each observation in a ranking list is not isolated and interactions between observations/clicks should be considered|click/position/query -> embedding ->attention ->BiLSTM-FFN|ranking results (MRR + NDCG) on Amazon Books|github.com|

有同学使用mindmap管理文献之间的分类和承上启下关系也非常好。

[best paper](https://jeffhuang.com/best_paper_awards/)以及强相关论文需要**精读**，要做到：
1. 公式能推导，必要时看参考文献
2. 代码能重现（求甚解！！！）
3. 记录可用的技术，尤其是非本领域
4. 学习写作技巧，摘录图、句子
5. 实验细节：数据集、比较实验、评估指标、可视化、预处理等
6. survey或者种子论文参考文献要看全

每隔一段时间写一小段阅读文献总结，把相同方法或技术路线的集中起来，分析他们的动机、实现方法和优劣。
