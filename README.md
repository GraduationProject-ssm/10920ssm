# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 10920ssm宠物医院信息管理系统

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Sh44eDEx6?p=21)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

宠物医院信息管理系统工作原理图如图4-1所示：

![](/md/blog.012.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。宠物医院信息管理系统的整体结构设计如图4-2所示。

![](/md/blog.013.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
数据库的概念结构设计采用实体—联系（E-R）模型设计方法。E-R模型法的组成元素有：实体、属性、联系，E-R模型用E-R图表示，是提示用户工作环境中所涉及的事物，属性则是对实体特性的描述。在系统设计当中数据库起着决定性的因素。下面设计出这几个关键实体的实体—关系图。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，公司中的每个用户，家里中的每个家具。

本系统的E-R图如下图所示：

1、医生信息实体图如图4-3所示：

![](/md/blog.014.png)

图4-3医生信息实体图

2、医嘱信息实体图如图4-4所示：

![](/md/blog.015.png)

`     `图4-4医嘱信息实体图

3、订单信息实体图如图4-5所示：

![](/md/blog.016.png)

`     `图4-5订单信息实体图

#########

### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表4-1 allusers表

|列名|数据类型|长度|约束|
| :-: | :-: | - | :-: |
|id|int|11|NOT NULL|
|username|varchar|50|` `default NULL|
|pwd|varchar|50|` `default NULL|
|cx|varchar|50|` `default NULL|

表4-2 keshixinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | - | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|keshimingcheng|varchar|50|default NULL|
|tupian|varchar|50|default NULL|
|yishengrenshu|varchar|50|default NULL|
|keshijianjie|varchar|50|default NULL|

表4-3：yaopinxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|yaopinmingcheng|varchar|50|default NULL|
|tupian|varchar|50|default NULL|
|guige|varchar|50|default NULL|
|shengchanshang|varchar|50|default NULL|
|shuliang|varchar|50|default NULL|
|jiage|varchar|50|default NULL|
|shengchanshang|varchar|50|default NULL|
|shuliang|varchar|50|default NULL|
|jiage|varchar|50|default NULL|
|yaopinxiangqing|varchar|50|default NULL|

表4-4 yisheng表

|列名|数据类型|长度|约束|
| :-: | :-: | - | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|yishenggonghao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|yishengxingming|varchar|50|default NULL|
|touxiang|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|lianxifangshi|varchar|50|default NULL|

`   `表4-5 yishengxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | - | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|yishenggonghao|varchar|50|default NULL|
|touxiang|varchar|50|default NULL|
|yishengxingming|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|yiling|varchar|50|default NULL|
|shanzhanglingyu|varchar|50|default NULL|
|keshimingcheng|varchar|50|default NULL|
|gerenjianjie|varchar|50|default NULL|




# 5统详细设计
## 5.1前台首页功能模块
宠物医院信息管理系统，在系统首页可以查看首页、医学知识、医生信息、药品信息、新闻资讯、留言反馈、我的、跳转到后台等内容，如图5-1所示。

![](/md/blog.017.png)

图5-1前台首页功能界面图



用户登录、用户注册，在注册页面可以填写用户名、密码、用户姓名、手机号码等信息进行注册、登录，如图5-2所

示。

![](/md/blog.018.png)

![](/md/blog.019.png)

图5-2用户注册、用户登录界面图
#########
个人中心，在个人中心页面通过填写用户名、密码、用户姓名、头像、性别、手机号码等信息进行更新信息、退出登录，如图5-3所示。在医生信息页面通过查看医生工号、头像、医生姓名、性别、医龄、擅长领域、科室名称、个人简介等信息进行预约挂号操作，如图5-4所示。

![](/md/blog.020.png)

图5-3个人中心界面图
#########
![](/md/blog.021.png)

图5-4医生信息界面图

## 5.2管理员功能模块
管理员登录，通过填写用户名、密码进行登录，如图5-5所示。

![](/md/blog.022.png)

图5-5管理员登录界面图

管理员登录进入宠物医院信息管理系统可以查看个人中心、用户管理、医生管理、医学知识管理、科室信息管理、医生信息管理、预约挂号管理、医嘱信息管理、药品信息管理、订单信息管理、留言板管理、系统管理等信息。

用户管理，在用户管理页面中可以通过查看用户名、用户姓名、头像、性别、手机号码等内容进行详情、修改、删除，如图5-6所示。还可以根据需要对医生管理进行详情，修改等详细操作，如图5-7所示。

![](/md/blog.023.png)

图5-6用户管理界面图

![](/md/blog.024.png)

图5-7医生管理界面图

医学知识管理，在医学知识管理页面中可以查看文章标题、图片、文章内容、发布日期等信息，并可根据需要对已有医学知识管理进行修改或删除等操作，如图5-8所示。

![](/md/blog.025.png)

图5-8医学知识管理界面图

科室信息管理，在科室信息管理页面中可以查看科室名称、图片、医生人数、科室简介等信息，并可根据需要对已有科室信息管理进行修改或删除等详细操作，如图5-9所示。

![](/md/blog.026.png)

图5-9科室信息管理界面图

医生信息管理，在医生信息管理页面中可以查看医生工号、头像、医生姓名、性别、医龄、擅长领域、科室名称、个人简介等内容，并且根据需要对已有医生信息管理进行详情，修改或删除等详细操作，如图5-10所示。

![](/md/blog.027.png)

图5-10医生信息管理界面图

轮播图；该页面为轮播图管理界面。管理员可以在此页面进行首页轮播图的管理，通过新建操作可在轮播图中加入新的图片，还可以对以上传的图片进行修改操作，以及图片的删除操作，如图5-11所示。

![](/md/blog.028.png)

图5-11轮播图管理界面图

订单信息管理，在订单信息管理页面中可以查看订单编号、药品名称、规格、生产商、数量、价格、总金额、用户名、用户姓名、是否支付等内容，并且根据需要对已有订单信息管理进行详情，修改或删除等详细操作，如图5-12所示。

![](/md/blog.029.png)

图5-12订单信息管理界面图


## 5.3医生功能模块
医生登录进入宠物医院信息管理系统可以查看个人中心、预约挂号管理、医嘱信息管理等内容。

预约挂号管理，在预约挂号管理页面中通过查看用户名、用户姓名、手机号码、宠物名、宠物状况、预约日期、医生工号、医生姓名、科室名称、是否审核、审核回复等信息，还可以根据需要对预约挂号管理进行修改，如图5-13所示。

![](/md/blog.030.png)

图5-13预约挂号管理界面图

医嘱信息管理，在医嘱信息管理页面中可以查看用户名、用户姓名、宠物名、宠物状况、医嘱、日期、医生工号、医生姓名、科室等信息，并且根据需要对已有医嘱信息管理进行查看删除等其他详细操作，如图5-14所示。

![](/md/blog.031.png)

图5-14医嘱信息管理界面图
#########
## 5.4用户功能模块
用户登录进入宠物医院信息管理系统可以查看个人中心、预约挂号管理、医嘱信息管理、订单信息管理等内容。

订单信息管理，在订单信息管理页面中通过查看订单编号、药品名称、规格、生产商、数量、价格、总金额、用户名、用户姓名、是否支付等信息，还可以根据需要对订单信息管理进行修改，如图5-15所示。

![](/md/blog.032.png)

图5-15订单信息管理界面图













