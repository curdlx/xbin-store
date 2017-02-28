## xbin-store

分布式商城项目

### 2017年01月24日15:44:59 完成项目搭建
> xbin-store-common、xbin-store-common-config、xbin-store-common-mapper、xbin-store-common-pojo、xbin-store-service-manager、xbin-store-service-manager-api、xbin-store-web-manager

### 2017年01月24日23:26:27 完成dubbo的rest和dubbo服务的测试 完成商品列表的展示
今天遇到的问题：
* MyBatis自动生成选择全部表——> %
* Dubbo消费端没有配置应用名和ZooKeeper地址
* Dubbo以Jar方式启动要配置Spring的配置文件路径
* POJO使用序列化kryo一定得实现Serializable接口
* web.xml配置的只加载一个Spring配置文件 一定要注意<import/>其他全部配置

### 2017年01月27日00:26:52 完成商品分类选择、上传图片、商品添加功能
今遇到的问题：
* dubbo服务发布问题 IDEA 配置错误 没有把service服务本身进行maven install操作
* FastDFS的配置文件必须在引用工具的工程中配置文件
* dubbo返回对象**一定要实现Serializable接口**
* FastDFS抽风 问题不清楚

### 2017年02月03日13:27:56 完成商品首页搭建
### 2017年02月03日16:52:52 完成首页大广告展示、Redis缓存服务工程搭建
### 2017年02月03日23:46:23 添加事务
### 2017年02月05日02:26:32 完成search服务 完成商品搜索功能
### 2017年02月05日16:27:22 修改log4j配置文件 增加全局异常处理器
### 2017年02月05日23:46:56 使用ActiveMQ完成添加商品时 Solr索引同步
### 2017年02月06日17:07:52 完成Item Web工程的搭建 item Service工程搭建 拆分 Manager工程 新建 Portal Service 工程 完成商品展示 缓存
### 2017年02月06日17:07:15 完成页面静态化
### 2017年02月06日23:23:12 修改BUG 服务名称错误
### 2017年02月07日16:45:11 修改Maven打包错误 Dubbo增加Host配置
### 2017年02月09日01:19:59 完成用户登录
### 2017年02月09日21:01:37 新建Notify Service服务 完成注册服务的 用户名、邮箱、手机号查重 推荐命名 验证码验证 手机验证码验证
### 2017年02月10日00:42:56 完成注册
### 2017年02月10日23:03:12 完成首页页面展示 功能未完成 完成Cart Service API Web工程的创建
### 2017年02月11日22:09:59 创建Admin Web API Service 工程
### 2017年02月13日22:40:43 创建Admin Web API Service 工程 完成搜索页面的替换
### 2017年02月14日23:31:21 完成首页导航数据导入
### 2017年02月15日22:59:24 完成首页大广告保存数据库
### 2017年02月16日20:45:32 保存item js和css
### 2017年02月20日21:17:12 完成商品一级分类编辑保存页面
### 2017年02月20日21:37:10 完成商品一级分类编辑保存
### 2017年02月21日16:14:19 完成商品二级分类编辑保存
### 2017年02月22日19:28:21 完成商品加入购物车
### 2017年02月22日19:38:23 购物车查询商品添加缓存
### 2017年02月24日21:54:54 完成订单跳转 拦截
### 2017年02月26日21:15:31 完成购物车功能
### 2017年02月26日21:37:19 完成购物车功能 之前手残覆盖源代码 哎
### 2017年02月28日21:11:03 完成Order页面提交 修改数据库及重新生成POJO Bug SSO系统有漏洞 待修复

### 命名规范(自己总结)
* 父工程 xx
    * xx-common
    * xx-common-config
    * xx-common-mapper
    * xx-common-pojo
    * xx-service-yy-api
    * xx-service-yy
    * xx-web-yy
    * ......

# 机器ip情况(本机)
### 需要联网
### 不需要联网
* Zookeeper1 192.168.125.128
* FastDFS 192.168.125.129
* Solr 192.168.125.131
* FastDFS 192.168.125.132
* Redis 192.168.125.133