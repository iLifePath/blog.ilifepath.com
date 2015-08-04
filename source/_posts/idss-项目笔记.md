title: iDSS 项目笔记
date: 2015-08-03 15:43:36
categories: 项目
tags:
  - iDSS
  - 项目
  - 笔记
---
![](http://7xjra2.com1.z0.glb.clouddn.com/junggle.jpg)

### 创业扶持
- aws 创业支持计划
- 七牛创业扶持计划

### 问题
- 标签化，可输入

### 市场
- 品牌合作
    - 特斯拉试驾
    - 大疆
    - 职业网站
- 聚乐部合作
    - 飞机试乘
    - 滑翔伞
    - 热气球
    - 海上垂钓，帆船，航海
    - 空降
    - 航模，无人机
- 事件营销
    - 冥王星时刻
    - 地球2.0
    - 船来了
- 文案
    - 相信的人都玩过了，不相信的人也来玩玩吧？只有相信的人玩过数据不准哦

<!-- more -->

### business model
- keepsake
- brand exhibition
- cooperation
- personalized service data provider


### cache architecture
- client:
    - http cache: etag, last-modified, cache-control
- server:
    - dynamic to static: rails default, nginx + lua
    - centrelized session: memcached
- application:
    - page cache
    - action cache
    - segment cache
- persistent:
    - object cache
    - query cache

### architecture
- rails container: passenger, puma, unicorn, mongrel
- cache: memcached, squid, vanish
- rails + memcached: gem 'dalli'
- rails inner cache: cache-money
- deployment: Capistrano
- 集群 session 同步：
    - 客户端 session，例如 cookie，数据量小
    - session 复制(tomcat,jboss)，广播风暴
    - 粘性 session
    - 数据库 session，开销大
    - 共享存储
    - memcached
    - terracott, session 专用工具

### stress test
- ab, siege, Web-CT, pylot

### sns share sdk
- ShareSDK/Mob, Baidu Share, JiaThis, bShare
- getsitecontrole

### 政策
- 零申报/无票/0 declare：没有应税收入，也没有应纳税额
- 核定税种，税种时限，激活税种
- 工商年检
- 企业核税，需要交印花税，注册资金的万分之五

### 公司
- 名称
    - 名字：止观，慧观，翌观，紫冠，之冠，致观
    - 天文：星环，光环[#]，彗星，流星，织女星[√]，太阳风[x]，天琴座[x]，月光，星云[#]，深空[√]，比邻星[x]，主序星，耀斑，光晕[√]，聚星[x]，猎户座[x]，旋臂[√]，光晕[]，繁星[x]，阵列
    - 物理：量子，重力，波动，光电，光子，光量子，引力波，统一场，光谱，三棱镜，棱镜[√]，以太，宇观[√]，折射，夸克，光帆[√]，黑洞[√]，虫洞[#]，单摆，费米，哈勃，佯谬
    - 计算机：图灵，弹性计算，决策支持，人工智能，大数据，决策树，熵，全栈，攻城狮，节点[#]
    - 地理：彩虹[x]，云图[x]，极光[x]，彩云[x]，港湾[x]，海湾[x]，雪浪，风雨彩虹[x]，天虹[x]，彩霞[x]，喷泉[√]，赤道[√]
    - 航空：湍流[√]，激波，涡流[√]
    - 数学：七桥，矩阵[x]，柯西，欧拉，黎曼，七巧板[√]，象限
    - 科幻：智子[#]，红岸，光粒[√]，星门[x]，明日科技，星舰，星船，深渊[#]，天眼[#]，天梯[#]，天渊，心灵[√]，天网[#]，心理历史，心灵史，心矢，基地，Psychohistory，心历
    - 文学：知你[√]，蓝色空间[x]，初心[√]，广寒宫，仰望深渊，嫦娥，天宫
    - 音乐：田园[x]，风铃[#]
    - 地名：美兰[x]
    - 化学：元素[x]
    - 植物：杏叶[√]，枫叶[x]，红豆[x]
    - 动物：羊羔，虎斑猫[√]，小花猫
    - 军事：小鹰[√]，战隼[√]，鹰狮[√]，旋风[x]，战斧，三叉戟，大黄蜂[x]
    - 么么哒：萌猫[√]，猫咪[√]，喵喵[*]，咪咪[√]，喵咪[#]，奶猫[√]，么么哒[√]，萌萌哒[√]，喵星人[√]，萌喵[√]，小强[√]，大虾[√]
    - 含义：数海，观数，观信
- 核名：
    - 彩虹，么么哒，萌萌哒，咪咪，喵喵，么么嗒
    - 光帆，织女星，七桥
    - 萌萌的，萌萌滴，萌萌哒，萌哒哒，心灵矢，心灵使，心使，心矢，心历，心灵史，心史，止观，止观，慧观，紫冠，之冠，致观，光晕，咪咪，喵喵，猫咪，萌猫，喵星人，萌喵，极光，光帆，织女星，七桥，星环，智子，红岸，光粒，棱镜，星门，小强，大虾，费米，哈勃，天眼，天梯，天渊，星环，旋臂，智子，风铃
- 行业名：上海xxx网络科技有限公司 （我考虑还是改用“网络科技”，不用“信息科技”了）
- 主营范围：互联网信息，电子商务，数据处理与分析，信息系统集成，信息咨询，系统研发，网站建设

### 主题
- 星座
- 现代名人
- 古代名人
- 字谜：王字去掉一笔
- 富人思维，穷人思维

### 渠道
- 主流 SNS: 微信朋友圈, 微博, QQ 空间, 人人
- 微型订阅号：《为什么要做神秘主义验证》《为什么要做心理模型验证》
- 群: QQ 群, 微信群
- 知乎（制造话题争议）
- 百度
    - 百度百科：“星座熵”，“神秘主义验证”，“人格熵”，“神秘主义数据化”
    - 百度问答：《星座到底多靠谱》《神秘主义能数据化嘛》
- 豆瓣
- 论坛：天涯论坛科技板块
- 视频传播
- linkedin, facebook, google+, twitter
- youku, youtube, github
- bootcss 优站 http://expo.bootcss.com/，提交地址 youzhan@bootcss.com
- bestsdk.com 运营推广板块 http://www.bestsdk.com/forum/lists/7.html
- http://www.devstore.cn/
- http://www.demo8.com/
- 小媒体
    - http://www.hrtechchina.com/
    - http://www.kejik.com/

### 策划
- 星座本身就存在争议
- 怎样寻找噱头
- 怎样利用争议
- 除了星座，还有什么其他有争议的话题？中医？能否利用？
- 还有什么主题是符合“社会实验”提法的？
- X 型文案，Y 型文案
- 微信公众号

### question
- 为什么没有人提盈利问题？
- 第一波需要注册制嘛？

### R-Ruby
- RinRuby, RSRuby
- rApache, Rook
- Rserve,

### 发散
- 大数据，云计算，移动互联网，决策支持
- 对撞机，天空实验室，望远镜，太空船
- 无穷大，幂
- 人生，抉择
- 光环
