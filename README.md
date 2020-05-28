## 项目说明
该项目为eureka微服务测试项目，主要实现的是maven-assembly打包该项目，
通过bin/文件夹下的shell脚本执行该程序。


### 本地启动注意
需要在启动参数中配置：
--spring.profiles.active=dev

### 服务端部署
拷贝target/eureka.zip进行部署
或者通过mvn assembly:assembly来打包成eureka.zip

使用：
```sbtshell
unzip eureka.zip
cd eureka
bin/start.sh
```

查看日志：
```sbtshell
tail -f logs/eureka.log
```
关闭
```sbtshell
bin/stop.sh
```


