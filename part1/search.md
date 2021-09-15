

> 在淘宝搜索“手机”，后台发生了什么？淘宝的用户量比较大，所以不可能是很简单后台查询数据库，然后响应数据。

# 后台响应数据的流程

1. 域名解析，获取到淘宝的IP（负载均衡服务器）。
2. 通过负载均衡服务器与应用程序集群建立连接，发送HTTP请求。
3. 应用程序负载均衡服务器，选择应用服务器处理该请求。
4. 应用服务器查询缓存，有缓存则返回缓存。没有缓存则通过Elasticsearch进行全文检索，然后查询数据库生成数据，响应请求 





# DNS（Domain Name System)
+ 根据地理位置返回IP
+ hosts



# 负载均衡
+ IOS七层网络模型
+ 四层负载均衡
+ 七层负载均衡
+ TCP/IP协议
+ 反向代理缓存

# 应用服务器集群

+ 应用服务器集群
+ 中台和微服务
+ 服务间通信
+ 服务注册、发现
+ ApiGateway


# 缓存
+ redis
+ 分布式一致性Hash算法
+ 分布式一致性算法（Raft、Zab）
+ CAP



# Elasticsearch
+ 倒排索引



# MySQL
+ 主从集群
+ 主主集群
+ 数据分片



# CDN（Content Delivery Network）
+ cdn -- 内容分发网络



# 消息队列
+ Kafka
+ RebbitMQ

# 文件服务
+ 动静分离

# 参考资料
- [负载均衡、TCP/IP、LVS 学习总结](https://blog.csdn.net/qq_38282454/article/details/101271916)
- [LVS+Nginx为什么会被同时使用](https://blog.csdn.net/qq_25188255/article/details/117465191)
- [在京东搜索一个“TT”，后台发生了什么？](https://mp.weixin.qq.com/s?__biz=MzI2NjI5MzU2Nw==&mid=2247514075&idx=1&sn=30575b69841c528a0c3219f13be6f03f)