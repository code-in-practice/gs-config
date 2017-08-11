# gs-config

## config service
- 配置文件的优先级  
`remote-spring.application.name.properties>remote-application.properties>local-application.properties`
- refresh 都做了什么？  
重新加载配置文件然后更新应用中的config bean；如果获取远程的配置文件失败，则配置没有任何变更（注意并不会直接使用本地的配置文件，除非重启应用）
