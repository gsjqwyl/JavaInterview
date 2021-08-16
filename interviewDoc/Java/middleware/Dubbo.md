**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [Dubbo是什么？](#dubbo是什么)
- [为什么要用Dubbo？](#为什么要用dubbo)
- [Dubbo 和 Spring Cloud 有什么区别？](#dubbo-和-spring-cloud-有什么区别)
- [dubbo都支持什么协议，推荐用哪种？](#dubbo都支持什么协议推荐用哪种)
- [Dubbo推荐用什么协议?使用该协议有哪些优缺点?](#dubbo推荐用什么协议使用该协议有哪些优缺点)
- [说说Dubbo的分层？](#说说dubbo的分层)
- [Dubbo核心组件是？](#dubbo核心组件是)
- [Dubbo核心配置有哪些？](#dubbo核心配置有哪些)
- [能说下Dubbo的工作原理吗？](#能说下dubbo的工作原理吗)
- [介绍一下Dubbo框架分层？](#介绍一下dubbo框架分层)
- [注册中心挂了可以继续通信吗？](#注册中心挂了可以继续通信吗)
- [Dubbo需要 Web 容器吗？](#dubbo需要-web-容器吗)
- [Dubbo的执行流程](#dubbo的执行流程)
- [Dubbo内置了哪几种服务容器？](#dubbo内置了哪几种服务容器)
- [Dubbo有哪些注册中心？](#dubbo有哪些注册中心)
- [Dubbo里面有哪几种节点角色？](#dubbo里面有哪几种节点角色)
- [Dubbo中zookeeper做注册中心，如果注册中心集群都挂掉，发布者和订阅者之间还能通信么？](#dubbo中zookeeper做注册中心如果注册中心集群都挂掉发布者和订阅者之间还能通信么)
- [注册中心宕机，服务间是否可以继续通信](#注册中心宕机服务间是否可以继续通信)
- [Dubbo服务负载均衡策略？](#dubbo服务负载均衡策略)
- [Dubbo在安全机制方面是如何解决的](#dubbo在安全机制方面是如何解决的)
- [Dubbo超时时间的设置](#dubbo超时时间的设置)
- [画一画服务注册与发现的流程图](#画一画服务注册与发现的流程图)
- [Dubbo默认使用什么注册中心，还有别的选择吗？](#dubbo默认使用什么注册中心还有别的选择吗)
- [Dubbo有哪几种配置方式？](#dubbo有哪几种配置方式)
- [Dubbo 核心的配置有哪些？](#dubbo-核心的配置有哪些)
- [在 Provider 上可以配置的 Consumer 端的属性有哪些？](#在-provider-上可以配置的-consumer-端的属性有哪些)
- [Dubbo启动时如果依赖的服务不可用会怎样？](#dubbo启动时如果依赖的服务不可用会怎样)
- [Dubbo支持哪些序列化方式?](#dubbo支持哪些序列化方式)
- [Dubbo推荐使用什么序列化框架，你知道的还有哪些？](#dubbo推荐使用什么序列化框架你知道的还有哪些)
- [Dubbo默认使用的是什么通信框架，还有别的选择吗？](#dubbo默认使用的是什么通信框架还有别的选择吗)
- [Dubbo有哪几种集群容错方案，哪几种负载均衡策略？](#dubbo有哪几种集群容错方案哪几种负载均衡策略)
- [Dubbo用到哪些设计模式，简要介绍？](#dubbo用到哪些设计模式简要介绍)
- [注册了多个同一样的服务，如果测试指定的某一个服务呢？](#注册了多个同一样的服务如果测试指定的某一个服务呢)
- [Dubbo支持服务多协议吗？](#dubbo支持服务多协议吗)
- [Dubbo 支持哪些协议，每种协议的应用场景，优缺点？](#dubbo-支持哪些协议每种协议的应用场景优缺点)
- [Dubbo 集群的负载均衡有哪些策略](#dubbo-集群的负载均衡有哪些策略)
- [当一个服务接口有多种实现时怎么做？](#当一个服务接口有多种实现时怎么做)
- [服务调用超时问题怎么解决](#服务调用超时问题怎么解决)
- [服务上线怎么兼容旧版本？](#服务上线怎么兼容旧版本)
- [Dubbo可以对结果进行缓存吗？](#dubbo可以对结果进行缓存吗)
- [Dubbo服务之间的调用是阻塞的吗？](#dubbo服务之间的调用是阻塞的吗)
- [Dubbo支持分布式事务吗？](#dubbo支持分布式事务吗)
- [Dubbo的心跳机制](#dubbo的心跳机制)
- [Dubbo的zookeeper做注册中心，如果注册中心全部挂掉，发布者和订阅者还能通信吗？](#dubbo的zookeeper做注册中心如果注册中心全部挂掉发布者和订阅者还能通信吗)
- [Dubbo telnet 命令能做什么？](#dubbo-telnet-命令能做什么)
- [说说服务暴露的流程？](#说说服务暴露的流程)
- [说说服务引用的流程？](#说说服务引用的流程)
- [有哪些负载均衡策略？](#有哪些负载均衡策略)
- [Dubbo如何优雅停机？](#dubbo如何优雅停机)
- [了解Dubbo SPI机制吗？](#了解dubbo-spi机制吗)
- [如果让你实现一个RPC框架怎么设计？](#如果让你实现一个rpc框架怎么设计)
- [服务提供者能实现失效踢出是什么原理？](#服务提供者能实现失效踢出是什么原理)
- [如何解决服务调用链过长的问题？](#如何解决服务调用链过长的问题)
- [服务读写推荐的容错策略是怎样的？](#服务读写推荐的容错策略是怎样的)
- [Dubbo必须依赖的包有哪些？](#dubbo必须依赖的包有哪些)
- [Dubbo的管理控制台能做什么？](#dubbo的管理控制台能做什么)
- [说说 Dubbo 服务暴露的过程。](#说说-dubbo-服务暴露的过程)
- [Dubbo 停止维护了吗？](#dubbo-停止维护了吗)
- [Dubbo 和 Dubbox 有什么区别？](#dubbo-和-dubbox-有什么区别)
- [在使用过程中都遇到了些什么问题？如何解决的？](#在使用过程中都遇到了些什么问题如何解决的)
- [你还了解别的分布式框架吗？](#你还了解别的分布式框架吗)

<!-- /TOC -->

### Dubbo是什么？ 

Dubbo是阿里巴巴开源的基于 Java 的高性能 RPC 分布式服务框架，现已成为 Apache 基金会孵化项目。

面试官问你如果这个都不清楚，那下面的就没必要问了。

官网：http://dubbo.apache.org



### 为什么要用Dubbo？

因为是阿里开源项目，国内很多互联网公司都在用，已经经过很多线上考验。内部使用了 Netty、Zookeeper，保证了高性能高可用性。

使用 Dubbo 可以将核心业务抽取出来，作为独立的服务，逐渐形成稳定的服务中心，可用于提高业务复用灵活扩展，使前端应用能更快速的响应多变的市场需求。

下面这张图可以很清楚的诠释，最重要的一点是，分布式架构可以承受更大规模的并发流量。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327010849.png)

下面是 Dubbo 的服务治理图。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327010906.png)

### Dubbo 和 Spring Cloud 有什么区别？

两个没关联，如果硬要说区别，有以下几点。

**1、**通信方式不同

Dubbo 使用的是 RPC 通信，而 Spring Cloud 使用的是 HTTP RESTFul 方式。

**2、**组成部分不同

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327010937.png)



### dubbo都支持什么协议，推荐用哪种？

**1、**dubbo://（推荐）

**2、**rmi://

**3、**hessian://

**4、**http://

**5、**webservice://

**6、**thrift://

**7、**memcached://

**8、**redis://

**9、**rest://



### Dubbo推荐用什么协议?使用该协议有哪些优缺点?

传入传出参数数据包较小(建议小于100K)，消费者比提供者个数多，单一消费者无法压满提供者，尽量不要用dubbo协议传输大文件或超大字符串。



### 说说Dubbo的分层？

从大的范围来说，dubbo分为三层，business业务逻辑层由我们自己来提供接口和实现还有一些配置信息，RPC层就是真正的RPC调用的核心层，封装整个RPC的调用过程、负载均衡、集群容错、代理，remoting则是对网络传输协议和数据转换的封装。

划分到更细的层面，就是图中的10层模式，整个分层依赖由上至下，除开business业务逻辑之外，其他的几层都是SPI机制。

| 层级      | 功能           |
| --------- | -------------- |
| service   | 服务实现层     |
| config    | 配置相关       |
| proxy     | 代理层         |
| register  | 服务注册机制   |
| cluster   | 多个服务的治理 |
| monitor   | 单个服务监控   |
| protocol  | 协议层         |
| exchange  | 信息交换层     |
| transport | 传输层         |
| serialize | 持久化层       |



### Dubbo核心组件是？

- 生产者（Provider）：暴露服务的提供方，可以通过jar或者容器的方式启动服务；
- 消费者（Consumer）：调用远程服务的服务消费方；
- 注册中心（Registry）：服务注册中心和发现中心；
- 监控中心（Monitor）：统计服务和调用次数，调用时间监控中心；
- 服务容器（Container）：服务运行的容器，负责启动、加载，运行服务；

流程：首先`生产者`将服务注册到`注册中心`（zk），使用zk持久节点进行存储，消费订阅zk节点，一旦有节点变更，zk通过事件通知传递给`消费者`，消费可以调用生产者服务。服务与服务之间进行调用，都会在`监控中心`中，存储一个记录。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9RdLdzUL98jK2bZo1aTxd7BkvO2mlJ6KK8ZHyEicp7icoWPCBP9eNLTG32bd9jNN5409UaPDfoBd6UPKibtxzxTNQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### Dubbo核心配置有哪些？

核心配置有：

| **配置**           | **说明**     |
| ------------------ | ------------ |
| dubbo:service/     | 服务配置     |
| dubbo:reference/   | 引用配置     |
| dubbo:argument/    | 参数配置     |
| dubbo:protocol/    | 协议配置     |
| dubbo:registry/    | 注册中心配置 |
| dubbo:application/ | 应用配置     |
| dubbo:provider/    | 提供方配置   |
| dubbo:consumer/    | 消费方配置   |
| dubbo:method/      | 方法配置     |
| dubbo:module/      | 模块配置     |
| dubbo:monitor/     | 监控中心配置 |



### 能说下Dubbo的工作原理吗？

**1、** 服务启动的时候，provider和consumer根据配置信息，连接到注册中心register，分别向注册中心注册和订阅服务

**2、** register根据服务订阅关系，返回provider信息到consumer，同时consumer会把provider信息缓存到本地。如果信息有变更，consumer会收到来自register的推送

**3、** consumer生成代理对象，同时根据负载均衡策略，选择一台provider，同时定时向monitor记录接口的调用次数和时间信息

**4、** 拿到代理对象之后，consumer通过代理对象发起接口调用

**5、** provider收到请求后对数据进行反序列化，然后通过代理调用具体的接口实现



![图片](https://mmbiz.qpic.cn/mmbiz_png/9RdLdzUL98iaibjgVQMFxYM73JC6RiclYY7YY5OsnvicXBHI9KvS4KibZTicoia8tkSwTwHWH3l1OIM82AFgOPqxAhypA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

![img](https://img-blog.csdnimg.cn/20190308103242996.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3lnbDE5OTIwMTE5,size_16,color_FFFFFF,t_70)

 

### 介绍一下Dubbo框架分层？

从大的范围来说，Dubbo分为**3**层：`Business业务逻辑层`由我们自己来提供接口和实现还有一些配置信息，`RPC层`就是真正的RPC调用的核心层，封装整个RPC的调用过程、负载均衡、集群容错、代理，`Remoting层`则是对网络传输协议和数据转换的封装。

划分到更细的层面，就是**10**层模式，整个分层依赖由上至下，除开business业务逻辑之外，其他的几层都是SPI机制。10层模式如下：

- **`服务接口层`（Service）：** 与实际业务逻辑相关的，根据服务提供方和服务消费方的业务设计对应的接口和实现。
- **`配置层`（Config）：** 对外配置接口，以ServiceConfig和ReferenceConfig为中心，可以直接new配置类，也可以通过Spring解析配置生成配置类。
- **`服务代理层`（Proxy）：** 服务接口透明代理，生成服务的客户端Stub和服务器端Skeleton，以ServiceProxy为中心，扩展接口为ProxyFactory。
- **`服务注册层`（Registry）：** 封装服务地址的注册与发现，以服务URL为中心，扩展接口为RegistryFactory、Registry和RegistryService。可能没有服务注册中心，此时服务提供方直接暴露服务。
- **`集群层`（Cluster）：** 封装多个提供者的路由及负载均衡，并桥接注册中心，以Invoker为中心，扩展接口为Cluster、Directory、Router和LoadBalance。将多个服务提供方组合为一个服务提供方，实现对服务消费方来透明，只需要与一个服务提供方进行交互。
- **`监控层`（Monitor）：** RPC调用次数和调用时间监控，以Statistics为中心，扩展接口为MonitorFactory、Monitor和MonitorService。
- **`远程调用层`（Protocol）： **封将RPC调用，以Invocation和Result为中心，扩展接口为Protocol、Invoker和Exporter。Protocol是服务域，它是Invoker暴露和引用的主功能入口，它负责Invoker的生命周期管理。Invoker是实体域，它是Dubbo的核心模型，其它模型都向它靠扰，或转换成它，它代表一个可执行体，可向它发起invoke调用，它有可能是一个本地的实现，也可能是一个远程的实现，也可能一个集群实现。
- **`信息交换层`（Exchange）：** 封装请求响应模式，同步转异步，以Request和Response为中心，扩展接口为Exchanger、ExchangeChannel、ExchangeClient和ExchangeServer。
- **`网络传输层`（Transport）：** 抽象mina和netty为统一接口，以Message为中心，扩展接口为Channel、Transporter、Client、Server和Codec。
- **`数据序列化层`（Serialize）：** 可复用的一些工具，扩展接口为Serialization、 ObjectInput、ObjectOutput和ThreadPool。

![图片](https://mmbiz.qpic.cn/mmbiz_png/9RdLdzUL98iaibjgVQMFxYM73JC6RiclYY7on7FnXM4LJyZBZcS7WmKUXWS6sabU9DVTyufYV3LI4tnOYRH4Zw55A/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)





### 注册中心挂了可以继续通信吗？

可以，因为刚开始初始化的时候，消费者会将提供者的地址等信息拉取到本地缓存，所以注册中心挂了可以继续通信。



### Dubbo需要 Web 容器吗？

不需要，如果硬要用 Web 容器，只会增加复杂性，也浪费资源。



### Dubbo的执行流程

项目一启动，加载配置文件的时候，就会初始化，服务的提供方ServiceProvider就会向注册中心注册自己提供的服务，当消费者在启动时，就会向注册中心订阅自己所需要的服务，如果服务提供方有数据变更等，注册中心将基于长连接的形式推送变更数据给消费者。
默认使用Dubbo协议：
连接个数：单连接
连接方式：长连接
传输协议：TCP
传输方式：NIO异步传输
序列化：Hessian二进制序列化
适用范围：传入传出参数数据包较小（建议小于100K），消费者比提供者个数多，单一消费者无法压满提供者，尽量不要使用dubbo协议传输大文件或超大字符串
使用场景：常规远程服务方法调用
从上面的适用范围总结，dubbo适合小数据量大并发的服务调用，以及消费者机器远大于生产者机器数的情况，不适合传输大数据量的服务比如文件、视频等，除非请求量很低。



### Dubbo内置了哪几种服务容器？

- Spring Container
- Jetty Container
- Log4j Container

Dubbo 的服务容器只是一个简单的 Main 方法，并加载一个简单的 Spring 容器，用于暴露服务。



### Dubbo有哪些注册中心？

- **Multicast 注册中心：** Multicast 注册中心不需要任何中心节点，只要广播地址，就能进行服务注册和发现,基于网络中组播传输实现。
- **Zookeeper 注册中心：** 基于分布式协调系统 Zookeeper 实现，采用 Zookeeper 的 watch 机制实现数据变更。
- **Redis 注册中心：** 基于 Redis 实现，采用 key/map 存储，key 存储服务名和类型，map 中 key 存储服务 url，value 服务过期时间。基于 Redis 的发布/订阅模式通知数据变更。
- **Simple 注册中心：** Simple 注册中心本身就是一个普通的 Dubbo 服务，可以减少第三方依赖，使整体通讯方式一致。



### Dubbo里面有哪几种节点角色？

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327011121.png)



###  Dubbo中zookeeper做注册中心，如果注册中心集群都挂掉，发布者和订阅者之间还能通信么？

可以通信的，启动 dubbo 时，消费者会从 zk 拉取注册的生产者的地址接口等数据，缓存在本地。每次调用时，按照本地存储的地址进行调用；

注册中心对等集群，任意一台宕机后，将会切换到另一台；注册中心全部宕机后，服务的提供者和消费者仍能通过本地缓存通讯。服务提供者无状态，任一台 宕机后，不影响使用；服务提供者全部宕机，服务消费者会无法使用，并无限次重连等待服务者恢复；

挂掉是不要紧的，但前提是你没有增加新的服务，如果你要调用新的服务，则是不能办到的。



### 注册中心宕机，服务间是否可以继续通信

可以通信的，启动dubbo时，消费者会从zk拉取注册的生产者的地址接口等数据，缓存在本地。每次调用时，按照本地存储的地址进行调用；但前提是你没有增加新的服务，如果你要调用新的服务，则是不能办到的。另外如果服务的提供者全部宕机，服务消费者会无法使用，并无限次重连等待服务者恢复。



### Dubbo服务负载均衡策略？

**l Random LoadBalance**

随机，按权重设置随机概率。在一个截面上碰撞的概率高，但调用量越大分布越均匀，而且按概率使用权重后也比较均匀，有利于动态调整提供者权重。(权重可以在 dubbo 管控台配置) 

**l RoundRobin LoadBalance**

轮循，按公约后的权重设置轮循比率。存在慢的提供者累积请求问题，比如：第二台机器很慢，但没挂，当请求调到第二台时就卡在那，久而久之，所有请求都卡在调到第二台上。

**l LeastActive LoadBalance**

最少活跃调用数，相同活跃数的随机，活跃数指调用前后计数差。使慢的提供者收到更少请求，因为越慢的提供者的调用前后计数差会越大。

**l ConsistentHash LoadBalance**

一致性 Hash，相同参数的请求总是发到同一提供者。当某一台提供者挂时，原本发往该提供者的请求，基于虚拟节点，平摊到其它提供者，不会引起剧烈变动。缺省只对第一个参数 Hash，如果要修改，请配置

```
<dubbo:parameter key="hash.arguments" value="0,1" />
```

缺省用 160 份虚拟节点，如果要修改，请配置

```
<dubbo:parameter key="hash.nodes" value="320" />
```



### Dubbo在安全机制方面是如何解决的

Dubbo 通过 Token 令牌防止用户绕过注册中心直连，然后在注册中心上管理授权。Dubbo 还提供服务黑白名单，来控制服务所允许的调用方。



### Dubbo超时时间的设置

通过timeout属性配置超时时间,服务的提供者和消费者都可以配置，尽量在服务提供者中配置，因为服务的提供者会对自己提供的服务情况更清楚超时时间不要设置太大(1~5S),会影响并发性能问题。





### 画一画服务注册与发现的流程图

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327011132.png)

该图来自 Dubbo 官网，供你参考，如果你说你熟悉 Dubbo, 面试官经常会让你画这个图，记好了。



### Dubbo默认使用什么注册中心，还有别的选择吗？

推荐使用 Zookeeper 作为注册中心，还有 Redis、Multicast、Simple 注册中心，但不推荐。



### Dubbo有哪几种配置方式？

- XML 配置文件方式；
- properties 配置文件方式；
- annotation 配置方式；
- API 配置方式；



### Dubbo 核心的配置有哪些？

我曾经面试就遇到过面试官让你写这些配置，我也是蒙逼。。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327011334.png)

配置之间的关系见下图。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327011346.png)



### 在 Provider 上可以配置的 Consumer 端的属性有哪些？

**1、** timeout：方法调用超时
**2、** retries：失败重试次数，默认重试 2 次
**3、** loadbalance：负载均衡算法，默认随机
**4、** actives 消费者端，最大并发调用限制



### Dubbo启动时如果依赖的服务不可用会怎样？

Dubbo 缺省会在启动时检查依赖的服务是否可用，不可用时会抛出异常，阻止 Spring 初始化完成，默认 check="true"，可以通过 check="false" 关闭检查。



### Dubbo支持哪些序列化方式?

**dubbo序列化：** 阿里尚未开发成熟的高效java序列化实现，阿里不建议在生产环境使用它。

**hessian2序列化(默认推荐)：** hessian是一种跨语言的高效二进制序列化方式。但这里实际不是原生的hessian2序列化，而是阿里修改过的hessian lite，它是dubbo RPC默认启用的序列化方式。

**json序列化：** 目前有两种实现，一种是采用的阿里的fastjson库，另一种是采用dubbo中自己实现的简单json库，但其实现都不是特别成熟，而且json这种文本序列化性能一般不如上面两种二进制序列化。

**java序列化：** 主要是采用JDK自带的Java序列化实现，性能很不理想。



### Dubbo推荐使用什么序列化框架，你知道的还有哪些？

默认使用 Hessian 序列化，还有 Duddo、FastJson、Java 自带序列化。hessian是一个采用二进制格式传输的服务框架，相对传统soap web service，更轻量，更快速。

Hessian原理与协议简析：

http的协议约定了数据传输的方式，hessian也无法改变太多：

**1、**  hessian中client与server的交互，基于http-post方式。

**2、** hessian将辅助信息，封装在http header中，比如“授权token”等，我们可以基于http-header来封装关于“安全校验”“meta数据”等。hessian提供了简单的”校验”机制。

**3、 **对于hessian的交互核心数据，比如“调用的方法”和参数列表信息，将通过post请求的body体直接发送，格式为字节流。

**4、** 对于hessian的server端响应数据，将在response中通过字节流的方式直接输出。

hessian的协议本身并不复杂，在此不再赘言；所谓协议(protocol)就是约束数据的格式，client按照协议将请求信息序列化成字节序列发送给server端，server端根据协议，将数据反序列化成“对象”，然后执行指定的方法，并将方法的返回值再次按照协议序列化成字节流，响应给client，client按照协议将字节流反序列话成”对象”。



### Dubbo默认使用的是什么通信框架，还有别的选择吗？

Dubbo 默认使用 Netty 框架，也是推荐的选择，另外内容还集成有Mina、Grizzly。



### Dubbo有哪几种集群容错方案，哪几种负载均衡策略？

在集群调用失败时，Dubbo 提供了多种容错方案，缺省为 failover 重试。具体的集群容错方案有：

| **集群容错方案**  | **说明**                                   |
| ----------------- | ------------------------------------------ |
| Failover Cluster  | 失败自动切换，自动重试其他服务器（默认）   |
| Failfast Cluster  | 快速失败，立即报错，只发起一次调用         |
| Failsafe Cluster  | 失败安全，出现异常时，直接忽略             |
| Failback Cluster  | 失败自动恢复，记录失败请求，定时重发       |
| Forking Cluster   | 并行调用多个服务器，只要一个成功即返回     |
| Broadcast Cluster | 广播逐个调用所有提供者，任意一个报错则报错 |



Dubbo内置了4种负载均衡策略：

| **负载均衡策略**          | **说明**                                               |
| ------------------------- | ------------------------------------------------------ |
| RandomLoadBalance         | 随机负载均衡，按权重设置随机概率（默认）               |
| RoundRobinLoadBalance     | 轮询负载均衡，按公约后的权重设置轮询比率               |
| LeastActiveLoadBalance    | 最少活跃调用数，相同活跃数的随机                       |
| ConsistentHashLoadBalance | 一致性Hash负载均衡，相同参数的请求总是发到同一个提供者 |



### Dubbo用到哪些设计模式，简要介绍？

- **工厂模式：** Provider在export服务时，会调用ServiceConfig的export方法，实现类的获取采用了JDK SPI的机制，想要扩展实现，只需要在classpath下增加文件即可，代码零侵入；
- **装饰器模式：** Dubbo在启动和调用阶段都大量使用了装饰器模式，如ClassLoaderFilter在主功能上添加功能，更改当前线程的ClassLoader是典型的装饰器模式；
- **观察者模式：** Dubbo的Provider启动时，需要与注册中心交互，先注册自己的服务，再订阅自己的服务，订阅时，采用了观察者模式；
- **动态代理模式：** Dubbo扩展JDK SPI的类ExtensionLoader的Adaptive实现是典型的动态代理实现，Dubbo需要灵活地控制实现类，即在调用阶段动态地根据参数决定调用哪个实现类，所以采用先生成代理类的方法，做到灵活的调用。



### 注册了多个同一样的服务，如果测试指定的某一个服务呢？

可以配置环境点对点直连，绕过注册中心，将以服务接口为单位，忽略注册中心的提供者列表。



### Dubbo支持服务多协议吗？

Dubbo 允许配置多协议，在不同服务上支持不同协议或者同一服务上同时支持多种协议。



### Dubbo 支持哪些协议，每种协议的应用场景，优缺点？

**1.dubbo默认协议：**

- 单一 TCP 长连接，Hessian 二进制序列化和 NIO 异步通讯；
- 适合于小数据包大并发的服务调用和服务消费者数远大于服务提供者数的情况；
- 不适合传送大数据包的服务；

 

**2.rmi协议：**

- 采用 JDK 标准的 java.rmi.* 实现，阻塞式短连接和 JDK 标准序列化方式；
- 如果服务接口继承了 java.rmi.Remote 接口，可以和原生 RMI 互操作；
- 因反序列化漏洞，需升级 commons-collections3 到 3.2.2版本或 commons-collections4 到 4.1 版本；
- 对传输数据包不限，消费者和传输者个数相当；

 

**3.hessian协议：**

- 底层 Http 通讯，Servlet 暴露服务，Dubbo 缺省内嵌 Jetty 作为服务器实现；
- 可与原生 Hessian 服务互操作；
- 通讯效率高于 WebService 和 Java 自带的序列化；
- 参数及返回值需实现 Serializable 接口，自定义实现 List、Map、Number、Date、Calendar 等接口；
- 适用于传输数据包较大，提供者比消费者个数多，提供者压力较大；

 

**4.http协议：**

- 基于 http 表单的远程调用协议，短连接，json 序列化；
- 对传输数据包不限，不支持传文件；
- 适用于同时给应用程序和浏览器 JS 使用的服务；

 

**5.webservice协议：**

- 基于Apache CXF 的frontend-simple和transports-http 实现，短连接，SOAP文本序列化；
- 可与原生WebService服务互操作；
- 适用于系统集成、跨语言调用；

 

**6.thrift协议：**

- 对 thrift 原生协议的扩展添加了额外的头信息；
- 使用较少，不支持传 null 值；

 

**7.redis协议:**

- redis在TCP端口6379上监听到来的连接，客户端连接到来时，Redis服务器为此创建一个TCP连接 ;
- redis接收由不同参数组成的命令。一旦收到命令，将会立刻被处理，并回复给客户端;



**8.memcached协议:**

- 客户端使用TCP链接与服务器通讯，一个运行中的memcached服务器监视一些端口，客户端连接这些端口，发送命令到服务器，读取回应，最后关闭连接;
- memcached协议中发送的数据分为文本行和自由数据两种；



### Dubbo 集群的负载均衡有哪些策略

Dubbo 提供了常见的集群策略实现，并预扩展点予以自行实现。

**Random LoadBalance:** 随机选取提供者策略，有利于动态调整提供者权重。截面碰撞率高，调用次数越多，分布越均匀；

**RoundRobin LoadBalance:** 轮循选取提供者策略，平均分布，但是存在请求累积的问题；

**LeastActive LoadBalance:** 最少活跃调用策略，解决慢提供者接收更少的请求；ConstantHash LoadBalance: 一致性 Hash 策略，使相同参数请求总是发到同一提供者，一台机器宕机，可以基于虚拟节点，分摊至其他提供者，避免引起提供者的剧烈变动；



### 当一个服务接口有多种实现时怎么做？

当一个接口有多种实现时，可以用 group 属性来分组，服务提供方和消费方都指定同一个 group 即可。



### 服务调用超时问题怎么解决

dubbo在调用服务不成功时，默认是会重试两次的。这样在服务端的处理时间超过了设定的超时时间时，就会有重复请求，比如在发邮件时，可能就会发出多份重复邮件，执行注册请求时，就会插入多条重复的注册数据，那么怎么解决超时问题呢？如下对于核心的服务中心，去除dubbo超时重试机制，并重新评估设置超时时间。业务处理代码必须放在服务端，客户端只做参数验证和服务调用，不涉及业务流程处理 全局配置实例

```
<dubbo:provider delay="-1" timeout="6000" retries="0"/>
```

当然Dubbo的重试机制其实是非常好的QOS保证，它的路由机制，是会帮你把超时的请求路由到其他机器上，而不是本机尝试，所以 dubbo的重试机器也能一定程度的保证服务的质量。但是请一定要综合线上的访问情况，给出综合的评估。



### 服务上线怎么兼容旧版本？

可以用版本号（version）过渡，多个不同版本的服务注册到注册中心，版本号不同的服务相互间不引用。这个和服务分组的概念有一点类似。



### Dubbo可以对结果进行缓存吗？

可以，Dubbo 提供了声明式缓存，用于加速热门数据的访问速度，以减少用户加缓存的工作量。



### Dubbo服务之间的调用是阻塞的吗？

默认是同步等待结果阻塞的，支持异步调用。

Dubbo 是基于 NIO 的非阻塞实现并行调用，客户端不需要启动多线程即可完成并行调用多个远程服务，相对多线程开销较小，异步调用会返回一个 Future 对象。

异步调用流程图如下。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327011636.png)



### Dubbo支持分布式事务吗？

目前暂时不支持，后续可能采用基于 JTA/XA 规范实现，如以图所示。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327011653.png)



### Dubbo的心跳机制

**目的：**
维持provider和consumer之间的长连接

**实现：**
dubbo心跳时间heartbeat默认是1s，超过heartbeat时间没有收到消息，就发送心跳消 息(provider，consumer一样),如果连着3次(heartbeatTimeout为heartbeat*3)没有收到心跳响应，provider会关闭channel，而consumer会进行重连;不论是provider还是consumer的心跳检测都是通过启动定时任务的方式实现；



### Dubbo的zookeeper做注册中心，如果注册中心全部挂掉，发布者和订阅者还能通信吗？
可以通信的，启动dubbo时，消费者会从zk拉取注册的生产者的地址接口等数据，缓存在本地。每次调用时，按照本地存储的地址进行调用；
注册中心对等集群，任意一台宕机后，将会切换到另一台；注册中心全部宕机后，服务的提供者和消费者仍能通过本地缓存通讯。服务提供者无状态，任一台 宕机后，不影响使用；服务提供者全部宕机，服务消费者会无法使用，并无限次重连等待服务者恢复；
挂掉是不要紧的，但前提是你没有增加新的服务，如果你要调用新的服务，则是不能办到的。



### Dubbo telnet 命令能做什么？

dubbo 通过 telnet 命令来进行服务治理

```
telnet localhost 8090
```



### 说说服务暴露的流程？

**1、** 在容器启动的时候，通过ServiceConfig解析标签，创建dubbo标签解析器来解析dubbo的标签，容器创建完成之后，触发ContextRefreshEvent事件回调开始暴露服务

**2、** 通过ProxyFactory获取到invoker，invoker包含了需要执行的方法的对象信息和具体的URL地址

**3、** 再通过DubboProtocol的实现把包装后的invoker转换成exporter，然后启动服务器server，监听端口

**4、** 最后RegistryProtocol保存URL地址和invoker的映射关系，同时注册到服务中心



![img](https://pic4.zhimg.com/80/v2-e9548bd49a572b6bf62fed16954ea493_720w.jpeg)



### 说说服务引用的流程？

服务暴露之后，客户端就要引用服务，然后才是调用的过程。

**1、** 首先客户端根据配置文件信息从注册中心订阅服务

**2、** 之后DubboProtocol根据订阅的得到provider地址和接口信息连接到服务端server，开启客户端client，然后创建invoker

**3、** invoker创建完成之后，通过invoker为服务接口生成代理对象，这个代理对象用于远程调用provider，服务的引用就完成了



![img](https://pic1.zhimg.com/80/v2-6eb15826a4dc44e0f592055ae9089690_720w.jpeg)



### 有哪些负载均衡策略？

**1、加权随机：** 假设我们有一组服务器 servers = [A, B, C]，他们对应的权重为 weights = [5, 3, 2]，权重总和为10。现在把这些权重值平铺在一维坐标值上，[0, 5) 区间属于服务器 A，[5, 8) 区间属于服务器 B，[8, 10) 区间属于服务器 C。接下来通过随机数生成器生成一个范围在 [0, 10) 之间的随机数，然后计算这个随机数会落到哪个区间上就可以了。

**2、最小活跃数：** 每个服务提供者对应一个活跃数 active，初始情况下，所有服务提供者活跃数均为0。每收到一个请求，活跃数加1，完成请求后则将活跃数减1。在服务运行一段时间后，性能好的服务提供者处理请求的速度更快，因此活跃数下降的也越快，此时这样的服务提供者能够优先获取到新的服务请求。

**3、一致性hash：** 通过hash算法，把provider的invoke和随机节点生成hash，并将这个 hash 投射到 [0, 2^32 - 1] 的圆环上，查询的时候根据key进行md5然后进行hash，得到第一个节点的值大于等于当前hash的invoker。



### Dubbo如何优雅停机？

Dubbo 是通过 JDK 的 ShutdownHook 来完成优雅停机的，所以如果使用 kill -9 PID 等强制关闭指令，是不会执行优雅停机的，只有通过 kill PID 时，才会执行。



### 了解Dubbo SPI机制吗？

SPI 全称为 Service Provider Interface，是一种服务发现机制，本质是将接口实现类的全限定名配置在文件中，并由服务加载器读取配置文件，加载实现类，这样可以在运行时，动态为接口替换实现类。

Dubbo也正是通过SPI机制实现了众多的扩展功能，而且dubbo没有使用java原生的SPI机制，而是对齐进行了增强和改进。

SPI在dubbo应用很多，包括协议扩展、集群扩展、路由扩展、序列化扩展等等。

使用方式可以在META-INF/dubbo目录下配置：

key=com.xxx.value

然后通过dubbo的Extensier按照指定的key加载对应的实现类，这样做的好处就是可以按需加载，性能上得到优化。



### 如果让你实现一个RPC框架怎么设计？

**1、** 首先需要一个服务注册中心，这样consumer和provider才能去注册和订阅服务

**2、** 需要负载均衡的机制来决定consumer如何调用客户端，这其中还当然要包含容错和重试的机制

**3、** 需要通信协议和工具框架，比如通过http或者rmi的协议通信，然后再根据协议选择使用什么框架和工具来进行通信，当然，数据的传输序列化要考虑

**4、** 除了基本的要素之外，像一些监控、配置管理页面、日志是额外的优化考虑因素。

那么，本质上，只要熟悉一两个RPC框架，就很容易想明白我们自己要怎么实现一个RPC框架。



### 服务提供者能实现失效踢出是什么原理？

服务失效踢出基于 Zookeeper 的临时节点原理。



### 如何解决服务调用链过长的问题？

Dubbo 可以使用 Pinpoint 和 Apache Skywalking(Incubator) 实现分布式服务追踪，当然还有其他很多方案。



### 服务读写推荐的容错策略是怎样的？

读操作建议使用 Failover 失败自动切换，默认重试两次其他服务器。

写操作建议使用 Failfast 快速失败，发一次调用失败就立即报错。



### Dubbo必须依赖的包有哪些？

Dubbo 必须依赖 JDK，其他为可选。



### Dubbo的管理控制台能做什么？

管理控制台主要包含：路由规则，动态配置，服务降级，访问控制，权重调整，负载均衡，等管理功能。



### 说说 Dubbo 服务暴露的过程。

Dubbo 会在 Spring 实例化完 bean 之后，在刷新容器最后一步发布 ContextRefreshEvent 事件的时候，通知实现了 ApplicationListener 的 ServiceBean 类进行回调 onApplicationEvent 事件方法，Dubbo 会在这个方法中调用 ServiceBean 父类 ServiceConfig 的 export 方法，而该方法真正实现了服务的（异步或者非异步）发布。



### Dubbo 停止维护了吗？

2014 年开始停止维护过几年，17 年开始重新维护，并进入了 Apache 项目。



### Dubbo 和 Dubbox 有什么区别？

Dubbox 是继 Dubbo 停止维护后，当当网基于 Dubbo 做的一个扩展项目，如加了服务可 Restful 调用，更新了开源组件等。



### 在使用过程中都遇到了些什么问题？如何解决的？

**1、** 同时配置了 XML 和 properties 文件，则 properties 中的配置无效只有 XML 没有配置时，properties 才生效。

**2、** dubbo 缺省会在启动时检查依赖是否可用，不可用就抛出异常，阻止 spring 初始化完成，check 属性默认为 true。测试时有些服务不关心或者出现了循环依赖，将 check 设置为 false

**3、** 为了方便开发测试，线下有一个所有服务可用的注册中心，这时，如果有一个正在开发中的服务提供者注册，可能会影响消费者不能正常运行。

解决：让服务提供者开发方，只订阅服务，而不注册正在开发的服务，通过直连测试正在开发的服务。设置 dubbo:registry 标签的 register 属性为 false。

**4、** spring 2.x 初始化死锁问题。在 spring 解析到 dubbo:service 时，就已经向外暴露了服务，而 spring 还在接着初始化其他 bean，如果这时有请求进来，并且服务的实现类里有调用 applicationContext.getBean() 的用法。getBean 线程和 spring 初始化线程的锁的顺序不一样，导致了线程死锁，不能提供服务，启动不了。

解决：不要在服务的实现类中使用 applicationContext.getBean(); 如果不想依赖配置顺序，可以将 dubbo:provider 的 deplay 属性设置为 - 1，使 dubbo 在容器初始化完成后再暴露服务。

**5、** 服务注册不上

检查 dubbo 的 jar 包有没有在 classpath 中，以及有没有重复的 jar 包

检查暴露服务的 spring 配置有没有加载

在服务提供者机器上测试与注册中心的网络是否通

**6、** 出现 RpcException: No provider available for remote service 异常

表示没有可用的服务提供者，

- 检查连接的注册中心是否正确

- 到注册中心查看相应的服务提供者是否存在

- 检查服务提供者是否正常运行

**7、** 出现” 消息发送失败” 异常

通常是接口方法的传入传出参数未实现 Serializable 接口。



### 你还了解别的分布式框架吗？

别的还有 Spring cloud、Facebook 的 Thrift、Twitter 的 Finagle 等。

