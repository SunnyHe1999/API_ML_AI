# 预约拍照app

发布日期 | 2019/12/3 
-|-
Epic | 预约拍照App |
文件现状 | 进行中 |
文件主人 | 何政阳 |
领头设计者 | 何政阳 |
领头开发者 | 何政阳 |
领头测试者 | 何政阳 |

# 1.价值主张设计
## 产品定位
本产品旨在为广大用户记录美好生活，拍下美丽瞬间。

## 价值宣言
本产品旨在运用定位以及图像分类技术为客户找到适合他们的摄影师。

## 加值宣言
#### 1、高德地图API对本产品的价值
* 移动互联时代，定位无处不在，任何一个应用只要想了解用户的位置，不管是为用户提供服务还是用于用户分析，就一定会用到定位，高德定位SDK通过GPS+基站定位+WiFi的混合定位模式进行定位，不论在室外、室内还是在高楼林立的城市峡谷，都可以实现精准的定位。之后再通过算法的筛选就可以快速找到附近的用户/摄影师。

#### 2、百度通用图像分析API对本产品的价值
* 基于百度深度学习的图像识别技术，支持超过10万类常见物体和场景识别，接口返回图片内1个或多个物体的名称，通过丰富的标签体系可以识别摄影师上传的精选作品，使用户可以通过这些标签快速找到适合自己的摄影师。

## 用户痛点
* 针对性
想象一下用户有一天穿得美美的出去逛街，可自拍就是怎么也不好看达不到想要的效果，这时候就需要一位专业摄影师来为她进行拍摄，通过本产品就可以使用筛选系统找到附近的摄影师。
* 普遍性
目前市面上的同类产品都是面向大型的商业活动，价格都极为昂贵不是一般人能承受得起的，而使用预约体验也不好。对于很多普通人来说都不知道如何寻找摄影师，一般都是通过熟人介绍，可选择的余地不多，通过本产品用户通过不同标签找到适合自己的摄影师。

## 用户需求
#### 显性需求
* 用户随时随地想拍美照的需求
* 用户想用较少的价钱拍摄美照的需求
* 自由摄影师想接更多单子的需求

#### 隐性需求
* 小型公司经费不足请不动专业的摄影公司，可以请花费相对较少的自由摄影师

## 目标用户
* 移动购物与支付用户
* 爱美人群
* 自由摄影师
* 中小型企业

## 功能简介
* 根据用户选择标签推荐符合的摄影师，比如用户选择了“旅拍”“人像”标签，就会推荐上传精选作品多为“旅拍”“人像”标签的摄影师。

* 附近的人：通过筛选条件，筛选出附近的摄影师进行拍摄。

* 提供大量精美的拍摄教程，教用户如何自拍好看。

# 2.产品原型设计
#### 1.整体预约交互流程（首页）
![首页交互流程](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E9%A6%96%E9%A1%B5%E4%BA%A4%E4%BA%92%E6%B5%81%E7%A8%8B.png)  

#### 2.论坛页交互流程
![论坛页交互流程](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E8%AE%BA%E5%9D%9B%E9%A1%B5%E4%BA%A4%E4%BA%92%E6%B5%81%E7%A8%8B.png)  

#### 3.成为摄影师交互流程
![成为摄影师交互流程](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E6%88%91%E7%9A%84%E9%A1%B5%E4%BA%A4%E4%BA%92%E6%B5%81%E7%A8%8B.png)  

## 口头操作说明
本款预约拍照APP一共有3个主要功能。预约拍照为核心功能，在首页输入自己对应的位置和使用标签即可根据这些信息搜索摄影师，按需排序摄影师后点击进入详情页，如果客户喜欢即可点击预约，预约成功后即会转到订单页可以查看预约的地点和时间，并且可以联系摄影师。第二个主要功能为论坛，置顶会摆放编辑精选的摄影教程，用户可以点击“查看更多”查看更多精选文章也可以往下划查看全部文章，或是自己收藏的文章，点进文章后，页头会显示标题、发布时间以及作者。第三个主要功能就是“我要成为摄影师”了，单击按钮可以让用户上传自己的一系列精选照片，让系统给他生成推荐的标签，当然用户不喜欢也可以自己删改，并且配上对自己简短的介绍，这段简介会出现在预约界面里，让其他用户对你有一个大概的认识。

# 3.API测试
#### 1、百度图像识别API
![百度图像识别API](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E7%99%BE%E5%BA%A6%E5%9B%BE%E5%83%8F%E8%AF%86%E5%88%ABAPI%E8%B0%83%E7%94%A8%EF%BC%88%E9%99%84%E5%9B%BE%E7%89%87%EF%BC%89.png)
* 输入：女模特摆拍照片
* 输出：人物特写、美女、演唱
* 判断：不完全正确（这并不是演唱，但确实是美女的人物特写照片）
* 检测时间：约3秒（尚可接受）

#### 2、高德定位API
![高德定位API](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E9%AB%98%E5%BE%B7%E5%9C%B0%E5%9B%BEAPI%E8%B0%83%E7%94%A8.png)
* 输入：中山大学南方学院
* 输出：中山大学南方学院
* 判断：正确
* 检测时间：约1秒

## API价格
#### 高德定位API价格
![高德定位API价格](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E9%AB%98%E5%BE%B7%E5%AE%9A%E4%BD%8DAPI%E4%BB%B7%E6%A0%BC.png)

#### 百度图像识别API价格
![百度图像识别API价格](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E7%99%BE%E5%BA%A6%E5%9B%BE%E5%83%8F%E8%AF%86%E5%88%AB%E4%BB%B7%E6%A0%BC.png)

## 使用到的API
* [高德地图定位API](https://lbs.amap.com/getting-started/locate). 
* [百度通用图像分析API](https://ai.baidu.com/tech/imagerecognition/general). 

# 价值主张训练

## 一句话版本
本产品旨在为用户寻找符合自己心水的摄影师

## 一分钟版本
本产品专注于减少用户与摄影师的“距离”，让用户和摄影师更快地“找到”对方。通过使用图像识别API可对摄影师上传的照片进行分类标签整理，而整理出来的标签可供用户进行选择以找到对应自己心水的摄影师，定位API更是可以搜索到在附近的摄影师，系统将会根据用户选择的标签和距离综合排序摄影师，用户只需按需选择即可。同时提供丰富有趣的摄影教程帮助用户提高摄影水平，提高用户粘性，甚至能把用户转化为摄影师。
