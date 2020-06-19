# SpringCloudLearn
* Spring Cloud 整体架构概览
* Spring Cloud Eureka：服务注册与发现
* Spring Cloud Ribbon：负载均衡的服务调用
* Spring Cloud Hystrix：服务容错保护
* Hystrix Dashboard：断路器执行监控
* Spring Cloud OpenFeign：基于Ribbon和Hystrix的声明式服务调用
* Spring Cloud Zuul：API网关服务
* Spring Cloud Config：外部集中化配置管理
* Spring Cloud Bus：消息总线
* Spring Cloud Sleuth：分布式请求链路跟踪
* Spring Cloud Consul：服务治理与配置中心
* Spring Cloud Gateway：新一代API网关服务
* Spring Boot Admin：微服务应用监控
* Spring Cloud Security：Oauth2使用入门
* Spring Cloud Security：Oauth2结合JWT使用
* Spring Cloud Security：Oauth2实现单点登录
* Spring Cloud Alibaba：Nacos 作为注册中心和配置中心使用
* Spring Cloud Alibaba：Sentinel实现熔断与限流
* 使用Seata彻底解决Spring Cloud中的分布式事务问题
* IDEA中创建和启动SpringBoot应用的正确姿势
# 项目结构
springCloudLearn
├── eureka-server -- eureka注册中心
├── eureka-security-server -- 带登录认证的eureka注册中心
├── eureka-client -- eureka客户端
├── user-service -- 提供User对象CRUD接口的服务
├── ribbon-service -- ribbon服务调用测试服务
├── hystrix-service -- hystrix服务调用测试服务
├── turbine-service -- 聚合收集hystrix实例监控信息的服务
├── hystrix-dashboard -- 展示hystrix实例监控信息的仪表盘
├── feign-service -- feign服务调用测试服务
├── zuul-proxy -- zuul作为网关的测试服务
├── config-server -- 配置中心服务
├── config-security-server -- 带安全认证的配置中心服务
├── config-client -- 获取配置的客户端服务
├── consul-config-client -- 用于演示consul作为配置中心的consul客户端
├── consul-user-service -- 注册到consul的提供User对象CRUD接口的服务
├── consul-service -- 注册到consul的ribbon服务调用测试服务
├── api-gateway -- gateway作为网关的测试服务
├── admin-server -- admin监控中心服务
├── admin-client -- admin监控中心监控的应用服务
├── admin-security-server -- 带登录认证的admin监控中心服务
├── oauth2-server -- oauth2认证测试服务
├── oauth2-jwt-server -- 使用jwt的oauth2认证测试服务
├── oauth2-client -- 单点登录的oauth2客户端服务
├── nacos-config-client -- 用于演示nacos作为配置中心的nacos客户端
├── nacos-user-service -- 注册到nacos的提供User对象CRUD接口的服务
├── nacos-ribbon-service -- 注册到nacos的ribbon服务调用测试服务
├── sentinel-service -- sentinel功能测试服务
├── seata-order-service -- 整合了seata的订单服务
├── seata-storage-service -- 整合了seata的库存服务
└── seata-account-service -- 整合了seata的账户服务
