Feign的常用配置
====
* 日志级别
    * NONE：默认的，不显示任何日志；
    * BASIC：仅记录请求方法、URL、响应状态码及执行时间；
    * HEADERS：除了BASIC中定义的信息之外，还有请求和响应的头信息；
    * FULL：除了HEADERS中定义的信息之外，还有请求和响应的正文及元数据。

* Feign自己的配置
    ```
    feign:
      hystrix:
        enabled: true #在Feign中开启Hystrix
      compression:
        request:
          enabled: false #是否对请求进行GZIP压缩
          mime-types: text/xml,application/xml,application/json #指定压缩的请求数据类型
          min-request-size: 2048 #超过该大小的请求会被压缩
        response:
          enabled: false #是否对响应进行GZIP压缩
    logging:
      level: #修改日志级别
        com.macro.cloud.service.UserService: debug
    ```
* Feign中的Ribbon配置
在Feign中配置Ribbon可以直接使用Ribbon的配置

* Feign中的Hystrix配置
在Feign中配置Hystrix可以直接使用Hystrix的配置