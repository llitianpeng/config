### git配置的映射方式

  /{application}/{profile}[/{label}]
  
  /{application}-{profile}.yml
  
  /{label}/{application}-{profile}.yml
  
  /{application}-{profile}.properties
  
  /{label}/{application}-{profile}.properties
  
### application

  application即spring.application.name的属性值
  
### label
  
  label为分支名称或者当前配置文件所在目录,默认为master

### profile
  
  profile为文件的后缀
  
### config client 默认选项

  name : application  
  
  profile: default 
  
  label: master 
  
  默认选项为在master下寻找application-default格式的配置文件
  
  可以通过修改label 修改spring.application.name profile 作为读取配置文件的名称和后缀来选择读取哪个配置文件
  
### discovery
  
  当服务注册到eureka的时候，可以通过spring.cloud.config.discovery.enabled = true
  
  的方式去配置spring.cloud.config.discovery.service-id链接config服务器
  
### 快速异常

  在config客户端连接config服务器出错的时候,不希望他继续启动，可以通过
  
  spring.cloud.config.failFast = true 来开启快速异常
  
### 详细的配置刚要地址

  https://springcloud.cc/spring-cloud-dalston.html#_spring_cloud_config
  
### 安全认证

  通过在config server 配置 security.user.name 和 security.user.password 的方式并注入spring-boot-starter-security的安全组件
  
  在config client中 设置 spring.cloud.config.username 和 spring.cloud.config.password属性对访问config server的客户端进行安全认证
  
  
  
  
  