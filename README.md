# Spring Cloud Config

## config server / config client
- 配置文件的优先级  
`remote-spring.application.name.properties>remote-application.properties>local-application.properties`
- refresh 都做了什么？  
重新加载配置文件然后更新应用中的config bean；如果获取远程的配置文件失败，则配置没有任何变更（注意并不会直接使用本地的配置文件，除非重启应用并且没有配置Fail Fast）
- 安全问题

## TODO
- Push Notifications and Spring Cloud Bus

# Spring Cloud Zookeeper
- Service Discovery: instances can be registered with Zookeeper and clients can discover the instances using Spring-managed beans 服务发现：实例可以注册到 Zookeeper 同时客户端可以使用 Spring 管理的 bean 来发现这些实例
- Distributed Configuration: using Zookeeper as a data store 分布式配置： 使用 Zookeeper 来做数据存储
