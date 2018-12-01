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
  
### 默认选项

  name : application
  
  profile: default
  
  label: master
  
  默认选型为在master分支下寻找application-default格式的配置文件
  
  可以通过修改master分支名称 修改name profile 作为读取配置文件的名称和后缀来选择读取哪个配置文件
  
  
  
  
  