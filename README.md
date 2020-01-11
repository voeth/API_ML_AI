## 快客app产品需求与市场需求文档
## 很荣幸接受大佬的检阅！大佬辛苦了！ :clap:  :clap:  :clap: :clap:
#### 目录
   1. [市场需求与竞品分析](https://github.com/voeth/API_ML_AI#1-%E5%B8%82%E5%9C%BA%E9%9C%80%E6%B1%82%E4%B8%8E%E7%AB%9E%E5%93%81%E5%88%86%E6%9E%90)  
   2. [用户概述](https://github.com/voeth/API_ML_AI#2-%E7%94%A8%E6%88%B7%E6%A6%82%E8%BF%B0)
   3. [产品介绍](https://github.com/voeth/API_ML_AI#3-%E4%BA%A7%E5%93%81%E4%BB%8B%E7%BB%8D)
   4. [产品原型](https://github.com/voeth/API_ML_AI#4-%E4%BA%A7%E5%93%81%E5%8E%9F%E5%9E%8B)
   5. [风险与应对措施](https://github.com/voeth/API_ML_AI#5-%E9%A3%8E%E9%99%A9%E5%8F%8A%E5%BA%94%E5%AF%B9%E6%8E%AA%E6%96%BD)
#### 1. 市场需求与竞品分析
##### 需求：
根据鲸准研究院做出的2018.05的中国智能客服行业研究报告中提出，中国大约有500万全职客服来应对顾客的咨询需求，并且随着互联网持续为市场经济发展注入活力，咨询业务的需求将越来越多，特别是在金融、教育、电商行业，所以现在涌现出小i机器人、网易七鱼、腾讯企点等一批智能客服厂商利用NLP,深度学习等技术来提高对话服务的工作效率。可见与顾客交谈所产生的数据价值是巨大的，可以根据交谈内容来获取顾客的情感倾向和关键反馈信息，将会为产品带来改进意见，为以用户为中心的设计提供指导。
##### 分析:
现在市场上的智能客服主要的价值主张是取代人工客服，实现高效地跟顾客进行沟通，为企业减少人力、物力成本。与快客app的价值主张不同，我们在于从谈话内容中快速提取对方的谈话重点与情感倾向，为运营商改进产品设计提供参考意见。  
再纵观现在的Saas（软件即服务）市场，还缺乏音频转文本，从文本中提取关键信息和情感态度、可视化反馈结果的三项功能集成的Saas产品。更多的是仅提供其中上述一项的Paas（平台即服务）产品

#### 2. 用户概述
（此部分包括 ）
   1. 受众群体  
   每天需要应对许多顾客的企业客服或产品研发部的工作人员
   2. 用户痛点/增长点/任务 
      1. 在与对方电话沟通的过程中，大部分注意力用于思考答复对方的内容，没有过多的精力去记忆对方的讲话内容，容易导致一些关键信息的遗漏。
      2. 对于企业的客服而言，每天都需要与很多顾客进行沟通，可以通过收集每次顾客与客服谈话的关键信息与情感倾向，就能挖掘出谈话信息的价值，更有针对性的改进产品的功能服务，满足用户需求。
   3. 需求列表
      1. 将谈话内容转化为文本
      2. 通过文本分析出情感倾向、关键信息
      3. 统计关键信息和情感倾向的数据，为用户理解对方的想法、动机提供可视化的建议
#### 3. 产品介绍
   1. 价值主张：
   （此部分加值宣言、MVP核心价值）
   从谈话内容中快速提取对方的谈话重点与情感倾向，为企业收集用户体验
   2. 20*20 展示：（口头说明）
   看文字太累了？看文字没看懂？请收看[视频版20*20的产品介绍](https://www.bilibili.com/video/av82768263?pop_share=1)（喉咙沙哑，说话困难只能配BGM了）
   3. 痛点解决办法：
   主要功能都是调取百度AI开放平台的语音技术与自然语言处理技术的API来实现，使用[音频文件转写API](https://ai.baidu.com/ai-doc/ITMA/Qk38ikh93)实现音频转换为文本；使用[评论观点抽取API](https://ai.baidu.com/tech/nlp_apply/comment_tag)提取文本中的关键信息，再使用[情感倾向分析](https://ai.baidu.com/tech/nlp_apply/sentiment_classify)判断对方的情感态度，可用于做数据统计。
   4. 功能与服务
      1. 批量读取模式或者手动读取模式，批量读取模式需要用户授权给app录音，每当打完电话后就会自动生成音频文件用于统计分析。如果是手动模式的话，就需要用户自己上传音频文件。
      2. 转换成文本后，让用户确认文本内容是否正确，确认无误后就开始提取关键信息，如果用户确认所提取的关键信息无误，就分析情感倾向。
      3. 用户可以选择关键信息呈现的形式（词云、条形图等），也可以选择情感倾向的数据统计区间分组。
   5. 人工智能概率性
1. 百度音频文件转写api的技术以及交流者普通话标准度都会影响音频转文本的准确度，我们可以通过[文本纠错API](https://ai.baidu.com/tech/nlp_apply/text_corrector)来纠正一定的错误。
2. 
#### 4. 产品原型
   1. 产品架构（原型2.信息设计）
![快客app架构](image/快客摘取app.png )  

   2. axure原型（低保真，原型1交互及界面设计、原型3原型文档）
   [快客app_prototype](https://voeth.github.io/API_ML_AI/快客app_prototype/)  
   
   3. 代码示例（API1.输入及输出数据、API4.加分项，我是使用了音频文件转写API、评论观点抽取API、情感倾向分析API，还调用pyecharts模块可视化api输出结果）
   [快客app%20集成百度智能云api开发代码示例](https://voeth.github.io/API_ML_AI/sources/%E5%BF%AB%E5%AE%A2app%20%E9%9B%86%E6%88%90%E7%99%BE%E5%BA%A6%E6%99%BA%E8%83%BD%E4%BA%91api%E5%BC%80%E5%8F%91%E4%BB%A3%E7%A0%81%E7%A4%BA%E4%BE%8B)  
   4. 各种自然语言处理的api比较分析（API2.比较分析） 
   
   企业 |  价格 | 难度
 ---- | ----- | ------  
 百度  | 不开源但是免费使用 | 介入难度不高，直接下载SDK导入即可使用，几行代码即可实现自然语言功能
 阿里  | 每天5万次免费次数，超出后10万次(￥450),50万次 (￥2,000),100万次 (￥3,500) | 接入相对百度复杂一小点点，几乎可以不计，也是API形式调用
 腾讯文智  | 成品1～10万次价格为￥50每万次，10～50万次为￥45每万次，50～100为40每万次，100+为35每万次 | 接口基于腾讯云API，接入相对百度差不多，也是API形式调用。
 
#### 5. 风险及应对措施
（此部分为API3.后风险报告）
##### 风险1：概率性误差
   1. 音频转文字的功能中，如果与普通话不太标准的顾客沟通，甚至有的顾客不会使用普通话与客服交流（百度语音识别仅支持粤语、四川话两种方言），就会大大影响文本转化的正确率将会更低，也将会影响后续提取关键信息和情感倾向的正确率。
   2. 从文本中提取关键信息的功能中，主要风险在于遗漏重要信息，在百度智能云的自然语言处理的评论观点抽取api中，仅抽取名词与形容词，其它实词比如动词、数词、量词被忽略了，可能会导致重要信息的遗漏。
##### 风险2：隐私数据保护问题
   1. 用户可能会对录制通话音频的行为反感。
##### 应对措施：
   1. 针对风险1，遇到使用非普通话交流的顾客，应该尽量引导其使用普通话交流，或者增加调用百度智能云的自然语言处理的[文本纠错API](https://ai.baidu.com/tech/nlp_apply/text_corrector)，提高文本转化的正确率。提取关键信息上，根据业务需求和语言交流环境选择其它自然语言处理的API，比如[新闻摘要API](https://ai.baidu.com/tech/nlp_apply/news_summary),精炼长对话。或者使用中文分词的第三方库对长对话进行分词，再做词频统计。
   2. 针对风险2，加强对通话录音数据的内部管理，禁止将通话内容泄露给第三方，仅用于为提升产品提供反馈意见，不做其它用途，对音频转为文本的内容做脱敏处理。

#### 彩蛋（将于2020.1.11 12:00 互评结束准时删库重建）
![](image/grade.jpg)
我的平时成绩不小心就跌到了48.8分，也差不多要挂科了，恳请大佬高抬贵手。如果觉得我的文档写得很烂或有什么建议可以在下方评论，或者给我发封邮件（13531457409@163.com），我很喜欢接受批评（我也很想做好，却难以理解ht的标准是什么），但请一定要给高分，不然就真的要挂了:fearful: 。 感谢好心人:innocent:

![](image/dalao.jpg)
