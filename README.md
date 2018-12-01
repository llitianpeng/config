### git配置的映射方式

  /{application}/{profile}[/{label}]
  
  /{application}-{profile}.yml
  
  /{label}/{application}-{profile}.yml
  
  /{application}-{profile}.properties
  
  /{label}/{application}-{profile}.properties
  
  application即spring.application.name的属性值
  
  label为分支名称或者当前配置文件所在目录,默认为master
  
  profile为文件的后缀
  