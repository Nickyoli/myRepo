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
