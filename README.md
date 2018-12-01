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
  
### 详细的配置刚要地址

  https://springcloud.cc/spring-cloud-dalston.html#_spring_cloud_config
  
### config client 默认选项

  name : application  
  
  profile: default 
  
  label: master 
  
  默认选项为在master下寻找application-default格式的配置文件
  
  可以通过修改label 修改spring.application.name profile 作为读取配置文件的名称和后缀来选择读取哪个配置文件
  
### discovery
  
  当服务注册到eureka的时候，可以通过spring.cloud.config.discovery.enabled = true
  
  的方式去配置spring.cloud.config.discovery.service-id链接config服务器
  
  
  
  
  