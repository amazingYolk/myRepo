  原文地址：梁桂钊的博客<br>
  https://github.com/brianway/webporter.git<br>
  博客地址：blog.720ui.com<br>
  https://jsoup.org/download/packages/jsoup-1.13.1.jar<br>
  这里，笔者结合自己过往的面试经验，整理了一些核心的知识清单，帮助读者更好地回顾与复习 Java 服务端核心技术。本文会以引出问题为主，后面有时间的话，笔者陆续会抽些重要的知识点进行详细的剖析与解答。敬请关注「服务端思维」微信公众号，获取最新文章。
<br>
`基础篇`<br>
`基本功`
* 面向对象的特征
<br>final, finally, finalize 的区别
<br>int 和 Integer 有什么区别
<br>重载和重写的区别
<br>抽象类和接口有什么区别
	    	说说反射的用途及实现
<br>说说自定义注解的场景及实现
<br>HTTP 请求的 GET 与 POST 方式的区别
<br>session 与 cookie 区别
<br>session 分布式处理
<br>JDBC 流程
<br>MVC 设计思想
<br>equals 与 == 的区别
* 集合
<br>List 和 Set 区别
<br>List 和 Map 区别
<br>Arraylist 与 LinkedList 区别
<br>ArrayList 与 Vector 区别
<br>HashMap 和 Hashtable 的区别
<br>HashSet 和 HashMap 区别
<br>HashMap 和 ConcurrentHashMap 的区别
<br>HashMap 的工作原理及代码实现
<br>ConcurrentHashMap 的工作原理及代码实现
* 线程
<br>创建线程的方式及实现
<br>sleep() 、join（）、yield（）有什么区别
<br>说说 CountDownLatch 原理
<br>说说 CyclicBarrier 原理
<br>说说 Semaphore 原理
<br>说说 Exchanger 原理
<br>说说 CountDownLatch 与 CyclicBarrier 区别
<br>ThreadLocal 原理分析
<br>讲讲线程池的实现原理
<br>线程池的几种方式
<br>线程的生命周期
* 锁机制
<br>说说线程安全问题
<br>volatile 实现原理
<br>synchronize 实现原理
<br>synchronized 与 lock 的区别
<br>CAS 乐观锁
<br>ABA 问题
<br>乐观锁的业务场景及实现方式
`核心篇`
* 数据存储
<br>MySQL 索引使用的注意事项
<br>说说反模式设计
<br>说说分库与分表设计
<br>分库与分表带来的分布式困境与应对之策
<br>说说 SQL 优化之道
<br>MySQL 遇到的死锁问题
<br>存储引擎的 InnoDB 与 MyISAM
<br>数据库索引的原理
<br>为什么要用 B-tree
<br>聚集索引与非聚集索引的区别
<br>limit 20000 加载很慢怎么解决
<br>选择合适的分布式主键方案
<br>选择合适的数据存储方案
<br>ObjectId 规则
<br>聊聊 MongoDB 使用场景
<br>倒排索引
<br>聊聊 ElasticSearch 使用场景
* 缓存使用
<br>Redis 有哪些类型
<br>Redis 内部结构
<br>聊聊 Redis 使用场景
<br>Redis 持久化机制
<br>Redis 如何实现持久化
<br>Redis 集群方案与实现
<br>Redis 为什么是单线程的
<br>缓存奔溃
<br>缓存降级
<br>使用缓存的合理性问题
* 消息队列
<br>消息队列的使用场景
<br>消息的重发补偿解决思路
<br>消息的幂等性解决思路
<br>消息的堆积解决思路
<br>自己如何实现消息队列
<br>如何保证消息的有序性
`框架篇`
* Spring
<br>BeanFactory 和 ApplicationContext 有什么区别
<br>Spring Bean 的生命周期
<br>Spring IOC 如何实现
<br>说说 Spring AOP
<br>Spring AOP 实现原理
<br>动态代理（cglib 与 JDK）
<br>Spring 事务实现方式
<br>Spring 事务底层原理
<br>如何自定义注解实现功能
<br>Spring MVC 运行流程
<br>Spring MVC 启动流程
<br>Spring 的单例实现原理
<br>Spring 框架中用到了哪些设计模式
<br>Spring 其他产品（Srping Boot、Spring Cloud、Spring Secuirity、Spring Data、Spring AMQP 等）
* Netty
<br>为什么选择 Netty
<br>说说业务中，Netty 的使用场景
<br>原生的 NIO 在 JDK 1.7 版本存在 epoll bug
<br>什么是TCP 粘包/拆包
<br>TCP粘包/拆包的解决办法
<br>Netty 线程模型
<br>说说 Netty 的零拷贝
<br>Netty 内部执行流程
<br>Netty 重连实现
`微服务篇`
* 微服务
<br>前后端分离是如何做的
<br>微服务哪些框架
<br>你怎么理解 RPC 框架
<br>说说 RPC 的实现原理
<br>说说 Dubbo 的实现原理
<br>你怎么理解 RESTful
<br>说说如何设计一个良好的 API
<br>如何理解 RESTful API 的幂等性
<br>如何保证接口的幂等性
<br>说说 CAP 定理、 BASE 理论
<br>怎么考虑数据一致性问题
<br>说说最终一致性的实现方案
<br>你怎么看待微服务
<br>微服务与 SOA 的区别
<br>如何拆分服务
<br>微服务如何进行数据库管理
<br>如何应对微服务的链式调用异常
<br>对于快速追踪与定位问题
<br>微服务的安全
* 分布式
<br>谈谈业务中使用分布式的场景
<br>Session 分布式方案
<br>分布式锁的场景
<br>分布是锁的实现方案
<br>分布式事务
<br>集群与负载均衡的算法与实现
<br>说说分库与分表设计
<br>分库与分表带来的分布式困境与应对之策
<br>安全问题
<br>安全要素与 STRIDE 威胁
<br>防范常见的 Web 攻击
<br>服务端通信安全攻防
<br>HTTPS 原理剖析
<br>HTTPS 降级攻击
<br>授权与认证
<br>基于角色的访问控制
<br>基于数据的访问控制
<br>性能优化
<br>性能指标有哪些
<br>如何发现性能瓶颈
<br>性能调优的常见手段
<br>说说你在项目中如何进行性能调优
`工程篇`
* 需求分析
<br>你如何对需求原型进行理解和拆分
<br>说说你对功能性需求的理解
<br>说说你对非功能性需求的理解
<br>你针对产品提出哪些交互和改进意见
<br>你如何理解用户痛点
* 设计能力
<br>说说你在项目中使用过的 UML 图
<br>你如何考虑组件化
<br>你如何考虑服务化
<br>你如何进行领域建模
<br>你如何划分领域边界
<br>说说你项目中的领域建模
<br>说说概要设计
* 设计模式
<br>你项目中有使用哪些设计模式
<br>说说常用开源框架中设计模式使用分析
<br>说说你对设计原则的理解
<br>23种设计模式的设计理念
<br>设计模式之间的异同，例如策略模式与状态模式的区别
<br>设计模式之间的结合，例如策略模式+简单工厂模式的实践
<br>设计模式的性能，例如单例模式哪种性能更好。
* 业务工程
<br>你系统中的前后端分离是如何做的
<br>说说你的开发流程
<br>你和团队是如何沟通的
<br>你如何进行代码评审
<br>说说你对技术与业务的理解
<br>说说你在项目中经常遇到的 Exception
<br>说说你在项目中遇到感觉最难Bug，怎么解决的
<br>说说你在项目中遇到印象最深困难，怎么解决的
<br>你觉得你们项目还有哪些不足的地方
<br>你是否遇到过 CPU 100% ，如何排查与解决
<br>你是否遇到过 内存 OOM ，如何排查与解决
<br>说说你对敏捷开发的实践
<br>说说你对开发运维的实践
<br>介绍下工作中的一个对自己最有价值的项目，以及在这个过程中的角色
`软实力`
<br>说说你的亮点
<br>说说你最近在看什么书
<br>说说你觉得最有意义的技术书籍
<br>工作之余做什么事情
<br>说说个人发展方向方面的思考
<br>说说你认为的服务端开发工程师应该具备哪些能力
<br>说说你认为的架构师是什么样的，架构师主要做什么
<br>说说你所理解的技术专家
<br>（完）

1. 什么是 spring cloud？  一系列微服务框架的集合，包括服务的注册与发现，服务的配置中心，服务的治理--负载均衡，熔断，数据监控，这一系列的框架都可以用spring boot的开发风格做到一键启动和部署 
2. spring cloud 熔断器的作用是什么？ 服务故障之后，通过熔断器监控到以后向调用方返回一个错误响应，而不是长时间的等待，避免了线程因调用故障服务被长时间占用不释放，避免故障在分布式系统中的蔓延，形成雪崩
3. spring cloud 的核心组件有哪些？ zuul，eureka，ribbon，feign，hystrix
4. SpringCloud和Dubbo 从技术选型上讲，从rest和rpc上对比，从文档质量和社区活跃度讲。dubbo实现了服务治理，而springcloud则实现了众多的包括服务注册发现，服务治理，配置中心等，调用方式一个是rpc调用一个是 rest api；dubbo本身没有实现服务网关，只是通过第三方技术整合，而springcloud拥有zuul网关作为路由服务器。
5. Springboot和SpringCloud  springboot是专注于快速，方便地开发单个的微服务个体，Springcloud关注全局的服务治理框架。
6. 微服务之间是如何独立通讯的   rpc 消息队列 rabbitMQ
7. 负载均衡的意义是什么? 改善计算机群体，网络连接，中央处理单元或者磁盘驱动器等多种计算资源的工作负载分布。负载均衡旨在优化资源使用，最大吞吐量，最小响应时间并避免任何单一资源的过载。使用多个组件进行负载均衡而不是单个组件可能会通过冗余来提高可靠性和可用性。负载均衡通常涉及专业软件或硬件，例如多重交换机或域名系统服务进程
8. springcloud如何实现服务的注册?  服务发布时，指定对应的服务名，将服务注册到注册中心（eureka zookeeper），注册中心加@EnableEurekaServer，服务用@EnableDiscoveryClient，然后用ribbon或feign进行服务直接的调用发现
9. 什么是服务熔断?什么是服务降级  微服务架构下，各种原因会导致服务的阻塞，在高并发场景下，服务的阻塞意味着线程的阻塞，导致当前线程不可用，服务器的线程全部阻塞，导致服务器崩溃，由于服务之间的调用是同步的，会对整个微服务系统造成服务雪崩    所以服务熔断就是将某个故障的服务切断，并返回错误的结果，避免服务阻塞；服务降级是当服务器压力剧增的情况下，根据实际情况及流量，对一些服务和页面有策略的不处理或换种简单的方式处理，从而释放服务器资源以保证核心交易正常运转或高效运作。换句话说就是服务器压力剧增时，将一些服务不处理或者简单处理，然另一些服务正常运作或者高速运作
10. 微服务的优缺点分别是什么?说下你在项目开发中碰到的坑  优缺点，服务耦合性低，具有功能意义的服务；代码量低，开发效率提高；一个服务只做一件事，微服务能够被小团体单独开发；面向接口编程，可以用不同语言开发；易于第三方集成；微服务只是业务逻辑的代码，不会与html，css或者其他页面结合；前后端分离或者全栈；可以灵活搭配，连接公共库/连接独立库；             缺点：服务数量增多，管理维护成本压力增大；  数据的一致性系统部署依赖。
11. 你所知道的微服务技术栈？
12.Eureka和ZooKeeper都可以提供服务注册与发现的功能,请说说两个的区别？eureka：保证的是可用性、分区容错性和最终一致性，zookeeper保证的一致性和分区容错性；eureka的各个节点平等，而dubbo拥有leader节点和follower节点；eureka拥有自我保护机制解决分区问题，dubbo拥有半数存活原则；eureka是一个工程，zookeeper只是一个进程
13. eureka自我保护机制是什么?  eureka server节点在短时间内丢失过多实例的连接（网络故障或频繁启动关闭客户端），节点会进入自我保护机制，保护注册信息，不会删除注册数据，故障恢复时，自动退出自我保护机制
14. 什么是Ribbon？ 负载均衡客户端，feign默认集成ribbon
15. 什么是feigin？它的优点是什么？  整合了ribbon和hystrix，基于接口的注解。添加依赖，开启注解启动@EnableFeignClients；定义接口@FeignClient（name=""）指定调用的服务
16. Ribbon和Feign的区别？  ribbon需要自己构建http请求，模拟请求然后使用resttemplate发送给其他服务，步骤繁琐；feign需要将调用的方法定义成抽象方法即可。
17. 什么是Spring Cloud Bus?   将分布式的节点用轻量级的消息代理连接起来，可以用于广播配置文件的更改或者服务直接通讯，也可以用于监控。如果修改了配置文件，发送一次请求，所有客户端会重新读取配置文件。添加依赖，配置rabbitmq
18. 什么是Hystrix?   熔断器，服务熔断，依赖隔离，服务监控，服务降级
19. springcloud断路器作用?  全开，半开，关闭。  全开，一段时间达到一定次数无法调用并且多次监控没有恢复的迹象，熔断器完全打开，下次请求就一定请求不到服务。半开：短时间内有恢复的迹象，发送部分请求到服务，若服务正常则断路器关闭；关闭：服务正常使用
20. 什么是SpringCloudConfig?  分布式服务众多，为了统一管理配置文件，实时更新，所以需要分布式配置中心组件。在springcloud中，spring cloud config的作用是支持配置服务的内存中（即本地），也支持在远程git仓库中。有config server 和config client。使用，添加依赖，配置文件添加相关配置，启动类添加注解@EnableConfigServer
21. 架构？  服务的注册与发现，服务消费，负载均衡，熔断器，路由网关，配置管理。    常见的负载均衡是，客户端的请求首先经过负载均衡（zuul、ngnix），再到路由网关（zuul集群），然后再到具体的服务，服务统一注册到高可用的服务注册中心集群，服务的所有配置文件有配置服务管理，配置服务的配置文件放在git仓库，方便随时修改。

rpc和rest api：rpc的缺点就是服务之间耦合性太高，每一个微服务都需要定义一个接口，并通过持续继承发布，需要严格的版本控制，否则会出现服务提供方和调用方因为版本而产生冲突。


什么是微服务：微服务 就是一种架构模式或者架构风格，是将一个单体应用拆分成不同的服务，每个服务围绕具体的业务逻辑进行构建，服务之间通过http rest api或者rpc进行通信，单个服务可以独立地运行在自己的进程中，并能独立地部署到测试环境生产环境
