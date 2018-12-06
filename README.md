# cat-movie
慕课网仿猫眼项目源码
## 1
传统应用带来的问题：
- 单一业务开发和迭代困难
- 扩容困难
- 部署和回滚困难

微服务概述：
- 微服务是一种将业务系统进一步拆分的架构风格
- 微服务强调每个业务都独立运行
- 每个单一服务都应该使用更轻量的机制保持通信
- 服务不强调环境，可以不同语言或数据源

## 2 演示环境构建
#### 安装zookeeper
zookeeper 3.4.10
解压，修改conf/zoo_sample.cfg为zoo.cfg
bin/zkServer.sh 启动

#### 配置zookeeper
添加zkclient依赖，配置：
spring:
  dubbo:
    registry: zookeeper://118.126.111.144:2181

## 3

