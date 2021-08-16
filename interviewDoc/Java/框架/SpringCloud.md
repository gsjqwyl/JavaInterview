**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [什么是微服务？](#%E4%BB%80%E4%B9%88%E6%98%AF%E5%BE%AE%E6%9C%8D%E5%8A%A1)
- [什么是微服务架构？](#%E4%BB%80%E4%B9%88%E6%98%AF%E5%BE%AE%E6%9C%8D%E5%8A%A1%E6%9E%B6%E6%9E%84)
- [使用Spring Cloud有什么优势？](#%E4%BD%BF%E7%94%A8spring-cloud%E6%9C%89%E4%BB%80%E4%B9%88%E4%BC%98%E5%8A%BF)
- [微服务的优缺点是什么？说下你在项目中碰到的坑。](#%E5%BE%AE%E6%9C%8D%E5%8A%A1%E7%9A%84%E4%BC%98%E7%BC%BA%E7%82%B9%E6%98%AF%E4%BB%80%E4%B9%88%E8%AF%B4%E4%B8%8B%E4%BD%A0%E5%9C%A8%E9%A1%B9%E7%9B%AE%E4%B8%AD%E7%A2%B0%E5%88%B0%E7%9A%84%E5%9D%91)
- [微服务的优点缺点?说下开发项目中遇到的坑?](#%E5%BE%AE%E6%9C%8D%E5%8A%A1%E7%9A%84%E4%BC%98%E7%82%B9%E7%BC%BA%E7%82%B9%E8%AF%B4%E4%B8%8B%E5%BC%80%E5%8F%91%E9%A1%B9%E7%9B%AE%E4%B8%AD%E9%81%87%E5%88%B0%E7%9A%84%E5%9D%91)
- [SpringBoot和SpringCloud的区别？](#springboot%E5%92%8Cspringcloud%E7%9A%84%E5%8C%BA%E5%88%AB)
- [使用 Spring Cloud 有什么优势？](#%E4%BD%BF%E7%94%A8-spring-cloud-%E6%9C%89%E4%BB%80%E4%B9%88%E4%BC%98%E5%8A%BF)
- [服务注册和发现是什么意思？Spring Cloud 如何实现？](#%E6%9C%8D%E5%8A%A1%E6%B3%A8%E5%86%8C%E5%92%8C%E5%8F%91%E7%8E%B0%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9Dspring-cloud-%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0)
- [你所知道微服务的技术栈有哪些？列举一二。](#%E4%BD%A0%E6%89%80%E7%9F%A5%E9%81%93%E5%BE%AE%E6%9C%8D%E5%8A%A1%E7%9A%84%E6%8A%80%E6%9C%AF%E6%A0%88%E6%9C%89%E5%93%AA%E4%BA%9B%E5%88%97%E4%B8%BE%E4%B8%80%E4%BA%8C)
- [微服务之间如何独立通讯的?](#%E5%BE%AE%E6%9C%8D%E5%8A%A1%E4%B9%8B%E9%97%B4%E5%A6%82%E4%BD%95%E7%8B%AC%E7%AB%8B%E9%80%9A%E8%AE%AF%E7%9A%84)
- [REST 和RPC对](#rest-%E5%92%8Crpc%E5%AF%B9)
- [你所知道的微服务技术栈？](#%E4%BD%A0%E6%89%80%E7%9F%A5%E9%81%93%E7%9A%84%E5%BE%AE%E6%9C%8D%E5%8A%A1%E6%8A%80%E6%9C%AF%E6%A0%88)
- [Spring Cloud的版本关系](#spring-cloud%E7%9A%84%E7%89%88%E6%9C%AC%E5%85%B3%E7%B3%BB)
- [Spring Cloud的子项目（主要项目）](#spring-cloud%E7%9A%84%E5%AD%90%E9%A1%B9%E7%9B%AE%E4%B8%BB%E8%A6%81%E9%A1%B9%E7%9B%AE)
- [spring cloud 的核心组件有哪些](#spring-cloud-%E7%9A%84%E6%A0%B8%E5%BF%83%E7%BB%84%E4%BB%B6%E6%9C%89%E5%93%AA%E4%BA%9B)
- [springcloud如何实现服务的注册?](#springcloud%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E6%9C%8D%E5%8A%A1%E7%9A%84%E6%B3%A8%E5%86%8C)
- [什么是 Hystrix？它如何实现容错？](#%E4%BB%80%E4%B9%88%E6%98%AF-hystrix%E5%AE%83%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E5%AE%B9%E9%94%99)
- [什么是 Hystrix 断路器？我们需要它吗？](#%E4%BB%80%E4%B9%88%E6%98%AF-hystrix-%E6%96%AD%E8%B7%AF%E5%99%A8%E6%88%91%E4%BB%AC%E9%9C%80%E8%A6%81%E5%AE%83%E5%90%97)
- [Hystrix相关注解](#hystrix%E7%9B%B8%E5%85%B3%E6%B3%A8%E8%A7%A3)
- [什么是 Netﬂix Feign？它的优点是什么？](#%E4%BB%80%E4%B9%88%E6%98%AF-net%EF%AC%82ix-feign%E5%AE%83%E7%9A%84%E4%BC%98%E7%82%B9%E6%98%AF%E4%BB%80%E4%B9%88)
- [分布式配置中心能干嘛？](#%E5%88%86%E5%B8%83%E5%BC%8F%E9%85%8D%E7%BD%AE%E4%B8%AD%E5%BF%83%E8%83%BD%E5%B9%B2%E5%98%9B)
- [什么是Eureka](#%E4%BB%80%E4%B9%88%E6%98%AFeureka)
- [eureka自我保护机制是什么?](#eureka%E8%87%AA%E6%88%91%E4%BF%9D%E6%8A%A4%E6%9C%BA%E5%88%B6%E6%98%AF%E4%BB%80%E4%B9%88)
- [作为 务注册中心，Eureka比Zookeeper好在哪里?](#%E4%BD%9C%E4%B8%BA-%E5%8A%A1%E6%B3%A8%E5%86%8C%E4%B8%AD%E5%BF%83eureka%E6%AF%94zookeeper%E5%A5%BD%E5%9C%A8%E5%93%AA%E9%87%8C)
- [Eureka和zookeeper都可以提供服务注册与发现的功能，请说说两个的区别？](#eureka%E5%92%8Czookeeper%E9%83%BD%E5%8F%AF%E4%BB%A5%E6%8F%90%E4%BE%9B%E6%9C%8D%E5%8A%A1%E6%B3%A8%E5%86%8C%E4%B8%8E%E5%8F%91%E7%8E%B0%E7%9A%84%E5%8A%9F%E8%83%BD%E8%AF%B7%E8%AF%B4%E8%AF%B4%E4%B8%A4%E4%B8%AA%E7%9A%84%E5%8C%BA%E5%88%AB)
- [你所知道的微服务技术栈？](#%E4%BD%A0%E6%89%80%E7%9F%A5%E9%81%93%E7%9A%84%E5%BE%AE%E6%9C%8D%E5%8A%A1%E6%8A%80%E6%9C%AF%E6%A0%88)
- [使用Spring Cloud有什么优势？](#%E4%BD%BF%E7%94%A8spring-cloud%E6%9C%89%E4%BB%80%E4%B9%88%E4%BC%98%E5%8A%BF)
- [SpringBoot 和 SpringCloud 之间关系？](#springboot-%E5%92%8C-springcloud-%E4%B9%8B%E9%97%B4%E5%85%B3%E7%B3%BB)
- [SpringCloud 和 Dubbo 有哪些区别?](#springcloud-%E5%92%8C-dubbo-%E6%9C%89%E5%93%AA%E4%BA%9B%E5%8C%BA%E5%88%AB)
- [什么是Spring Cloud Config?](#%E4%BB%80%E4%B9%88%E6%98%AFspring-cloud-config)
- [什么是 zuul路由网关](#%E4%BB%80%E4%B9%88%E6%98%AF-zuul%E8%B7%AF%E7%94%B1%E7%BD%91%E5%85%B3)
- [什么是Ribbon？](#%E4%BB%80%E4%B9%88%E6%98%AFribbon)
- [Ribbon负载均衡能干什么？](#ribbon%E8%B4%9F%E8%BD%BD%E5%9D%87%E8%A1%A1%E8%83%BD%E5%B9%B2%E4%BB%80%E4%B9%88)
- [什么是feigin？它的优点是什么？](#%E4%BB%80%E4%B9%88%E6%98%AFfeigin%E5%AE%83%E7%9A%84%E4%BC%98%E7%82%B9%E6%98%AF%E4%BB%80%E4%B9%88)
- [Ribbon和Feign的区别？](#ribbon%E5%92%8Cfeign%E7%9A%84%E5%8C%BA%E5%88%AB)
- [什么是Spring Cloud Gateway?](#%E4%BB%80%E4%B9%88%E6%98%AFspring-cloud-gateway)
- [什么是 Hystrix？它如何实现容错？](#%E4%BB%80%E4%B9%88%E6%98%AF-hystrix%E5%AE%83%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E5%AE%B9%E9%94%99)
- [什么是 Hystrix 断路器？我们需要它吗？](#%E4%BB%80%E4%B9%88%E6%98%AF-hystrix-%E6%96%AD%E8%B7%AF%E5%99%A8%E6%88%91%E4%BB%AC%E9%9C%80%E8%A6%81%E5%AE%83%E5%90%97)
- [什么是 Netflix Feign？它的优点是什么？](#%E4%BB%80%E4%B9%88%E6%98%AF-netflix-feign%E5%AE%83%E7%9A%84%E4%BC%98%E7%82%B9%E6%98%AF%E4%BB%80%E4%B9%88)
- [什么是Spring Cloud Gateway?](#%E4%BB%80%E4%B9%88%E6%98%AFspring-cloud-gateway)
- [服务注册和发现是什么意思？Spring Cloud如何实现？](#%E6%9C%8D%E5%8A%A1%E6%B3%A8%E5%86%8C%E5%92%8C%E5%8F%91%E7%8E%B0%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9Dspring-cloud%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0)
- [负载平衡的意义什么？](#%E8%B4%9F%E8%BD%BD%E5%B9%B3%E8%A1%A1%E7%9A%84%E6%84%8F%E4%B9%89%E4%BB%80%E4%B9%88)
- [什么是熔断？什么是服务降级？](#%E4%BB%80%E4%B9%88%E6%98%AF%E7%86%94%E6%96%AD%E4%BB%80%E4%B9%88%E6%98%AF%E6%9C%8D%E5%8A%A1%E9%99%8D%E7%BA%A7)
- [什么是Netflix Feign？它的优点是什么？](#%E4%BB%80%E4%B9%88%E6%98%AFnetflix-feign%E5%AE%83%E7%9A%84%E4%BC%98%E7%82%B9%E6%98%AF%E4%BB%80%E4%B9%88)
- [什么是 Spring Cloud Bus？我们需要它吗？](#%E4%BB%80%E4%B9%88%E6%98%AF-spring-cloud-bus%E6%88%91%E4%BB%AC%E9%9C%80%E8%A6%81%E5%AE%83%E5%90%97)
- [微服务是如何对外提供统一接口的zuul具体使用](#%E5%BE%AE%E6%9C%8D%E5%8A%A1%E6%98%AF%E5%A6%82%E4%BD%95%E5%AF%B9%E5%A4%96%E6%8F%90%E4%BE%9B%E7%BB%9F%E4%B8%80%E6%8E%A5%E5%8F%A3%E7%9A%84zuul%E5%85%B7%E4%BD%93%E4%BD%BF%E7%94%A8)
- [Zuul 的过滤功能](#zuul-%E7%9A%84%E8%BF%87%E6%BB%A4%E5%8A%9F%E8%83%BD)

<!-- /TOC -->

### 什么是微服务？

> 单个轻量级服务一般为一个**单独微服务**，微服务讲究的是 专注某个功能的实现，比如登录系统只专注于用户登录方面功能的实现，讲究的是**职责单一，开箱即用，可以独立运行**。微服务架构系统是一个**分布式的系统**，按照业务进行划分服务单元模块，**解决单个系统的不足**，满足越来越**复杂的业务需求**。
>
> 马丁福勒（Martin Fowler）：就目前而言，对于微服务业界并没有一个统一的、标准的定义。但通常而言，微服务架构是一种架构模式或者说是架构风格，它提倡将单一应用程序划分成一组小的服务。每个服务运行在其独立的自己的进程中服务之间相互配合、相互协调，为用户提供最终价值。服务之间采用轻量级通信。每个服务都围绕具体业务进行构建，并能够独立部署到生产环境等。另外应尽量避免统一的、集中的服务管理机制。

通俗的来讲：

微服务就是一个独立的职责单一的服务应用程序。在 intellij idea 工具里面就是用maven开发的一个个独立的module，具体就是使用springboot 开发的一个小的模块，处理单一专业的业务逻辑，一个模块只做一个事情。

微服务强调的是服务大小，关注的是某一个点，具体解决某一个问题/落地对应的一个服务应用，可以看做是idea 里面一个 module。

比如你去医院：你的牙齿不舒服，那么你就去牙科。你的头疼，那么你就去脑科。一个个的科室，就是一个微服务，一个功能就是一个服务。



### 什么是微服务架构？

在前面你理解什么是微服务，那么对于微服务架构基本上就已经理解了。

微服务架构 就是 对微服务进行管理整合应用的。微服务架构 依赖于 微服务，是在微服务基础之上的。

**例如： **上面已经列举了什么是微服务。在医院里，每一个科室都是一个独立的微服务，那么 这个医院 就是 一个大型的微服务架构，就类似 院长 可以 对下面的 科室进行管理。微服务架构主要就是这种功能。



### 使用Spring Cloud有什么优势？

使用Spring Boot开发分布式微服务时，我们面临以下问题:

与分布式系统相关的复杂性-这种开销包括网络问题，延迟开销，带宽问题，安全问题。

服务发现-服务发现工具管理群集中的流程和服务如何查找和互相交谈。它涉及一个服务目录，在该目录中注册服务，然后能够查找并连接到该目录中的服务。

冗余-分布式系统中的冗余问题。

负载平衡 --负载平衡改善跨多个计算资源的工作负荷，诸如计算机，计算机集群，网络链路，中央处理单元，或磁盘驱动器的分布。

性能-问题 由于各种运营开销导致的性能问题。部署复杂性-Devops技能的要求。





### 微服务的优缺点是什么？说下你在项目中碰到的坑。

**优点：**松耦合，聚焦单一业务功能，无关开发语言，团队规模降低。在开发中，不需要了解多有业务，只专注于当前功能，便利集中，功能小而精。微服务一个功能受损，对其他功能影响并不是太大，可以快速定位问题。微服务只专注于当前业务逻辑代码，不会和 html、css 或其他界面进行混合。可以灵活搭配技术，独立性比较舒服。

**缺点：**随着服务数量增加，管理复杂，部署复杂，服务器需要增多，服务通信和调用压力增大，运维工程师压力增大，人力资源增多，系统依赖增强，数据一致性，性能监控。



### 微服务的优点缺点?说下开发项目中遇到的坑?

**优点:**

（1）每个服务直接足够内聚，代码容易理解

（2）开发效率高，一个服务只做一件事，适合小团队开发

（3）松耦合，有功能意义的服务。

（4）可以用不同语言开发，面向接口编程。

（5）易于第三方集成

（6）微服务只是业务逻辑的代码，不会和HTML,CSS或其他界

（7）可以灵活搭配，连接公共库/连接独立库

**缺点:**

（1）分布式系统的责任性

（2）多服务运维难度加大。

（3）系统部署依赖，服务间通信成本，数据一致 ，系统集成测试，性能监控。



### SpringBoot和SpringCloud的区别？

SpringBoot专注于快速方便的开发单个个体微服务。

SpringCloud是关注全局的微服务协调整理治理框架，它将SpringBoot开发的一个个单体微服务整合并管理起来，为各个微服务之间提供，配置管理、服务发现、断路器、路由、微代理、事件总线、全局锁、决策竞选、分布式会话等等集成服务SpringBoot可以离开SpringCloud独立使用开发项目， 但是SpringCloud离不开SpringBoot ，属于依赖的关系.

SpringBoot专注于快速、方便的开发单个微服务个体，SpringCloud关注全局的 治理框架



### 使用 Spring Cloud 有什么优势？

使用 Spring Boot 开发分布式微服务时，我们面临以下问题

**1、** 与分布式系统相关的复杂性-这种开销包括网络问题，延迟开销，带宽问题，安全问题。

**2、** 服务发现-服务发现工具管理群集中的流程和服务如何查找和互相交谈。它涉及一个服务目录，在该目录中注册服务，然后能够查找并连接到该目录中的服务。

**3、** 冗余-分布式系统中的冗余问题。

**4、** 负载平衡 --负载平衡改善跨多个计算资源的工作负荷，诸如计算机，计算机集群，网络链路，中央处理单元，或磁盘驱动器的分布。

**5、** 性能-问题 于各种运营开销导致的性能问题。

**6、** 部署复杂性 evops 技能的要求。



### 服务注册和发现是什么意思？Spring Cloud 如何实现？

当我们开始一个项目时，我们通常在属性文件中进行所有的配置。随着越来越多的服务开发和部署，添加和修改这些属性变得更加复杂。有些服务可能会下降，而某些位置可能会发生变化。手动更改属性可能会产生问题。Eureka 服务注册和发现可以在这种情况下提供帮助。由于所有服务都在 Eureka 服务器上注册并通过调用 Eureka 服务器完成查找，因此无需处理服务地点的任何更改和处理。



### 你所知道微服务的技术栈有哪些？列举一二。

| 微服务条目                     | 落地技术                                                     |
| :----------------------------- | :----------------------------------------------------------- |
| 服务开发                       | SpringBoot、Spring、SpringMVC                                |
| 服务配置与管理                 | Netfix公司的Archaius、阿里的Dlamond等                        |
| 服务注册与发现                 | Eurka、Consul、Zookeeper等                                   |
| 服务调用                       | Rest（服务通信）、RPC（Dubbo）、GRpc                         |
| 服务熔断器                     | Hystrix、Envoy等                                             |
| 负载均衡                       | Nginx、Ribbon等                                              |
| 服务接口调用（客户端简化工具） | Fegin等                                                      |
| 消息队列                       | Kafka、RabbitMQ、ActiveMQ等                                  |
| 服务配置中心管理               | SpringCloudConfig、Chef等                                    |
| 服务路由（API网关）            | Zuul等                                                       |
| 服务监控                       | Zabbix，Nagios，Metrics，Spectator等                         |
| 全链路追踪                     | Zipkin，Brave，Dapper等                                      |
| 服务部署                       | Docker，OpenStack，Kubernetes等                              |
| 数据流操作开发包               | SpringCloud Stream（封装与Redis，Rabbit，kafka等发送接收消息） |
| 事件消息总线                   | Spring Cloud Bus                                             |



### 微服务之间如何独立通讯的?

同步通信：dobbo通过 **RPC 远程过程调用、springcloud通过 REST 接口json调用** 等。

异步：消息队列，如：**RabbitMq、ActiveM、Kafka** 等。



### REST 和RPC对

**1、** RPC主要的缺陷是服务提供方和调用方式之间的依赖太强，需要对每一个微服务进行接口的定义，并通过持续继承发布，严格版本控制才不会出现冲突。

**2、** REST是轻量级的接口，服务的提供和调用不存在代码之间的耦合，只需要一个约定进行规范。



### 你所知道的微服务技术栈？

维度(springcloud)

服务开发：springboot spring springmvc

服务配置与管理:Netﬁx公司的Archaiusm ,阿里的Diamond

服务注册与发现:Eureka,Zookeeper

服务调用:Rest RPC gRpc

服务熔断器:Hystrix

服务负载均衡:Ribbon Nginx

服务接口调用:Fegin

消息队列:Kafka Rabbitmq activemq

服务配置中心管理:SpringCloudConﬁg

服务路由（API网关）Zuul

事件消息总线:SpringCloud Bus



### Spring Cloud的版本关系

Spring Cloud是一个由许多子项目组成的综合项目，各子项目有不同的发布节奏。为了管理Spring Cloud与各子项目的版本依赖关系，发布了一个清单，其中包括了某个Spring Cloud版本对应的子项目版本。

为了避免Spring Cloud版本号与子项目版本号混淆，Spring Cloud版本采用了名称而非版本号的命名，这些版本的名字采用了伦敦地铁站的名字，根据字母表的顺序来对应版本时间顺序，例如Angel是第一个版本，Brixton是第二个版本。

当Spring Cloud的发布内容积累到临界点或者一个重大BUG被解决后，会发布一个"service releases"版本，简称SRX版本，比如Greenwich.SR2就是Spring Cloud发布的Greenwich版本的第2个SRX版本。

**Spring Cloud和SpringBoot版本对应关系**

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330143709.png)

**Spring Cloud和各子项目版本对应关系**

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330143747.png)

> 注意：Hoxton版本是基于SpringBoot 2.2.x版本构建的，不适用于1.5.x版本。随着2019年8月SpringBoot 1.5.x版本停止维护，Edgware版本也将停止维护。



### Spring Cloud的子项目（主要项目）

大致可分成两类，

一类是对现有成熟框架"Spring Boot化"的封装和抽象，也是数量最多的项目；

第二类是开发了一部分分布式系统的基础设施的实现，如Spring Cloud Stream扮演的就是kafka, ActiveMQ这样的角色。



**Spring Cloud Config**

集中配置管理工具，分布式系统中统一的外部配置管理，默认使用Git来存储配置，可以支持客户端配置的刷新及加密、解密操作。



**Spring Cloud Netflix**

Netflix OSS 开源组件集成，包括Eureka、Hystrix、Ribbon、Feign、Zuul等核心组件。

- Eureka：服务治理组件，包括服务端的注册中心和客户端的服务发现机制；
- Ribbon：负载均衡的服务调用组件，具有多种负载均衡调用策略；
- Hystrix：服务容错组件，实现了断路器模式，为依赖服务的出错和延迟提供了容错能力；
- Feign：基于Ribbon和Hystrix的声明式服务调用组件；
- Zuul：API网关组件，对请求提供路由及过滤功能。



**Spring Cloud Bus**

用于将服务和服务实例与分布式消息系统链接在一起的事件总线。在集群中传播状态更改很有用（例如配置更改事件）。

你可以简单理解为 `Spring Cloud Bus` 的作用就是**管理和广播分布式系统中的消息**，也就是消息引擎系统中的广播模式。当然作为 **消息总线** 的 `Spring Cloud Bus` 可以做很多事而不仅仅是客户端的配置刷新功能。

而拥有了 `Spring Cloud Bus` 之后，我们只需要创建一个简单的请求，并且加上 `@ResfreshScope` 注解就能进行配置的动态修改了，下面我画了张图供你理解。

![img](https://my-blog-to-use.oss-cn-beijing.aliyuncs.com/2019-11/springcloud-bus-s213dsfsd.jpg)





**Spring Cloud Consul**

基于Hashicorp Consul的服务治理组件。



**Spring Cloud Security**

安全工具包，对Zuul代理中的负载均衡OAuth2客户端及登录认证进行支持。



**Spring Cloud Sleuth**

Spring Cloud应用程序的分布式请求链路跟踪，支持使用Zipkin、HTrace和基于日志（例如ELK）的跟踪。



**Spring Cloud Stream**

轻量级事件驱动微服务框架，可以使用简单的声明式模型来发送及接收消息，主要实现为Apache Kafka及RabbitMQ。



**Spring Cloud Task**

用于快速构建短暂、有限数据处理任务的微服务框架，用于向应用中添加功能性和非功能性的特性。



**Spring Cloud Zookeeper**

基于Apache Zookeeper的服务治理组件。



**Spring Cloud Gateway**

API网关组件，对请求提供路由及过滤功能。



**Spring Cloud OpenFeign**

基于Ribbon和Hystrix的声明式服务调用组件，可以动态创建基于Spring MVC注解的接口实现用于服务调用，在Spring Cloud 2.0中已经取代Feign成为了一等公民。



### spring cloud 的核心组件有哪些

- Eureka：服务注册于发现。
- Feign：基于动态代理机制，根据注解和选择的机器，拼接请求 url 地址，发起请求。
- Ribbon：实现负载均衡，从一个服务的多台机器中选择一台。
- Hystrix：提供线程池，不同的服务走不同的线程池，实现了不同服务调用的隔离，避免了服务雪崩的问题。
- Zuul：网关管理，由 Zuul 网关转发请求给对应的服务。



### springcloud如何实现服务的注册?

**1、**服务发布时，指定对应的服务名,将服务注册到 注册中心(eureka zookeeper)
**2、**注册中心加@EnableEurekaServer,服务用@EnableDiscoveryClient，然后用ribbon或feign进行服务直接的调用发现。



### 什么是 Hystrix？它如何实现容错？

Hystrix 是一个延迟和容错库，旨在隔离远程系统，服务和第三方库的访问点，当出现故障是不可避免的故障时，停止级联故障并在复杂的分布式系统中实现弹性。通常对于使用微服 构开发的系统，涉及到许多微服务。这些微服务彼此协作。思考以下微服务

![图片](https://mmbiz.qpic.cn/mmbiz_png/x0kXIOa6owXwanmibU2gOcWrOOrXBUb5ASnuA0eiavgIwwsk40nyWzqm9dnUsoQKktGNq5zRxDvepX0mDR2YI8XA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

假设如果上图中的微服务 9 失败了，那么使用传统方法我们将传播一个异常。但这仍然会导致整个系统崩溃。随着微服务数量的增加，这个问题变得更加复杂。微服务的数量可以高达 1000.这是 hystrix 出现的地方 我们将使 Hystrix 在这种情况下的 Fallback 方法功能。我们有两个服务 employee-consumer 使用由 employee-consumer 公开的服务。简化图如下所示

![图片](https://mmbiz.qpic.cn/mmbiz_png/x0kXIOa6owXwanmibU2gOcWrOOrXBUb5AGVgzJbUtCIhibUqmrMpr27CthYaykld2aMZB5HibBSkOSl94YOam1JLA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

现在假设由于 原因，employee-producer 公开的服务会抛出异常。我们在这种情况下使用 Hystrix定义了一个回退方法。这种后备方法应该具有与公开服务相同的返回类型。如果暴露服务中出现异常，则回退方法将返回一些值。



### 什么是 Hystrix 断路器？我们需要它吗？

由于某些原因，employee-consumer 公开服务会引发异常。在这种情况下使用Hystrix 我们定义了一个回退方法。如果在公开服务中发生异常，则回退方法返回一些默认值。

![图片](https://mmbiz.qpic.cn/mmbiz_png/x0kXIOa6owXwanmibU2gOcWrOOrXBUb5A7kjib4qXO62rribXq9uiawf005jh7icOye24w3I27TpTpQ6tbqWibvBwnnA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

如果 ﬁrstPage method() 中的异常继续发生，则 Hystrix 电 ，并且员工使用者将一起跳过ﬁrtsPage 方法，并直接调用回退方法。断路器的目的是给第一 方法或第一页方法可能调用的其他方法留出时间，并导致异常恢复。可能发生的情况是，在负载较小的情况下，导致异常的问题有更好的恢复机会 。

![图片](https://mmbiz.qpic.cn/mmbiz_png/x0kXIOa6owXwanmibU2gOcWrOOrXBUb5AHD5Jich9ibMpmLOcBAYGvr0HGC1B61W9ogsiaicEXH3ybDLkGaMRWWJwaw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### Hystrix相关注解

**@EnableHystrix： **开启熔断

**@HystrixCommand(fallbackMethod=”XXX”)：** 声明一个失败回滚处理函数XXX，当被注解的方法执行超时（默认是 0毫秒），就会执行fallback函数，返回错误提示。

![图片](https://mmbiz.qpic.cn/mmbiz_png/x0kXIOa6owXwanmibU2gOcWrOOrXBUb5ArUGBoWDcLRiciaJic8icibcC0ug8wcaqmoLwBoZibb0QRTzCPkZz3dxna0Ug/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### 什么是 Netﬂix Feign？它的优点是什么？

Feign 是受到 Retroﬁt，JAXRS-2.0 和 WebSocket 启发的 java 客户端联编程序。Feign 的第一个目标是将约束分母的复杂性统一到 http apis，而不考虑其稳定性。在 employee-consumer 的例子中，我们使用了 emplo e-producer 使用 REST模板公开的 REST 服务。

但是我们必须编写大量代码才能执行以下步骤

**1、** 使用功能区进行负载平衡。

**2、** 获取服务实例，然后获取基本 URL。

**3、** 利用 REST 模板来使用服务。前面的代码如下

```java
@Controllerpublic class ConsumerControllerClient {
	@Autowired
	private LoadBalancerClient loadBalancer;
	public void getEmployee() throws RestClientException, IOException {
		ServiceInstance serviceInstance=loadBalancer.choose("employee-producer");
		System.out.println(serviceInstance.getUri());
		String baseUrl=serviceInstance.getUri().toString();
		baseUrl=baseUrl+"/employee";
		RestTemplate restTemplate = new RestTemplate();
		ResponseEntity<String> response=null;
		try{
			response=restTemplate.exchange(baseUrl,
			HttpMethod.GET, getHeaders(),String.class);
		}
		catch (Exception ex)
		{
			System.out.println(ex);
		}
		System.out.println(response.getBody());
	}}
```

之前的代码，有像 NullPointer 这样的例外的机会，并不是最优 。我们将看到如何使用 Netﬂix Fe n使呼叫变得更加轻松和清洁。如果 Netﬂix Ribbon 依赖关系 径中，那么 Feign 默认也会负载平衡。



### 分布式配置中心能干嘛？

**1、** 集中管理配置文件不同环境不同配置，动态化的配置更新，分环境部署比如

dev/test/prod/beta/release

**2、** 运行期间动态调整 置，不再需要在每个服务部署的机器上编写配置文件，服务会向配置中心统一拉取配置自己的信息

**3、** 当配置发生变动时，服务不需要重启即可感知到配置的变化并应用新的配置将配置信息以REST接口的形式暴露



###  什么是Eureka

eureka是Netflix开发的服务发现组件，本身是一个基于REST的服务。Spring Cloud将它集成在其子项目spring-cloud-netflix中， 以实现Spring Cloud的服务发现功能。eureka现在已经从1.0升级到2.0，可惜的是eureka2.0不在开源，但也不影响我们的使用。 由于基于REST服务，自然而然的就能想到，这个服务一定会有心跳检测、健康检查和客户端缓存等机制。

**Eureka包括两个端：**

- **Eureka Server：注册中心服务端**，用于维护和管理注册服务列表。
- **Eureka Client：注册中心客户端**，向注册中心注册服务的应用都可以叫做Eureka Client（包括Eureka Server本身）。



**Eureka Server**

- 依赖介绍
  - spring-cloud-starter-netflix-eureka-server eureka服务端的标识，标志着此服务是做为注册中心
- application.properties配置

```xml
spring.application.name=eureka-server  //服务名称
server.port=8000            //服务端口

eureka.client.register-with-eureka=false  //自身不做为服务注册到注册中心

eureka.client.fetch-registry=false     //从注册表拉取信息

eureka.client.serviceUrl.defaultZone=http://localhost:8000/eureka/    服务注册地址
```

- 运行服务spring-cloud-eureka
- 运行成功后访问localhost:8000，会显示eureka提供的服务页面



**Eureka Client**

- 依赖介绍
  - spring-cloud-starter-netflix-eureka-client eureka客户端所需依赖。
  - spring-boot-starter-web web服务所需，内置tomcat服务器。
- application.properties配置

```xml
spring.application.name=eureka-client-a
server.port=8001

eureka.client.serviceUrl.defaultZone=http://localhost:8000/eureka/
```

- 运行服务spring-cloud-clientA
- 运行成功后访问localhost:8000，会显示eureka提供的服务页面



### eureka自我保护机制是什么?

当Eureka Server 点在短时间内丢失了过多实例的连接时（比如网络故障或频繁启动关闭客户端）节点会进入自我保护模式，保护注册信息，不再删除注册数据，故障恢复时，自动退出自我保护模式。



### 作为 务注册中心，Eureka比Zookeeper好在哪里?

**1、** Eureka保证的是可用性和分区容错性，Zookeeper 保证的是一致性和分区容错性 。

**2、** Eureka还有一种自我保护机制，如果在15分钟内超过85%的节点都没有正常的心跳，那么Eureka就认为客户端与注册中心出现了网络故障。而不会像zookeeper那样使整个注册服务瘫痪。



### Eureka和zookeeper都可以提供服务注册与发现的功能，请说说两个的区别？

Zookeeper保证了CP（C：一致性，P：分区容错性），Eureka保证了AP（A：高可用）

**1、** 当向注册中心查询服务列表时，我们可以容忍注册中心返回的是几分钟以前的信息，但不能容忍直接down掉不可用。就是说，服务注册功能对高可用性要求比较高，但zk会出现这样一种情况，当master节点因为网络故障与其他节点失去联系时，剩余节点会重新选leader。问题在于，选取leader时间过长，30 ~ 120s，且选取期间zk集群都不可用，这样就会导致选取期间注册服务瘫痪。在云部署的环境下，因网络问题使得zk集群失去master节点是较大概率会发生的事，虽然服务能够恢复，但是漫长的选取时间导致的注册长期不可用是不能容忍的。

**2、** Eureka保证了可用性，Eureka各个节点是平等的，几个节点挂掉不会影响正常节点的工作，剩余的节点仍然可以提供注册和查询服务。而Eureka的客户端向某个Eureka注册或发现时发生连接失败，则会自动切换到其他节点，只要有一台Eureka还在，就能保证注册服务可用，只是查到的信息可能不是最新的。除此之外，Eureka还有自我保护机制，如果在15分钟内超过85%的节点没有正常的心跳，那么Eureka就认为 户端与注册中心发生了网络故障，此时会出现以下几种情况：

①、Eureka不 从注册列表中移除因为长时间没有收到心跳而应该过期的服务。

②、Eureka仍然能够接受新服务的注册和查询请求，但是不会被同步到其他节点上（即保证当前节点仍然可用）

③、当网络稳定时，当前实例新的注册信息会被同步到其他节点。

因此，Eureka可以很好的应对因网络故障导致部分节点失去联系的情况，而不会像Zookeeper那样使整个微服务瘫痪。



### 你所知道的微服务技术栈？

当Eureka Server 节点在短时间内丢失了过多实例的连接时（比如网络故障或频繁启动关闭客户端）节点会进入自我保护模式，保护注册信息，不再删除注册数据，故障恢复时，自动退出自我保护模式。



### 使用Spring Cloud有什么优势？

使用Spring Boot开发分布式微服务时，我们面临以下问题

- 与分布式系统相关的复杂性-这种开销包括网络问题，延迟开销，带宽问题，安全问题。
- 服务发现-服务发现工具管理群集中的流程和服务如何查找和互相交谈。它涉及一个服务目录，在该目录中注册服务，然后能够查找并连接到该目录中的服务。
- 冗余-分布式系统中的冗余问题。
- 负载平衡 --负载平衡改善跨多个计算资源的工作负荷，诸如计算机，计算机集群，网络链路，中央处理单元，或磁盘驱动器的分布。
- 性能-问题 由于各种运营开销导致的性能问题。
- 部署复杂性-Devops技能的要求。



### SpringBoot 和 SpringCloud 之间关系？

**SpringBoot：**专注于快速方便的开发单个个体微服务（关注微观）；

**SpringCloud：**关注全局的微服务协调治理框架，将SpringBoot开发的一个个单体微服务组合并管理起来（关注宏观）；

SpringBoot可以离开SpringCloud独立使用，但是SpringCloud不可以离开SpringBoot，属于依赖关系。



### SpringCloud 和 Dubbo 有哪些区别?

首先，他们都是**分布式管理框架**。

dubbo 是**二进制传输**，占用带宽会少一点。SpringCloud是**http 传输**，带宽会多一点，同时使用http协议一般会使用**JSON报文**，消耗会更大。

dubbo 开发难度较大，所依赖的 jar 包有很多问题**大型工程无法解决**。SpringCloud 对第三方的继承可以**一键式生成，天然集成**。

SpringCloud 接口协议约定比较松散，**需要强有力的行政措施来限制接口无序升级**。

最大的区别: **Spring Cloud抛弃了Dubbo 的RPC通信，采用的是基于HTTP的REST方式。**

>  严格来说，这两种方式各有优劣。虽然在一定程度上来说，后者牺牲了服务调用的性能，但也避免了上面提到的原生RPC带来的问题。而且REST相比RPC更为灵活，服务提供方和调用方的依赖只依靠一纸契约，不存在代码级别的强依赖，这在强调快速演化的微服务环境下，显得更为合适。



### 什么是Spring Cloud Config?

在分布式系统中，由于服务数量巨多，为了方便服务配置文件统一管理，实时更新，所以需要分布式配置中心组件。在Spring Cloud中，有分布式配置中心组件spring cloud config ，它支持配置服务放在配置服务的内存中（即本地），也支持放在远程Git仓库中。在spring cloud config 组件中，分两个角色，一是config server，二是config client。

使用：

**1、**添加pom依赖

**2、**配置文件添加相关配置

**3、**启动类添加注解@EnableConfigServer



### 什么是 zuul路由网关

**1、** Zuul 包含了对请求的路由和过滤两个最主要的功能:其中 责将外部请求转发到具体的微服务实例上，是实现外部访问统一入口的基础而过滤器功能则负 请求的处理过程进行干预，是实现请求校验、服务聚合等功能的基础、

**2、** Zuul和Eureka进行整合，将Zuul自身注册为Eureka服务治理下的应用，同时从Eureka中获得其他微服务的消息，也即以后的访问微服务都是通过Zuul跳转后获得。

**注意：** Zuul服务最终还是会注册进Eureka 提供=代理+路由+过滤 三大功能



### 什么是Ribbon？

ribbon是一个负载均衡客户端，可以很好的控制htt和tcp的一些行为。feign默认集成了ribbon。



### Ribbon负载均衡能干什么？

**1、** 将用户的请求平摊的分配到多个服务上

**2、** 集中式LB即在服务的消费方和提供方之间使用独立的LB设施(可以是硬件，如F5, 也可以是软件，如nginx), 由该设施负责把访问请求通过某种策略转发至服务的提供方；

**3、** 进程内LB将LB逻辑集成到消费方，消费方从服务注册中心获知有哪些地址可用，然后自己再从这些地址中选择出一个合适的服务器。

注意：Ribbon就属于进程内LB，它只是一个类库，集成于消费方进程，消费方 它来获取到服务提供方的地址。



###  什么是feigin？它的优点是什么？

**1、**feign采用的是基于接口的注解
**2、**feign整合了ribbon，具有负载均衡的能力
**3、**整合了Hystrix，具有熔断的能力

使用:
**1、**添加pom依赖。
**2、**启动类添加@EnableFeignClients
**3、**定义一个接口@FeignClient(name=“xxx”)指定调用哪个服务



### Ribbon和Feign的区别？

**1、**Ribbon都是调用其他服务的，但方式不同。
**2、**启动类注解不同，Ribbon是@RibbonClient feign的是@EnableFeignClients
**3、**服务指定的位置不同，Ribbon是在@RibbonClient注解上声明，Feign则是在定义抽象方法的接口中使用@FeignClient声明。
**4、**调用方式不同，Ribbon需要自己构建http请求，模拟http请求然后使用RestTemplate发送给其他服务，步骤相当繁琐。Feign需要将调用的方法定义成抽象方法即可。



### 什么是Spring Cloud Gateway?

Spring Cloud Gateway是Spring Cloud官方推出的第二代网关框架，取代Zuul网关。网关作为流量的，在微服务系统中有着非常作用，网关常见的功能有路由转发、权限校验、限流控制等作用。

使用了一个RouteLocatorBuilder的bean去创建路由，除了创建路由RouteLocatorBuilder可以让你添加各种predicates和filters，predicates断言的意思，顾名思义就是根据具体的请求的规则，由具体的route去处理，filters是各种过滤器，用来对请求做各种判断和修改。



### 什么是 Hystrix？它如何实现容错？

Hystrix 是一个延迟和容错库，旨在隔离远程系统，服务和第三方库的访问点，当出现故障是不可避免的故障时，停止级联故障并在复杂的分布式系统中实现弹性。

通常对于使用微服务架构开发的系统，涉及到许多微服务。这些微服务彼此协作。

思考以下微服务

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330144146.png)



假设如果上图中的微服务 9 失败了，那么使用传统方法我们将传播一个异常。但这仍然会导致整个系统崩溃。

随着微服务数量的增加，这个问题变得更加复杂。微服务的数量可以高达 1000.这是 hystrix 出现的地方 我们将使用 Hystrix 在这种情况下的 Fallback 方法功能。我们有两个服务 employee-consumer 使用由 employee-consumer 公开的服务。

简化图如下所示

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330144204.png)

现在假设由于某种原因，employee-producer 公开的服务会抛出异常。我们在这种情况下使用 Hystrix 定义了一个回退方法。这种后备方法应该具有与公开服务相同的返回类型。如果暴露服务中出现异常，则回退方法将返回一些值



### 什么是 Hystrix 断路器？我们需要它吗？

由于某些原因，employee-consumer 公开服务会引发异常。在这种情况下使用Hystrix 我们定义了一个回退方法。如果在公开服务中发生异常，则回退方法返回一些默认值。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330144450.png)

如果 firstPage method() 中的异常继续发生，则 Hystrix 电路将中断，并且员工使用者将一起跳过 firtsPage 方法，并直接调用回退方法。断路器的目的是给第一页方法或第一页方法可能调用的其他方法留出时间，并导致异常恢复。可能发生的情况是，在负载较小的情况下，导致异常的问题有更好的恢复机会 。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330144513.png)



### 什么是 Netflix Feign？它的优点是什么？

Feign 是受到 Retrofit，JAXRS-2.0 和 WebSocket 启发的 java 客户端联编程序。

Feign 的第一个目标是将约束分母的复杂性统一到 http apis，而不考虑其稳定性。

在 employee-consumer 的例子中，我们使用了 employee-producer 使用 REST模板公开的 REST 服务。

但是我们必须编写大量代码才能执行以下步骤

**1、** 使用功能区进行负载平衡。

**2、 ** 获取服务实例，然后获取基本 URL。

**3、 ** 利用 REST 模板来使用服务。前面的代码如下

```java
@Controller
public class ConsumerControllerClient {
@Autowired
private LoadBalancerClient loadBalancer;
public void getEmployee() throws RestClientException, IOException {
	ServiceInstance serviceInstance=loadBalancer.choose("employee-producer");
	System.out.println(serviceInstance.getUri());
	String baseUrl=serviceInstance.getUri().toString();
	baseUrl=baseUrl+"/employee";
	RestTemplate restTemplate = new RestTemplate();
	ResponseEntity<String> response=null;
	try{
		response=restTemplate.exchange(baseUrl,
					HttpMethod.GET, getHeaders(),String.class);
	}
	catch (Exception ex)
		{
		System.out.println(ex);
	}
	System.out.println(response.getBody());

```

之前的代码，有像 NullPointer 这样的例外的机会，并不是最优的。我们将看到如何使用 Netflix Feign 使呼叫变得更加轻松和清洁。如果 Netflix Ribbon 依赖关系也在类路径中，那么 Feign 默认也会负责负载平衡。



### 什么是Spring Cloud Gateway?

Spring Cloud Gateway是Spring Cloud官方推出的第二代网关框架，取代Zuul网关。网关作为流量的，在微服务系统中有着非常作用，网关常见的功能有路由转发、权限校验、限流控制等作用。

使用了一个RouteLocatorBuilder的bean去创建路由，除了创建路由RouteLocatorBuilder可以让你添加各种predicates和filters，predicates断言的意思，顾名思义就是根据具体的请求的规则，由具体的route去处理，filters是各种过滤器，用来对请求做各种判断和修改。



### 服务注册和发现是什么意思？Spring Cloud如何实现？

当我们开始一个项目时，我们通常在属性文件中进行所有的配置。随着越来越多的服务开发和部署，添加和修改这些属性变得更加复杂。有些服务可能会下降，而某些位置可能会发生变化。手动更改属性可能会产生问题。 Eureka服务注册和发现可以在这种情况下提供帮助。由于所有服务都在Eureka服务器上注册并通过调用Eureka服务器完成查找，因此无需处理服务地点的任何更改和处理。



### 负载平衡的意义什么？

在计算中，负载平衡可以改善跨计算机，计算机集群，网络链接，中央处理单元或磁盘驱动器等多种计算资源的工作负载分布。负载平衡旨在优化资源使用，最大化吞吐量，最小化响应时间并避免任何单一资源的过载。使用多个组件进行负载平衡而不是单个组件可能会通过冗余来提高可靠性和可用性。负载平衡通常涉及专用软件或硬件，例如多层交换机或域名系统服务器进程。



### 什么是熔断？什么是服务降级？

服务熔断的作用类似于我们家用的保险丝，当某服务出现不可用或响应超时的情况时，为了防止整个系统出现雪崩，暂时停止对该服务的调用。

服务降级是从整个系统的负荷情况出发和考虑的，对某些负荷会比较高的情况，为了预防某些功能（业务场景）出现负荷过载或者响应慢的情况，在其内部暂时舍弃对一些非核心的接口和数据的请求，而直接返回一个提前准备好的fallback（退路）错误处理信息。这样，虽然提供的是一个有损的服务，但却保证了整个系统的稳定性和可用性。



### 什么是Netflix Feign？它的优点是什么？

Feign是受到Retrofit，JAXRS-2.0和WebSocket启发的java客户端联编程序。Feign的第一个目标是将约束分母的复杂性统一到http apis，而不考虑其稳定性。在employee-consumer的例子中，我们使用了employee-producer使用REST模板公开的REST服务。

但是我们必须编写大量代码才能执行以下步骤

- 使用功能区进行负载平衡。
- 获取服务实例，然后获取基本URL。
- 利用REST模板来使用服务。 前面的代码如下

```java
@Controller
public class ConsumerControllerClient {

@Autowired
private LoadBalancerClient loadBalancer;

public void getEmployee() throws RestClientException, IOException {

    ServiceInstance serviceInstance=loadBalancer.choose("employee-producer");

    System.out.println(serviceInstance.getUri());

    String baseUrl=serviceInstance.getUri().toString();

    baseUrl=baseUrl+"/employee";

    RestTemplate restTemplate = new RestTemplate();
    ResponseEntity<String> response=null;
    try{
    response=restTemplate.exchange(baseUrl,
            HttpMethod.GET, getHeaders(),String.class);
    }catch (Exception ex)
    {
        System.out.println(ex);
    }
    System.out.println(response.getBody());
}
```

之前的代码，有像NullPointer这样的例外的机会，并不是最优的。我们将看到如何使用Netflix Feign使呼叫变得更加轻松和清洁。如果Netflix Ribbon依赖关系也在类路径中，那么Feign默认也会负责负载平衡。



### 什么是 Spring Cloud Bus？我们需要它吗？

考虑以下情况：我们有多个应用程序使用 Spring Cloud Config 读取属性，而Spring Cloud Config 从 GIT 读取这些属性。

下面的例子中多个员工生产者模块从 Employee Config Module 获取 Eureka 注册的财产。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330144607.png)

如果假设 GIT 中的 Eureka 注册属性更改为指向另一台 Eureka 服务器，会发生什么情况。在这种情况下，我们将不得不重新启动服务以获取更新的属性。

还有另一种使用执行器端点/刷新的方式。但是我们将不得不为每个模块单独调用这个 url。例如，如果 Employee Producer1 部署在端口 8080 上，则调用 http：// localhost：8080 / refresh。同样对于 Employee Producer2 http：//localhost：8081 / refresh 等等。这又很麻烦。这就是 Spring Cloud Bus 发挥作用的地方。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330145409.png)

Spring Cloud Bus 提供了跨多个实例刷新配置的功能。因此，在上面的示例中，如果我们刷新 Employee Producer1，则会自动刷新所有其他必需的模块。如果我们有多个微服务启动并运行，这特别有用。这是通过将所有微服务连接到单个消息代理来实现的。无论何时刷新实例，此事件都会订阅到侦听此代理的所有微服务，并且它们也会刷新。可以通过使用端点/总线/刷新来实现对任何单个实例的刷新。



### 微服务是如何对外提供统一接口的(zuul具体使用)

因为每一个微服务都是独立运行的，都有自己独立的IP和端口，而当他们需要统一对外提供服务这时候就需要
SpringCloud网关 zuul网关也是netflix公司旗下的项目

使用它也很简单
在pom依赖中 引入 Spring-cloud-starter-netflix-zuul

在SpringBoot启动类中 开启 @EnableZuulProxy

然后在配置文件中定义 路由规则：

routes:
路由名称:
path: /映射路径/**
serviceId: Eureka中的服务名称

zuul也提供了过滤器功能，如果要做一些token检查 或者 过滤时可以使用
用法 就是写一个类 继承 ZuulFilter类
会要求我们实现几个方法
filterType: 过滤器什么时候执行 pre 前置 post 过程中 after 之后
shouldFilter: 过滤器是否执行 可以写判断方法 返回boolean值 true执行，false不执行此过滤器
filterOrder: 过滤器的执行顺序 排序号
run: 具体过滤器的方法



### Zuul 的过滤功能

如果说，路由功能是 `Zuul` 的基操的话，那么**过滤器**就是 `Zuul`的利器了。毕竟所有请求都经过网关(Zuul)，那么我们可以进行各种过滤，这样我们就能实现 **限流**，**灰度发布**，**权限控制** 等等。



**简单实现一个请求时间日志打印**

要实现自己定义的 `Filter` 我们只需要继承 `ZuulFilter` 然后将这个过滤器类以 `@Component` 注解加入 Spring 容器中就行了。

在给你们看代码之前我先给你们解释一下关于过滤器的一些注意点。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330161410.png)

过滤器类型：`Pre`、`Routing`、`Post`。前置`Pre`就是在请求之前进行过滤，`Routing`路由过滤器就是我们上面所讲的路由策略，而`Post`后置过滤器就是在 `Response` 之前进行过滤的过滤器。你可以观察上图结合着理解，并且下面我会给出相应的注释。

```java
// 加入Spring容器
@Component
public class PreRequestFilter extends ZuulFilter {
    // 返回过滤器类型 这里是前置过滤器
    @Override
    public String filterType() {
        return FilterConstants.PRE_TYPE;
    }
    // 指定过滤顺序 越小越先执行，这里第一个执行
    // 当然不是只真正第一个 在Zuul内置中有其他过滤器会先执行
    // 那是写死的 比如 SERVLET_DETECTION_FILTER_ORDER = -3
    @Override
    public int filterOrder() {
        return 0;
    }
    // 什么时候该进行过滤
    // 这里我们可以进行一些判断，这样我们就可以过滤掉一些不符合规定的请求等等
    @Override
    public boolean shouldFilter() {
        return true;
    }
    // 如果过滤器允许通过则怎么进行处理
    @Override
    public Object run() throws ZuulException {
        // 这里我设置了全局的RequestContext并记录了请求开始时间
        RequestContext ctx = RequestContext.getCurrentContext();
        ctx.set("startTime", System.currentTimeMillis());
        return null;
    }
}

```



```java
// lombok的日志
@Slf4j
// 加入 Spring 容器
@Component
public class AccessLogFilter extends ZuulFilter {
    // 指定该过滤器的过滤类型
    // 此时是后置过滤器
    @Override
    public String filterType() {
        return FilterConstants.POST_TYPE;
    }
    // SEND_RESPONSE_FILTER_ORDER 是最后一个过滤器
    // 我们此过滤器在它之前执行
    @Override
    public int filterOrder() {
        return FilterConstants.SEND_RESPONSE_FILTER_ORDER - 1;
    }
    @Override
    public boolean shouldFilter() {
        return true;
    }
    // 过滤时执行的策略
    @Override
    public Object run() throws ZuulException {
        RequestContext context = RequestContext.getCurrentContext();
        HttpServletRequest request = context.getRequest();
        // 从RequestContext获取原先的开始时间 并通过它计算整个时间间隔
        Long startTime = (Long) context.get("startTime");
        // 这里我可以获取HttpServletRequest来获取URI并且打印出来
        String uri = request.getRequestURI();
        long duration = System.currentTimeMillis() - startTime;
        log.info("uri: " + uri + ", duration: " + duration / 100 + "ms");
        return null;
    }
}

```

上面就简单实现了请求时间日志打印功能，你有没有感受到 `Zuul` 过滤功能的强大了呢？

没有？好的、那我们再来。

**令牌桶限流**

当然不仅仅是令牌桶限流方式，`Zuul` 只要是限流的活它都能干，这里我只是简单举个例子

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330161523.png)

我先来解释一下什么是 **令牌桶限流** 吧。

首先我们会有个桶，如果里面没有满那么就会以一定 **固定的速率** 会往里面放令牌，一个请求过来首先要从桶中获取令牌，如果没有获取到，那么这个请求就拒绝，如果获取到那么就放行。很简单吧，啊哈哈、

下面我们就通过 `Zuul` 的前置过滤器来实现一下令牌桶限流。

```java
package com.lgq.zuul.filter;

import com.google.common.util.concurrent.RateLimiter;
import com.netflix.zuul.ZuulFilter;
import com.netflix.zuul.context.RequestContext;
import com.netflix.zuul.exception.ZuulException;
import lombok.extern.slf4j.Slf4j;
import org.springframework.cloud.netflix.zuul.filters.support.FilterConstants;
import org.springframework.stereotype.Component;

@Component
@Slf4j
public class RouteFilter extends ZuulFilter {
    // 定义一个令牌桶，每秒产生2个令牌，即每秒最多处理2个请求
    private static final RateLimiter RATE_LIMITER = RateLimiter.create(2);
    @Override
    public String filterType() {
        return FilterConstants.PRE_TYPE;
    }

    @Override
    public int filterOrder() {
        return -5;
    }

    @Override
    public Object run() throws ZuulException {
        log.info("放行");
        return null;
    }

    @Override
    public boolean shouldFilter() {
        RequestContext context = RequestContext.getCurrentContext();
        if(!RATE_LIMITER.tryAcquire()) {
            log.warn("访问量超载");
            // 指定当前请求未通过过滤
            context.setSendZuulResponse(false);
            // 向客户端返回响应码429，请求数量过多
            context.setResponseStatusCode(429);
            return false;
        }
        return true;
    }
}

```

这样我们就能将请求数量控制在一秒两个，有没有觉得很酷？