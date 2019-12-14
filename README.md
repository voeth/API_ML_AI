## 快客摘取app产品需求文档
#### 1. 市场需求与竞品分析
#### 2. 用户概述
   1. 受众群体  
   通过电话沟通快速提取对方的谈话重点以及情感倾向的用户，特别是每天需要应对许多顾客的客服。
   2. 用户痛点
      1. 在与对方电话沟通的过程中，大部分注意力用于思考答复对方的内容，没有过多的精力去记忆对方的讲话内容，容易导致一些关键信息的遗漏。
      2. 对于企业的客服而言，每天都需要与很多顾客进行沟通，可以通过收集每次顾客与客服谈话的关键信息与情感倾向，就能挖掘出谈话信息的价值，更有针对性的改进产品的功能服务，满足用户需求。
   3. 需求列表
      1. 将谈话内容转化为文本
      2. 通过文本分析出情感倾向、关键信息
      3. 统计关键信息和情感倾向的数据，为用户理解对方的想法、动机提供可视化的建议
#### 3. 产品介绍
   1. 价值主张
   从谈话内容中快速提取对方的谈话重点与情感倾向
   2. 痛点解决办法
      主要功能都是调取百度AI开放平台的语音技术与自然语言处理技术的API来实现，使用[音频文件转写API](https://ai.baidu.com/tech/speech/aasr)实现音频转换为文本；使用[评论观点抽取API](https://ai.baidu.com/tech/nlp_apply/comment_tag)提取文本中的关键信息，再使用[情感倾向分析](https://ai.baidu.com/tech/nlp_apply/sentiment_classify)判断对方的情感态度，可用于做数据统计。
   3. 功能与服务
      1. 批量读取模式或者手动读取模式，批量读取模式需要用户授权给app读取
#### 4. 产品原型
   1. 产品架构
   2. axure原型
   3. 代码示例
#### 5. 产品运营与盈利
