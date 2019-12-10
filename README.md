# 预约拍照app

发布日期 | 2019/12/3 
-|-
Epic | 预约拍照App |
文件现状 | 进行中 |
文件主人 | 何政阳 |
领头设计者 | 何政阳 |
领头开发者 | 何政阳 |
领头测试者 | 何政阳 |

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

## 原型-部分功能说明
#### 1、首页——所有的预约功能都是在这实现的
![首页](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E9%A6%96%E9%A1%B5.png)
系统会为用户推荐目前合适拍摄地点，当然用户不满意的话也可以在这里选择自己想选择的地点，同样的系统会为用户推荐当前地点热门的标签，用户不喜欢的话也可以自行更换。点击搜索后系统会为用户选择的标签和当前距离较近的摄影师进行综合排序，也可以按照摄影师的距离进行排序。点击摄影师即可进入他的详情页，如果客户喜欢即可点击预约。  

#### 2、预约订单——所有历史预约订单都可以在这里进行查询
![预约订单](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E9%A2%84%E7%BA%A6%E8%AE%A2%E5%8D%95.png)
预约订单将会根据从新到旧进行排序，用户点击正在进行的订单的话可以查看预约的地点和时间，并且可以联系摄影师。  

#### 3、论坛——用户可以在这里学习专业摄影师发布的摄影教程
![论坛](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E8%AE%BA%E5%9D%9B.png)
论坛的置顶会摆放编辑精选的摄影教程，用户可以点击“查看更多”查看更多精选文章也可以往下划查看全部文章，或是自己收藏的文章。点进文章后，页头会显示标题、发布时间以及作者。  

#### 4、个人中心——用户自己的账户设置以及申请成为摄影师将在这里进行
![个人中心](https://github.com/SunnyHe1999/API_ML_AI/blob/master/image/%E4%B8%AA%E4%BA%BA%E4%B8%AD%E5%BF%83.png)
用户对于自己的账户设置比如偏爱的标签、头像等都可以在这里进行更改。而下面的“我要成为摄影师”按钮可以让用户上传自己的一系列精选照片，让系统给他生成推荐的标签，当然用户不喜欢也可以自己删改，并且配上对自己简短的介绍，这段简介会出现在预约界面里，让其他用户对你有一个大概的认识。  

## 目标用户
* 移动购物与支付用户
* 爱美人群
* 自由摄影师
* 中小型企业

## 功能简介
* 根据用户选择标签推荐符合的摄影师，比如用户选择了“旅拍”“人像”标签，就会推荐上传精选作品多为“旅拍”“人像”标签的摄影师。

* 附近的人：通过筛选条件，筛选出附近的摄影师进行拍摄。

* 提供大量精美的拍摄教程，教用户如何自拍好看。

## 使用到的API
* [高德地图定位API](https://lbs.amap.com/getting-started/locate). 
* [百度通用图像分析API](https://ai.baidu.com/tech/imagerecognition/general). 
