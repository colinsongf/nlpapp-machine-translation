# NLP WEBAPP

# 项目背景 
+ 由于对基于深度学习的自然语言处理技术较为感兴趣，于是用bert训练了两个有趣的机器人,算法不服主要还是借鉴了苏神的项目
+ 自动写词机器人和阅读理解机器人
# 项目技术
### 项目目录
![project](/img/project.png)
+ 其中train目录下时模型训练，包含训练数据
+ stastic和template是前端部分
+ 预训练的bert权重从https://github.com/ymcui/Chinese-BERT-wwm下载的RoBERTa-wwm-ext的版本
+ 训练好的模型会放在models文件夹中
+ app.py ci.py mc.py 是后端部分

### 算法部分
+ 自动写词机器人的算法部分主要借鉴苏剑林大神的这篇博客https://spaces.ac.cn/archives/6933,
+ 阅读理解机器人的的算法部主要借鉴苏剑林大神的这篇博客https://spaces.ac.cn/archives/6736,
### 部署部分
+ 前端技术 bootstrap,js,css
+ 后端技术 flask
# webapp 演示部分
### 自动写词机器人
##### 其中第一个form填**词牌名**，格式是——**“菩萨蛮：”** , 第二个form填beamsearch解码器的**topk值**,不同的topk会生成不同的词。
当beamsearch的 topk = 6时
![generate_ci](/img/ci1.png)
当beamsearch的 topk = 10时
![generate_ci](/img/ci2.png)
### 阅读理解机器人
##### 其中第一个form填入**资料**， 第二个form填入**问题**,机器会自动帮你寻找到合适的答案。
演示1
![geerate_ans](/img/mc1.png)
演示2
![generate_ans](/img/mc2.png)
# TO DO
+ 采用容器化技术docker实现项目的部署
+ 增加更多的NLP相关的机器人

