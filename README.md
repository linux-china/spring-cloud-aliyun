Spring Cloud for Aliyun Cloud Services
======================================
将Aliyun提供的云服务整合到Spring Cloud中，方便最终用户开发


### 如何使用
在你的Spring Boot应用中的pom.xml的dependency management中添加对spring-cloud-aliyun-dependencies的依赖
接下来就是引入对应的starter，如spring-cloud-starter-aliyun-jdbc, spring-cloud-starter-aliyun-sms，
接下来在application.properties响应的配置如下：
```properties
    cloud.aliyun.credentials.accessKey=xxxx
    cloud.aliyun.credentials.secretKey=yyyy
```

最后调用指定的服务即可，如下:
```groovy
   @Autowired
   SmsService smsService;
```

### 服务列表

* RDS
* SMS
* ...
  
