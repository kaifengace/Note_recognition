

# 项目名称：“全票” 票据小助手
## Product Documentation(产品需求文档)
---
|  Title   |   Content  |
| --- | --- |
| Target release    |  2019/11   |
|  Epic   |  “全票” 票据小助手  |
|  Document status   |  进行中   |
|  Document owner   |  胡凯锋  |
|  Designer   |  胡凯锋   |
|  Developer   |  胡凯锋   |
|  QA   |   胡凯锋  |

- 版本修订记录

|修订版本号|迭代日期|修订内容|迭代者|
|---------|-------|--------|-----|
|v1.0|11.20-12.01|文档初稿撰写，建立基本产品文档框架，添加重要产品理念与技术开发项目流程|胡凯锋|
|v2.0|12.01-12.08|测试可用 API 并进行可用性测试比对，进行市场回访调查|胡凯锋|
|v3.0|12.08-12.15|选定 API 类型并实现测试运行，产品后台代码实现可用|胡凯锋|
|v4.0|12.15-12.22|开发 APP 原型，制作低保真原型初步实现逻辑|胡凯锋|
|v5.0|12.23-     |产品上线并进行不断功能反馈|胡凯锋|

## Documentation Directory(文档目录)
---
- [产品介绍](#产品介绍)
- [市场背景](#市场背景)
- [价值主张设计](#价值主张设计)
  - [加值宣言](#加值宣言)
  - [核心价值宣言](#核心价值宣言)
  - [用户痛点宣言](#用户痛点宣言)
  - [人工智能概率性与用户痛点](#人工智能概率性与用户痛点)
  - [需求列表与人工智能API加值](#需求列表与人工智能API加值)
- [原型文档](#原型文档)
  - [交互及界面设计](##交互及界面设计)
  - [信息设计](#信息设计)
  - [原型文档](#原型文档)
  - [口头操作说明](#口头操作说明)
- [API 产品使用关键AI或机器学习之API的输出入展示](#API产品使用关键AI机器学习之API的输出入展示)
  - [使用水平](#使用水平)
  - [使用比较分析](#使用比较分析)
  - [使用后风险报告](#使用后风险报告)
  - [加分项](#加分项)

# 产品介绍
---
“全票” 票据小助手“ 是一款基于文字识别和图像识别的票据收录小助手，专门针对有票据收录整理需求的用户推出的一个便捷、专业、安全的平台，让用户不再票据杂乱而感到苦恼，让它从此“井然有序”的呈现在你眼前。

# 市场背景
---
经过调查研究，随着移动互联网及通讯设备的普及，不难发现目前已有不少整理票据的APP，例如“票据宝”，“票据管家”等，专门针对票据客户提供的APP。但是随着人工智能的发展，文字识别将有效的代替各种繁琐冗杂的票据信息录入，基于此，票据小助手类轻巧便捷的小程序无疑是更好的整理票据的一种形式，因而，“全票”的诞生就变得非常有必要。

 **优势**

>- 涵盖多样的票据类型，使用便捷性提高。
>- 市场占比少，市面上仅有数款票据APP，市场有待进一步扩张。
>- 功能齐全，界面功能简洁易懂，可以分类整理各类票据。

#### **竞品分析**

**竞品：财政票据管理系统**

优点：
>- 功能齐全，包含偏好设置，各种查询入口 ，还有票据销毁等隐私保护措施。

缺点：
>- 界面不够简洁美观，功能界面不清晰。
>- 录入系统不方便，需要手动输入，不能拍照识别和本地上传，过于繁杂。
>- 版本太低，太久没更新了已经不适合现代人使用，

# 价值主张设计
### （一）加值宣言
采用百度的文字识别API和图像识别API对现有产品进行加值和优化。 运用了机器学习中的图像文字识别的功能，通过即对于输入的一张图片（可正常解码，且长宽比适宜），使用混贴票据识别技术，对企业员工提交的原始票据粘贴单进行识别，有效提升财务核算效率，降低企业人力成本，实现财务报销的自动化。

百度图像识别api的价值: 
>-  将票据上的logo信息自动识别后自动分门别类，省去了整理各类票据的时间，提高了效率。

文字识别api的价值：
>- 可以将各类票据的票面文字信息直接转成文字。

发票验真api的价值：
>- 使用增值税发票识别技术，实现对发票代码、号码、开具金额、开票日期四个关键字段的识别，供用户接入税务机关发票查验平台进行真伪查验，能够实现发票真伪查验的自动化，有效降低人力成本，控制业务风险。

财务报销api的价值：
>- 使用混贴票据识别技术，对企业员工提交的原始票据粘贴单进行识别，自动完成各类报销凭证的自动切分及结构化识别，可应用于企业内部财务报销、核算、记录等场景，有效提升财务核算效率，降低企业人力成本，实现财务报销的自动化。


### （二）核心价值
- 最小可行性产品（产品的核心价值）
着眼于用户的最基本需求，提供图像logo识别和文字识别功能，解决用户管理票据信息繁琐冗杂的问题，同时提供永久记忆保存的最基础服务。
---
1）产品背景：
现在我们出行，购物，医疗甚至买彩票 都会产生票据，例如火车票，购物小票，增值税票等。每日收到票据的票据可能多而杂乱，因此对于票据的内容及对票据本身的整理和保存显得尤为重要，这款APP对票据的票面内容进行识别，能减少用户人工输入成本，大幅度提升录入效率及用户使用体验。

2）产品目的：
让票据信息不再繁多冗杂，实现永久记忆保存。

3）产品目标：
 拍下票据，识别票据类型并分类整理。
拍下票据，识别票面信息，收集并以文字的形式反馈给用户。

4）产品用户：
公司企业财务审核人员、车机站票据工作人员，需要整理收集各种票据的用户。

### （三）核心价值与用户痛点
|  核心价值 | 用户痛点说明 |
 | -- | -- |
 |  **便捷性** | 用户可以不用通过人工输入文字信息等繁琐的操作，只需要通过手机拍照识别相应的票据类型后即可返回票据内容。 |
 |  **永久性** | 在当代社会，生活处处是票据，管理并保存好这些大量的票据成为用户的一大需求，这款APP可实现对各种票据信息录入并分门别类的进行永久保存。 |

### （四）人工智能概率性与用户痛点

* ###### 百度AI文字识别功能的保障：
 1、针对各类票据的打印字体和样式、套打偏移情况进行专项优化，识别准确率可达95%，各类票据切分准确率可达99%以上。
 2、依托百度云技术实力，提供高可靠性、弹性可伸缩、高并发承载的文字识别服务，服务可用性高达99.99%。

> 据此，该产品票据识别功能准确率有保障，通常不会出现与实际数据偏差太大的情况，但是由于此功能以外的因素（如网络延迟或者卡顿无法使视频图像被正确识别）会导致数据输出延迟或者不准确，此概率事件可以通过改进得到缓解，对用户的负面影响不会过大。


### （五）需求列表与人工智能API加值

##### 需求列表

|  主题   |  用户案例   |  重要性   |  备注   |  api加值   |
| --- | --- | --- | --- | --- |
|  文字识别收集 |  用户A需要通过拍照识别录入各种票据的票面信息  |  核心功能   |  对文字识别api的精确度要求高   |  百度文字识别api   |
|  票据分类整理   |  用户B想把所有的票据通过拍照识别其类型并分类整理好，以便以后进行查看。   |  次核心功能   |  信息云储存   |  百度图像识别api   |
|  信息永久存储   |  用户C想要永久存储票据信息，为了以后能在想查看的时候能查看   |  次核心功能   | 信息云储存      |  云存储  |

##### 人工智能API加值

百度图像识别api的价值: 
>- 将票据上的logo信息自动识别后自动分门别类，省去了整理各类票据的时间，提高了效率。

文字识别api的价值：
>- 可以将各类票据的票面文字信息直接转成文字。

行程单api的价值：
>- 使用行程单识别技术，实现对乘机人姓名、日期、始发站、目的站、票价等信息的自动识别和录入，应用于企业税务核算及内部报销等场景，能够有效减少人工核算工作量，降低人力成本，实现财税报销的自动化。

混贴票据api的价值：
>- 可对粘贴在同一张A4纸上的多张不同种类票据进行自动切分，并返回每张票据的位置、种类及票面的结构化识别结果，方便进行后处理。支持识别多种常用票据混合排布的粘贴单，并可准确识别各类票据的多个关键字段，满足财会报销场景的信息提取需求。

通用票据api的价值：
>- 使用通用票据识别技术，实现对各类购物小票、医疗票据、银行兑票等非标准型报销凭证的识别和录入，可应用于企业税务核算及内部报销等场景，能够有效减少人工核算工作量，降低人力成本，实现财税报销的自动化。

# 原型文档
### （一）交互及界面设计
设计小助手界面布局达到可视性从而使用户产生可记忆性，流畅的交互体验，流程设计可使用户提高对产品的使用效率，增强用户对产品的可学习性。

|核心功能|交互设计|界面设计|
 |---------|-------|-------| 
|票据识别|拍照上传票据照片进行识别|简洁大方| 
|票据收藏|各类票据分窗口收藏|简洁大方|

### （二）信息设计
1）产品框架图
![框架图](https://github.com/kaifengace/Note_recognition/raw/master/%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB%E6%9E%B6%E6%9E%84%E5%9B%BE.PNG)

2）产品流程图
![流程图](https://github.com/kaifengace/Note_recognition/raw/master/%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB%E6%B5%81%E7%A8%8B%E5%9B%BE.PNG)

### （三）原型文档
#### 1）原型的全局说明

###### 功能权限分为登录/未登录两个状态：

*   登陆状态：用户能操作所有功能，查看管理所有个人票据。
*   未登陆状态：只能进行简单的操作，如拍照识别。但是不能被保存记录等。

###### 底部栏：
首页：首页的功能包括记录信息、撰写文章和文本审核。
我的：我的页面可以登陆/注册，和查看个人稿箱等。

*  票据：票据页面的功能包括票据管理、票据管理和查看最近。
*  主页：主要页面的识别功能。
*   我的：我的页面可以登陆/注册，和查看个人收藏等。

#### 2）原型文档交互展示
- 最小可行性产品的交互界面可以交互的文档，

##### [Axure原型文档交互展示](http://hukaif.gitee.io/api_final)


##### [Axure原型下载地址](https://gitee.com/hukaif/API_final)
![产品交互及设计低保真原型](https://gitee.com/hukaif/API_final/raw/master/%E7%A4%BA%E4%BE%8B.PNG)
# 口头操作说明
- 已在课堂完成此部分

# API 产品使用关键AI或机器学习之API的输出入展示

### （一）使用水平
**概要：核心功能票据识别的代码展示——文字识别+图像识别**

##### 1）百度文字识别
- [混贴票据识别](https://ai.baidu.com/tech/ocr/mixed_receipt)
- [通用票据识别](https://ai.baidu.com/tech/ocr_receipts/receipt)
- [行程单识别](https://ai.baidu.com/tech/ocr_receipts/air_ticket)

##### 2）百度图像识别
- [品牌logo识别](https://ai.baidu.com/tech/imagerecognition/logo)
---
**输入：票据票面信息；输出：文字**

**输入：图片；输出：文字**
- [代码示例](https://github.com/kaifengace/Note_recognition/tree/master/final/code)


### （二）使用比较分析

#### 票据识别比较

- 通过搜索引擎发现排名较为靠前的百度ai开放平台和阿里开放平台提供票据识别服务并对此进行比较

|对比项|百度|阿里|
|---|---|---|
|代码比较|[百度票据识别api详细代码示例](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E7%99%BE%E5%BA%A6%E9%80%9A%E7%94%A8%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB.ipynb)|[阿里票据识别api详细代码](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E9%98%BF%E9%87%8C%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB.ipynb)
|使用效果|基于各种场景提供多种识别模板，针对各类票据特定的字体、打印样式进行优化，综合场景下字段准确率高达98%，其中增值税发票、出租车票四要素准确率高达99.9%|支持对增值税发票、火车票的结构化识别；及对医疗票据、保险保单、银行兑票、购物小票、的士发票等各类票据进行通用识别，并按行输出所有文字结果
|成熟度|[百度票据识别](https://ai.baidu.com/tech/ocr_receipts)有相应开发语言的调用示例代码，并与数个大公司有合作关系，服务较为成熟。|[阿里票据识别](https://market.aliyun.com/products/57124001/cmapi031364.html?spm=5176.730005.productlist.d_cmapi031364.319535240sA67h&innerSource=search_%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB#sku=yuncode2536400001)界面较为杂乱，调用方法和过程比较繁琐，没有给定参考代码，服务刚刚推出，处于起步阶段|
|性价比|每日 50000 次免费调用量，开通按量后付费。调用失败不计费[百度票据识别api产品价格](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|免费次数为100次服务量，若是付费的话分为三个套餐，5000次服务量238元/年；5万服务量2008/年；50万服务量16008元/年[阿里票据识别api产品价格](https://market.aliyun.com/products/57124001/cmapi031364.html?spm=5176.730005.productlist.d_cmapi031364.2e4f3524emrAZ3&innerSource=search_%E7%A5%A8%E6%8D%AE#sku=yuncode2536400001)|
|服务评估|参数划分完整，提供业务参数，可扩展性强[功能发布记录](https://ai.baidu.com/ai-doc/OCR/zk3h7xw5e)及[api调用教程](https://ai.baidu.com/ai-doc/OCR/Ck3h7y2ia)|仅有api文档且无示例代码，应用场景和参数不完整，无法进行进一步开发调用。|

- 总结：通过对比调取百度ai开放平台和阿里开放平台提供的票据识别api，对比输出结果，综合上述内容，最终选定使用百度开发平台提供的api服务。


### （三） 使用后风险报告

- 自行进行代码测试比较，百度api和阿里api利用同一图片进行比较，百度api识别率更高，但仍存在一些误差，可能会对用户体验造成影响，但本APP可进行自定义编辑，手动输入票据代码，票据名称等，可对错误识别的文字进行更正。

对比项 | 百度 | 阿里 | 总结
---|---|---|---
API市场竞争程度 | bing搜索排行为第三 | bing搜索排行第三五| 百度api搜索引擎排名较前，且是api说明介绍页面，说明经常更新，服务推出较早，比较成熟。阿里仅显示文档调用页面，说明并不是核心业务，推出时间较短。
输入输出限制 | 输出JSON格式 | 输出JSON格式| 对于文字识别的全面性上，百度的服务更为完善。
定价 |[百度票据识别api产品价格](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|[阿里票据识别api价格](https://market.aliyun.com/products/57124001/cmapi031364.html?spm=5176.730005.productlist.d_cmapi031364.2e4f3524emrAZ3&innerSource=search_%E7%A5%A8%E6%8D%AE#sku=yuncode2536400001)| 从免费额度来看，百度提供每日5W次免费调用量，阿里提供30天100次调用的免费调用量。百度可进行更高，按套餐付费与按量付费也比阿里更优惠。

- 总结：综上所述，百度ai服务样式多，性价比更高，故选择百度ai。



### （四） 加分项
- 用到的的api有ogo识别api、百度混贴票据api、百度行程单api、百度通用票据api、阿里票据api
- [logo识别代码示例](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E7%99%BE%E5%BA%A6%E5%9B%BE%E5%83%8Flogo%E8%AF%86%E5%88%AB.ipynb)

- [百度混贴票据代码示例](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E7%99%BE%E5%BA%A6%E6%B7%B7%E8%B4%B4%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB.ipynb)


- [百度行程单代码示例](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E7%99%BE%E5%BA%A6%E8%A1%8C%E7%A8%8B%E5%8D%95%E8%AF%86%E5%88%AB.ipynb)


- [百度通用票据代码示例](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E7%99%BE%E5%BA%A6%E9%80%9A%E7%94%A8%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB.ipynb)


- [阿里票据识别详细代码](https://github.com/kaifengace/Note_recognition/blob/master/final/code/API_%E9%98%BF%E9%87%8C%E7%A5%A8%E6%8D%AE%E8%AF%86%E5%88%AB.ipynb)








