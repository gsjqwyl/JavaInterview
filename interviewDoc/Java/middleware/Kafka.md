**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [什么是kafka](#什么是kafka)
- [Kafka 都有哪些特点？](#kafka-都有哪些特点)
- [请说明Kafka相对传统技术有什么优势?](#请说明kafka相对传统技术有什么优势)
- [Kafka的优势是什么？](#kafka的优势是什么)
- [Kafka消息传递系统与其他消息传递框架有何不同？](#kafka消息传递系统与其他消息传递框架有何不同)
- [在Kafka中，领导者和追随者是什么意思？](#在kafka中领导者和追随者是什么意思)
- [你知道Kafka的不同组成部分吗？](#你知道kafka的不同组成部分吗)
- [Zookeeper在Kafka的重要性是什么？](#zookeeper在kafka的重要性是什么)
- [Kafka的抵消额是多少？](#kafka的抵消额是多少)
- [请简述下你在哪些场景下会选择 Kafka？](#请简述下你在哪些场景下会选择-kafka)
- [Kafka 缺点？](#kafka-缺点)
- [你们Kafka集群的硬盘一共多大？有多少台机器？日志保存多久？用什么监控的？](#你们kafka集群的硬盘一共多大有多少台机器日志保存多久用什么监控的)
- [Kafka分区数、副本数和topic数量多少比较合适？](#kafka分区数副本数和topic数量多少比较合适)
- [Kafka 可以脱离 zookeeper 单独使用吗？为什么？](#kafka-可以脱离-zookeeper-单独使用吗为什么)
- [Kafka为什么不支持读写分离？](#kafka为什么不支持读写分离)
- [Java Consumer 为什么采用单线程来获取消息？](#java-consumer-为什么采用单线程来获取消息)
- [解释Kafka的Zookeeper是什么?我们可以在没有Zookeeper的情况下使用Kafka吗?](#解释kafka的zookeeper是什么我们可以在没有zookeeper的情况下使用kafka吗)
- [解释一下，在数据制作过程中，你如何能从Kafka得到准确的信息?](#解释一下在数据制作过程中你如何能从kafka得到准确的信息)
- [Consumer与topic关系](#consumer与topic关系)
- [Kafka 的设计架构你知道吗？](#kafka-的设计架构你知道吗)
- [Kafka 分区的目的？](#kafka-分区的目的)
- [Kafka中的消息有序吗？怎么实现的？](#kafka中的消息有序吗怎么实现的)
- [你知道 Kafka 是如何做到消息的有序性？](#你知道-kafka-是如何做到消息的有序性)
- [为什么要使用 kafka，为什么要使用消息队列](#为什么要使用-kafka为什么要使用消息队列)
- [Kafka中的ISR、AR又代表什么？ISR的伸缩又指什么](#kafka中的israr又代表什么isr的伸缩又指什么)
- [LEO、HW、LSO、LW等分别代表什么](#leohwlsolw等分别代表什么)
- [Kafka 消费者是否可以消费指定分区消息？](#kafka-消费者是否可以消费指定分区消息)
- [Kafka消息是采用Pull模式，还是Push模式？](#kafka消息是采用pull模式还是push模式)
- [Kafka 高效文件存储设计特点](#kafka-高效文件存储设计特点)
- [kafka中的broker 是干什么的](#kafka中的broker-是干什么的)
- [Kafka创建Topic时如何将分区放置到不同的Broker中](#kafka创建topic时如何将分区放置到不同的broker中)
- [topic的分区数可以增加或减少吗？为什么？](#topic的分区数可以增加或减少吗为什么)
- [你知道kafka是怎么维护offset的吗？](#你知道kafka是怎么维护offset的吗)
- [你们是怎么对Kafka进行压测的？](#你们是怎么对kafka进行压测的)
- [当Kafka消息数据出现了积压，应该怎么处理？](#当kafka消息数据出现了积压应该怎么处理)
- [聊聊Kafka分区分配策略？](#聊聊kafka分区分配策略)
- [谈谈你对Kafka幂等性的理解？](#谈谈你对kafka幂等性的理解)
- [你对Kafka事务了解多少？](#你对kafka事务了解多少)
- [Kafka怎么实现如此高的读写效率？](#kafka怎么实现如此高的读写效率)
- [Kafka新建的分区会在哪个目录下创建](#kafka新建的分区会在哪个目录下创建)
- [**什么是消费者组？**](#什么是消费者组)
- [**kafka中的 zookeeper 起到什么作用，可以不用zookeeper么**](#kafka中的-zookeeper-起到什么作用可以不用zookeeper么)
- [Kafka 为什么那么快](#kafka-为什么那么快)
- [谈一谈 Kafka 的再均衡](#谈一谈-kafka-的再均衡)
- [Kafka 是如何实现高吞吐率的？](#kafka-是如何实现高吞吐率的)
- [**如何设置Kafka能接收的最大消息的大小？**](#如何设置kafka能接收的最大消息的大小)
- [**监控Kafka的框架都有哪些？**](#监控kafka的框架都有哪些)
- [**如何估算Kafka集群的机器数量？**](#如何估算kafka集群的机器数量)
- [**Kafka能手动删除消息吗？**](#kafka能手动删除消息吗)
- [**consumeroffsets是做什么用的？**](#consumeroffsets是做什么用的)
- [Kafka Stream的一些独特功能是什么？](#kafka-stream的一些独特功能是什么)
- [为什么说Kafka是分布式流媒体平台？](#为什么说kafka是分布式流媒体平台)

<!-- /TOC -->

### **什么是kafka**

Kafka是分布式发布-订阅消息系统，它最初是由LinkedIn公司开发的，之后成为Apache项目的一部分，Kafka是一个分布式，可划分的，冗余备份的持久性的日志服务，它主要用于处理流式数据。



### Kafka 都有哪些特点？

- 高吞吐量、低延迟：kafka每秒可以处理几十万条消息，它的延迟最低只有几毫秒，每个topic可以分多个partition, consumer group 对partition进行consume操作。
- 可扩展性：kafka集群支持热扩展
- 持久性、可靠性：消息被持久化到本地磁盘，并且支持数据备份防止数据丢失
- 容错性：允许集群中节点失败（若副本数量为n,则允许n-1个节点失败）
- 高并发：支持数千个客户端同时读写



### 请说明Kafka相对传统技术有什么优势?

Apache Kafka与传统的消息传递技术相比优势之处在于：

**快速:** 单一的Kafka代理可以处理成千上万的客户端，每秒处理数兆字节的读写操作。

**可伸缩:** 在一组机器上对数据进行分区和简化，以支持更大的数据

**持久:** 消息是持久性的，并在集群中进行复制，以防止数据丢失。

**设计:** 它提供了容错保证和持久性



### Kafka的优势是什么？

Kafka的主要优点包括容错，更高的吞吐量，可伸缩性，更低的延迟和耐用性。Kafka不需要任何大型硬件组件，并且在管理高容量和高速数据方面显示出卓越的性能。

最重要的是，它可以以每秒数千条消息的速率支持消息吞吐量。Kafka描述了对集群中节点或机器故障的有希望的抵制。Kafka的较低延迟可以帮助在毫秒内轻松管理消息。此外，Kafka还确保消息复制，从而减少了对消息丢失的担忧。Apache Kafka的另一个关键优势是可通过添加更多节点来确保可伸缩性。



### Kafka消息传递系统与其他消息传递框架有何不同？

- 该设计遵循公共订购模型。
- 无缝支持Spark和其他大数据技术。
- 支持集群模式操作。
- 容错功能可减少对消息丢失的担忧。
- 支持Scala和Java编程语言。
- 易于编码和配置。
- Web服务体系结构以及大数据体系结构的理想选择。



### 在Kafka中，领导者和追随者是什么意思？

Kafka中的每个分区都与一台充当领导者角色的服务器相关联，另一台服务器充当跟随者角色。

领导者负责执行有关分区的所有读取和写入请求。另一方面，追随者必须被动地复制领导者。如果领导者失败，则跟随者之一可以担当领导者角色，以确保负载平衡。



### 你知道Kafka的不同组成部分吗？

Kafka有四个主要组成部分，例如主题、生产者、经纪人和消费者。Kafka中的主题是同一类型的消息流。



Kafka中的Producer可以帮助你将消息发布到某个主题。代理是一组服务器，用于存储生产者发布的消息。消费者是Kafka组件，它有助于订阅不同的主题并从中间商获取数据。



### Zookeeper在Kafka的重要性是什么？


Zookeeper主要负责开发集群中不同节点之间的协调。Zookeeper可以帮助在节点发生故障时从先前提交的偏移恢复到偏移，因为它可以作为定期提交偏移进行工作。

此外，Zookeeper还有助于领导者检测，配置管理，同步以及检测离开或加入集群的任何节点。此外，Kafka将Zookeeper用作存储有关特定主题的已消耗消息的偏移量的存储。Zookeeper还可以帮助根据特定的消费者组对消息的偏移量进行分区。



### Kafka的抵消额是多少？

Kafka中的偏移量是分配给分区中消息的顺序ID号。偏移量有助于特定分区中每个消息的唯一标识。



### 请简述下你在哪些场景下会选择 Kafka？

- 日志收集：一个公司可以用Kafka可以收集各种服务的log，通过kafka以统一接口服务的方式开放给各种consumer，例如hadoop、HBase、Solr等。
- 消息系统：解耦和生产者和消费者、缓存消息等。
- 用户活动跟踪：Kafka经常被用来记录web用户或者app用户的各种活动，如浏览网页、搜索、点击等活动，这些活动信息被各个服务器发布到kafka的topic中，然后订阅者通过订阅这些topic来做实时的监控分析，或者装载到hadoop、数据仓库中做离线分析和挖掘。
- 运营指标：Kafka也经常用来记录运营监控数据。包括收集各种分布式应用的数据，生产各种操作的集中反馈，比如报警和报告。
- 流式处理：比如spark streaming和 Flink



### Kafka 缺点？

- 由于是批量发送，数据并非真正的实时；
- 对于mqtt协议不支持；
- 不支持物联网传感数据直接接入；
- 仅支持统一分区内消息有序，无法实现全局消息有序；
- 监控不完善，需要安装插件；
- 依赖zookeeper进行元数据管理；



### 你们Kafka集群的硬盘一共多大？有多少台机器？日志保存多久？用什么监控的？

这里考察应试者对kafka实际生产部署的能力，也是为了验证能力的真实程度，如果这个都答不好，那可能就不会再继续下去了。

一般企业判断这些指标有一个标准：

集群硬盘大小：每天的数据量/70%*日志保存天数；

机器数量：Kafka 机器数量=2*（峰值生产速度*副本数/100）+1；

日志保存时间：可以回答保存7天；

监控Kafka：一般公司有自己开发的监控器，或者cdh配套的监控器，另外还有一些开源的监控器：kafkaeagle、KafkaMonitor、KafkaManager。



### Kafka分区数、副本数和topic数量多少比较合适？

首先要知道**分区数并不是越多越好**，一般分区数不要超过集群机器数量。分区数越多占用内存越大 （ISR 等），一个节点集中的分区也就越多，当它宕机的时候，对系统的影响也就越大。

分区数一般设置为：3-10 个。

副本数一般设置为：2-3个。

topic数量需要根据日志类型来定，一般有多少个日志类型就定多少个topic，不过也有对日志类型进行合并的。



### Kafka 可以脱离 zookeeper 单独使用吗？为什么？

kafka 不能脱离 zookeeper 单独使用，因为 kafka 使用 zookeeper 管理和协调 kafka 的节点服务器。



### Kafka为什么不支持读写分离？

**如果支持了读写分离，就意味着可能的数据不一致，或数据滞后。**这其实是分布式场景下的通用问题，因为我们知道CAP理论下，我们只能保证C（可用性）和A（一致性）取其一，如果支持读写分离，那其实对于一致性的要求可能就会有一定折扣，因为通常的场景下，副本之间都是通过同步来实现副本数据一致的，那同步过程中肯定会有时间的消耗。

 

Leader/Follower模型并没有规定Follower副本不可以对外提供读服务。很多框架都是允许这么做的，只是 Kafka最初为了避免不一致性的问题，而采用了让Leader统一提供服务的方式。

 

不过，自Kafka 2.4之后，Kafka提供了有限度的读写分离，也就是说，Follower副本能够对外提供读服务。



### Java Consumer 为什么采用单线程来获取消息？

首先，Java Consumer是双线程的设计。其中一个线程是用户主线程，负责获取消息；另一个线程是心跳线程，负责向Kafka汇报消费者存活情况。将心跳单独放入专属的线程，能够有效地规避因消息处理速度慢而被视为下线的“假死”情况。

 

单线程获取消息的设计能够避免阻塞式的消息获取方式。单线程轮询方式容易实现异步非阻塞式，这样便于将消费者扩展成支持实时流处理的操作算子。因为很多实时流处理操作算子都不能是阻塞式的。

 

另外一个可能的好处是，可以简化代码的开发。多线程交互的代码是非常容易出错的。



### 解释Kafka的Zookeeper是什么?我们可以在没有Zookeeper的情况下使用Kafka吗?

Zookeeper是一个开放源码的、高性能的协调服务，它用于Kafka的分布式应用。不，不可能越过Zookeeper，直接联系Kafka broker。一旦Zookeeper停止工作，它就不能服务客户端请求。

Zookeeper主要用于在集群中不同节点之间进行通信

在Kafka中，它被用于提交偏移量，因此如果节点在任何情况下都失败了，它都可以从之前提交的偏移量中获取

除此之外，它还执行其他活动，如: leader检测、分布式同步、配置管理、识别新节点何时离开或连接、集群、节点实时状态等等。



### 解释一下，在数据制作过程中，你如何能从Kafka得到准确的信息?

在数据中，为了精确地获得Kafka的消息，你必须遵循两件事: 在数据消耗期间避免重复，在数据生产过程中避免重复。

这里有两种方法，可以在数据生成时准确地获得一个语义:

每个分区使用一个单独的写入器，每当你发现一个网络错误，检查该分区中的最后一条消息，以查看您的最后一次写入是否成功

在消息中包含一个主键(UUID或其他)，并在用户中进行反复制



### Consumer与topic关系

每个group中可以有多个consumer，每个consumer属于一个consumer group，通常情况下，一个group中会包含多个consumer，这样不仅可以提高topic中消息的并发消费能力，而且还能提高"故障容错"性，如果group中的某个consumer失效那么其消费的partitions将会有其他consumer自动接管。

对于Topic中的一条特定的消息，只会被订阅此Topic的每个group中的其中一个consumer消费，此消息不会发送给一个group的多个consumer,不过一个consumer可以同时消费多个partitions中的消息。



### Kafka 的设计架构你知道吗？

Kafka 架构分为以下几个部分

- Producer ：消息生产者，就是向 kafka broker 发消息的客户端。
- Consumer ：消息消费者，向 kafka broker 取消息的客户端。
- Topic ：可以理解为一个队列，一个 Topic 又分为一个或多个分区，
- Consumer Group：这是 kafka 用来实现一个 topic 消息的广播（发给所有的 consumer）和单播（发给任意一个 consumer）的手段。一个 topic 可以有多个 Consumer Group。
- Broker ：一台 kafka 服务器就是一个 broker。一个集群由多个 broker 组成。一个 broker 可以容纳多个 topic。
- Partition：为了实现扩展性，一个非常大的 topic 可以分布到多个 broker上，每个 partition 是一个有序的队列。partition 中的每条消息都会被分配一个有序的id（offset）。将消息发给 consumer，kafka 只保证按一个 partition 中的消息的顺序，不保证一个 topic 的整体（多个 partition 间）的顺序。
- Offset：kafka 的存储文件都是按照 offset.kafka 来命名，用 offset 做名字的好处是方便查找。例如你想找位于 2049 的位置，只要找到 2048.kafka 的文件即可。当然 the first offset 就是 00000000000.kafka。



### Kafka 分区的目的？

分区对于 Kafka 集群的好处是：实现负载均衡。分区对于消费者来说，可以提高并发度，提高效率。



### Kafka中的消息有序吗？怎么实现的？

kafka无法保证整个topic多个分区有序，但是由于每个分区（partition）内，每条消息都有一个offset，故**可以保证分区内有序**。



### 你知道 Kafka 是如何做到消息的有序性？

kafka 中的每个 partition 中的消息在写入时都是有序的，而且单独一个 partition 只能由一个消费者去消费，可以在里面保证消息的顺序性。但是分区之间的消息是不保证有序的。



### 为什么要使用 kafka，为什么要使用消息队列

**缓冲和削峰：**上游数据时有突发流量，下游可能扛不住，或者下游没有足够多的机器来保证冗余，kafka在中间可以起到一个缓冲的作用，把消息暂存在kafka中，下游服务就可以按照自己的节奏进行慢慢处理。

**解耦和扩展性：**项目开始的时候，并不能确定具体需求。消息队列可以作为一个接口层，解耦重要的业务流程。只需要遵守约定，针对数据编程即可获取扩展能力。

**冗余：**可以采用一对多的方式，一个生产者发布消息，可以被多个订阅topic的服务消费到，供多个毫无关联的业务使用。

**健壮性：**消息队列可以堆积请求，所以消费端业务即使短时间死掉，也不会影响主要业务的正常进行。

**异步通信：**很多时候，用户不想也不需要立即处理消息。消息队列提供了异步处理机制，允许用户把一个消息放入队列，但并不立即处理它。想向队列中放入多少消息就放多少，然后在需要的时候再去处理它们。



### Kafka中的ISR、AR又代表什么？ISR的伸缩又指什么

ISR:In-Sync Replicas 副本同步队列
AR:Assigned Replicas 所有副本
ISR是由leader维护，follower从leader同步数据有一些延迟（包括延迟时间replica.lag.time.max.ms和延迟条数replica.lag.max.messages两个维度, 当前最新的版本0.10.x中只支持replica.lag.time.max.ms这个维度），任意一个超过阈值都会把follower剔除出ISR, 存入OSR（Outof-Sync Replicas）列表，新加入的follower也会先存放在OSR中。AR=ISR+OSR。



### LEO、HW、LSO、LW等分别代表什么

- LEO：是 LogEndOffset 的简称，代表当前日志文件中下一条
- HW：水位或水印（watermark）一词，也可称为高水位(high watermark)，通常被用在流式处理领域（比如Apache Flink、Apache Spark等），以表征元素或事件在基于时间层面上的进度。在Kafka中，水位的概念反而与时间无关，而是与位置信息相关。严格来说，它表示的就是位置信息，即位移（offset）。取 partition 对应的 ISR中 最小的 LEO 作为 HW，consumer 最多只能消费到 HW 所在的位置上一条信息。
- LSO：是 LastStableOffset 的简称，对未完成的事务而言，LSO 的值等于事务中第一条消息的位置(firstUnstableOffset)，对已完成的事务而言，它的值同 HW 相同 
- LW：Low Watermark 低水位, 代表 AR 集合中最小的 logStartOffset 值。



### Kafka 消费者是否可以消费指定分区消息？

Kafa consumer消费消息时，向broker发出fetch请求去消费特定分区的消息，consumer指定消息在日志中的偏移量（offset），就可以消费从这个位置开始的消息，customer拥有了offset的控制权，可以向后回滚去重新消费之前的消息，这是很有意义的



### Kafka消息是采用Pull模式，还是Push模式？

Kafka最初考虑的问题是，customer应该从brokes拉取消息还是brokers将消息推送到consumer，也就是pull还push。在这方面，Kafka遵循了一种大部分消息系统共同的传统的设计：producer将消息推送到broker，consumer从broker拉取消息。

一些消息系统比如Scribe和Apache Flume采用了push模式，将消息推送到下游的consumer。这样做有好处也有坏处：由broker决定消息推送的速率，对于不同消费速率的consumer就不太好处理了。消息系统都致力于让consumer以最大的速率最快速的消费消息，但不幸的是，push模式下，当broker推送的速率远大于consumer消费的速率时，consumer恐怕就要崩溃了。最终Kafka还是选取了传统的pull模式。

Pull模式的另外一个好处是consumer可以自主决定是否批量的从broker拉取数据。Push模式必须在不知道下游consumer消费能力和消费策略的情况下决定是立即推送每条消息还是缓存之后批量推送。如果为了避免consumer崩溃而采用较低的推送速率，将可能导致一次只推送较少的消息而造成浪费。Pull模式下，consumer就可以根据自己的消费能力去决定这些策略。

Pull有个缺点是，如果broker没有可供消费的消息，将导致consumer不断在循环中轮询，直到新消息到t达。为了避免这点，Kafka有个参数可以让consumer阻塞知道新消息到达(当然也可以阻塞知道消息的数量达到某个特定的量这样就可以批量发



### Kafka 高效文件存储设计特点

- Kafka把topic中一个parition大文件分成多个小文件段，通过多个小文件段，就容易定期清除或删除已经消费完文件，减少磁盘占用。
- 通过索引信息可以快速定位message和确定response的最大大小。
- 通过index元数据全部映射到memory，可以避免segment file的IO磁盘操作。
- 通过索引文件稀疏存储，可以大幅降低index文件元数据占用空间大小



### kafka中的broker 是干什么的

broker 是消息的代理，Producers往Brokers里面的指定Topic中写消息，Consumers从Brokers里面拉取指定Topic的消息，然后进行业务处理，broker在中间起到一个代理保存消息的中转站。



### Kafka创建Topic时如何将分区放置到不同的Broker中

- 副本因子不能大于 Broker 的个数；
- 第一个分区（编号为0）的第一个副本放置位置是随机从 brokerList 选择的；
- 其他分区的第一个副本放置位置相对于第0个分区依次往后移。也就是如果我们有5个 Broker，5个分区，假设第一个分区放在第四个 Broker 上，那么第二个分区将会放在第五个 Broker 上；第三个分区将会放在第一个 Broker 上；第四个分区将会放在第二个 Broker 上，依次类推；
- 剩余的副本相对于第一个副本放置位置其实是由 nextReplicaShift 决定的，而这个数也是随机产生的



### topic的分区数可以增加或减少吗？为什么？

topic的分区数只能增加不能减少，因为减少掉的分区也就是被删除的分区的数据难以处理。

增加topic命令如下：

```
bin/kafka-topics.sh --zookeeper localhost:2181/kafka --alter \
--topic topic-config --partitions 3
```

关于topic还有一个面试点要知道：消费者组中的消费者个数如果超过topic的分区，那么就会有消费者消费不到数据。



### 你知道kafka是怎么维护offset的吗？

**1、维护offset的原因**：由于consumer在消费过程中可能会出现断电宕机等故障，consumer恢复后，需要从故障前的位置的继续消费，所以consumer需要实时记录自己消费到了哪个offset，以便故障恢复后继续消费。

**2、维护offset的方式** ：Kafka 0.9版本之前，consumer默认将offset保存在Zookeeper中，从0.9版本开始，consumer默认将offset保存在Kafka一个内置的topic中，该topic为__consumer_offsets。

**3、需要掌握的关于offset的常识** ：消费者提交消费位移时提交的是当前消费到的最新消息的offset+1而不是offset。



### 你们是怎么对Kafka进行压测的？

Kafka官方自带了压力测试脚本（kafka-consumer-perf-test.sh、kafka-producer-perf-test.sh）， Kafka 压测时，可以查看到哪个地方出现了瓶颈（CPU，内存，网络 IO），一般都是网络 IO 达到瓶颈。



### 当Kafka消息数据出现了积压，应该怎么处理？

数据积压主要可以从两个角度去分析：

**1、** 如果是 Kafka 消费能力不足，则可以考虑增加 Topic 的分区数，并且同时提升消费 组的消费者数量，消费者数=分区数。（两者缺一不可）

**2、** 如果是下游的数据处理不及时：提高每批次拉取的数量。如果是因为批次拉取数据过少（拉取 数据/处理时间<生产速度），也会使处理的数据小于生产的数据，造成数据积压。



### 聊聊Kafka分区分配策略？

在 Kafka 内部存在三种默认的分区分配策略：Range ， RoundRobin以及0.11.x版本引入的Sticky。Range 是默认策略。Range 是对每个 Topic 而言的（即一个 Topic 一个 Topic 分），首先 对同一个 Topic 里面的分区按照序号进行排序，并对消费者按照字母顺序进行排序。然后用 Partitions 分区的个数除以消费者线程的总数来决定每个消费者线程消费几个分区。如果除不尽，那么前面几个消费者线程将会多消费一个分区。

三种分区分配策略详见文章：深入分析Kafka架构（三）：消费者消费方式、分区分配策略（Range分配策略、RoundRobin分配策略、Sticky分配策略）、offset维护

文中对三种分区分配策略举例并进行了非常详细的对比，值得一看。



### 谈谈你对Kafka幂等性的理解？

Producer的幂等性指的是当发送同一条消息时，数据在 Server 端只会被持久化一次，数据不丟不重，但是这里的幂等性是有条件的：

**1、** 只能保证 Producer 在单个会话内不丟不重，如果 Producer 出现意外挂掉再重启是 无法保证的。**因为幂等性情况下，是无法获取之前的状态信息，因此是无法做到跨会话级别的不丢不重**。

**2、** 幂等性不能跨多个 Topic-Partition，只能保证单个 Partition 内的幂等性，当涉及多个Topic-Partition 时，这中间的状态并没有同步。



### 你对Kafka事务了解多少？

Kafka是在0.11 版本开始引入了事务支持。事务可以保证 Kafka 在 Exactly Once 语义的基 础上，生产和消费可以跨分区和会话，要么全部成功，要么全部失败。

**1、Producer 事务：**

为了实现跨分区跨会话的事务，需要引入一个全局唯一的 Transaction ID，并将 Producer 获得的 PID 和 Transaction ID 绑定。这样当 Producer 重启后就可以通过正在进行的 Transaction ID 获得原来的 PID。

为了管理 Transaction，Kafka 引入了一个新的组件 Transaction Coordinator。Producer 就 是通过和 Transaction Coordinator 交互获得 Transaction ID 对应的任务状态。Transaction Coordinator 还负责将事务所有写入 Kafka 的一个内部 Topic，这样即使整个服务重启，由于 事务状态得到保存，进行中的事务状态可以得到恢复，从而继续进行。

**2、Consumer 事务：**

上述事务机制主要是从Producer方面考虑，对于 Consumer 而言，事务的保证就会相对较弱，尤其时无法保证 Commit 的信息被精确消费。这是由于 Consumer 可以通过offset访问任意信息，而且不同的 Segment File生命周期不同，同一事务的消息可能会出现重启后被删除的情况。



### Kafka怎么实现如此高的读写效率？

**1、** 首先kafka本身是分布式集群，同时采用了分区技术，具有较高的并发度；

**2、** 顺序写入磁盘，Kafka 的 producer 生产数据，要写入到 log 文件中，写的过程是一直追加到文件末端，为顺序写。

官网有数据表明，同样的磁盘，顺序写能到 600M/s，而随机写只有 100K/s。这 与磁盘的机械机构有关，顺序写之所以快，是因为其省去了大量磁头寻址的时间。

**3、** 零拷贝技术



### Kafka新建的分区会在哪个目录下创建

在启动 Kafka 集群之前，我们需要配置好 log.dirs 参数，其值是 Kafka 数据的存放目录，这个参数可以配置多个目录，目录之间使用逗号分隔，通常这些目录是分布在不同的磁盘上用于提高读写性能。

当然我们也可以配置 log.dir 参数，含义一样。只需要设置其中一个即可。

如果 log.dirs 参数只配置了一个目录，那么分配到各个 Broker 上的分区肯定只能在这个目录下创建文件夹用于存放数据。

但是如果 log.dirs 参数配置了多个目录，那么 Kafka 会在哪个文件夹中创建分区目录呢？答案是：Kafka 会在含有分区目录最少的文件夹中创建新的分区目录，分区目录名为 Topic名+分区ID。注意，是分区文件夹总数最少的目录，而不是磁盘使用量最少的目录！也就是说，如果你给 log.dirs 参数新增了一个新的磁盘，新的分区目录肯定是先在这个新的磁盘上创建直到这个新的磁盘目录拥有的分区目录不是最少为止。



### **什么是消费者组？**

消费者组是Kafka独有的概念，如果面试官问这个，就说明他对此是有一定了解的。

**官网上的介绍言简意赅，即消费者组是Kafka提供的可扩展且具有容错性的消费者机制。**

但实际上，消费者组（Consumer Group）其实包含两个概念，作为队列，消费者组允许你分割数据处理到一组进程集合上（即一个消费者组中可以包含多个消费者进程，他们共同消费该topic的数据），这有助于你的消费能力的动态调整；作为发布-订阅模型（publish-subscribe），Kafka允许你将同一份消息广播到多个消费者组里，以此来丰富多种数据使用场景。

需要注意的是：在消费者组中，多个实例共同订阅若干个主题，实现共同消费。同一个组下的每个实例都配置有相同的组ID，被分配不同的订阅分区。当某个实例挂掉的时候，其他实例会自动地承担起它负责消费的分区。因此，消费者组在一定程度上也保证了消费者程序的高可用性。



![图片](https://mmbiz.qpic.cn/mmbiz_jpg/A1HKVXsfHNmVGNayOCy5c88kf89bF3fSeXoNcB6t6QFpKyWel0DbwZwnhwxTCiaYOHlKbmqLbWd7et5YgKRIGfw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



注意：消费者组的题目，能够帮你在某种程度上掌控下面的面试方向。

- 如果你擅长位移值原理（Offset），就不妨再提一下消费者组的位移提交机制；
- 如果你擅长Kafka Broker，可以提一下消费者组与Broker之间的交互；
- 如果你擅长与消费者组完全不相关的Producer，那么就可以这么说：“消费者组要消费的数据完全来自于Producer端生产的消息，我对Producer还是比较熟悉的。”



总之，你总得对consumer group相关的方向有一定理解，然后才能像面试官表名你对某一块很理解。



### **kafka中的 zookeeper 起到什么作用，可以不用zookeeper么**

zookeeper 是一个分布式的协调组件，早期版本的kafka用zk做meta信息存储，consumer的消费状态，group的管理以及 offset的值。考虑到zk本身的一些因素以及整个架构较大概率存在单点问题，新版本中逐渐弱化了zookeeper的作用。新的consumer使用了kafka内部的group coordination协议，也减少了对zookeeper的依赖，

但是broker依然依赖于ZK，zookeeper 在kafka中还用来选举controller 和 检测broker是否存活等等。




### Kafka 为什么那么快

Cache Filesystem Cache PageCache缓存

顺序写 由于现代的操作系统提供了预读和写技术，磁盘的顺序写大多数情况下比随机写内存还要快。

Zero-copy 零拷技术减少拷贝次数

Batching of Messages 批量量处理。合并小的请求，然后以流的方式进行交互，直顶网络上限。

Pull 拉模式 使用拉模式进行消息的获取消费，与消费端处理能力相符。



### 谈一谈 Kafka 的再均衡

在Kafka中，当有新消费者加入或者订阅的topic数发生变化时，会触发Rebalance(再均衡：在同一个消费者组当中，分区的所有权从一个消费者转移到另外一个消费者)机制，Rebalance顾名思义就是重新均衡消费者消费。Rebalance的过程如下：

**第一步：** 所有成员都向coordinator发送请求，请求入组。一旦所有成员都发送了请求，coordinator会从中选择一个consumer担任leader的角色，并把组成员信息以及订阅信息发给leader。

**第二步：** leader开始分配消费方案，指明具体哪个consumer负责消费哪些topic的哪些partition。一旦完成分配，leader会将这个方案发给coordinator。coordinator接收到分配方案之后会把方案发给各个consumer，这样组内的所有成员就都知道自己应该消费哪些分区了。

所以对于Rebalance来说，Coordinator起着至关重要的作用



###  Kafka 是如何实现高吞吐率的？

Kafka是分布式消息系统，需要处理海量的消息，Kafka的设计是把所有的消息都写入速度低容量大的硬盘，以此来换取更强的存储能力，但实际上，使用硬盘并没有带来过多的性能损失。kafka主要使用了以下几个方式实现了超高的吞吐率：

- 顺序读写；
- 零拷贝
- 文件分段
- 批量发送
- 数据压缩。




### **如何设置Kafka能接收的最大消息的大小？**

对于SRE来讲，该题简直是送分题啊，但是，最大消息的设置通常情况下有生产者端，消费者端，broker端和topic级别的参数，我们需要正确设置，以保证可以正常的生产和消费。

- Broker端参数：message.max.bytes，max.message.bytes（topic级别），replica.fetch.max.bytes（否则follow会同步失败）
- Consumer端参数：fetch.message.max.bytes



###  **监控Kafka的框架都有哪些？**

对于SRE来讲，依然是送分题。但基础的我们要知道，Kafka本身是提供了JMX（Java Management Extensions）的，我们可以通过它来获取到Kafka内部的一些基本数据。

- **Kafka Manager：**更多是Kafka的管理，对于SRE非常友好，也提供了简单的瞬时指标监控。
- **Kafka Monitor：**LinkedIn开源的免费框架，支持对集群进行系统测试，并实时监控测试结果。
- **CruiseControl：**也是LinkedIn公司开源的监控框架，用于实时监测资源使用率，以及提供常用运维操作等。无UI界面，只提供REST API，可以进行多集群管理。
- **JMX监控：**由于Kafka提供的监控指标都是基于JMX的，因此，市面上任何能够集成JMX的框架都可以使用，比如Zabbix和Prometheus。
- 已有大数据平台自己的监控体系：像Cloudera提供的CDH这类大数据平台，天然就提供Kafka监控方案。
- **JMXTool：**社区提供的命令行工具，能够实时监控JMX指标。可以使用kafka-run-class.sh kafka.tools.JmxTool来查看具体的用法。



### **如何估算Kafka集群的机器数量？**

该题也算是SRE的送分题吧，对于SRE来讲，任何生产的系统第一步需要做的就是容量预估以及集群的架构规划，实际上也就是机器数量和所用资源之间的关联关系，资源通常来讲就是CPU，内存，磁盘容量，带宽。但需要注意的是，Kafka因为独有的设计，对于磁盘的要求并不是特别高，普通机械硬盘足够，而通常的瓶颈会出现在带宽上。

在预估磁盘的占用时，你一定不要忘记计算副本同步的开销。如果一条消息占用1KB的磁盘空间，那么，在有3个副本的主题中，你就需要3KB的总空间来保存这条消息。同时，需要考虑到整个业务Topic数据保存的最大时间，以上几个因素，基本可以预估出来磁盘的容量需求。

需要注意的是：对于磁盘来讲，一定要提前和业务沟通好场景，而不是等待真正有磁盘容量瓶颈了才去扩容磁盘或者找业务方沟通方案。

对于带宽来说，常见的带宽有1Gbps和10Gbps，通常我们需要知道，当带宽占用接近总带宽的90%时，丢包情形就会发生。



### **Kafka能手动删除消息吗？**

Kafka不需要用户手动删除消息。它本身提供了留存策略，能够自动删除过期消息。当然，它是支持手动删除消息的。



- 对于设置了Key且参数cleanup.policy=compact的主题而言，我们可以构造一条 的消息发送给Broker，依靠Log Cleaner组件提供的功能删除掉该 Key 的消息。
- 对于普通主题而言，我们可以使用kafka-delete-records命令，或编写程序调用Admin.deleteRecords方法来删除消息。这两种方法殊途同归，底层都是调用Admin的deleteRecords方法，通过将分区Log Start Offset值抬高的方式间接删除消息。



### **__consumer_offsets是做什么用的？**

这是一个内部主题，主要用于存储消费者的偏移量，以及消费者的元数据信息（消费者实例，消费者id等等）

需要注意的是：Kafka的GroupCoordinator组件提供对该主题完整的管理功能，包括该主题的创建、写入、读取和Leader维护等。



### Kafka Stream的一些独特功能是什么？

Kafka Stream是理想的实时数据流工具。以下是确立Kafka Stream受欢迎程度的独特功能。

- 高可扩展性和容错能力。
- 轻松部署到云，容器，裸机或虚拟机。
- 通过与Kafka安全性的集成。
- 编写标准Java应用程序的工具。
- 一次性处理语义。
- 适用于小型，中型和大型用例。
- 无需单独的处理集群。



### 为什么说Kafka是分布式流媒体平台？

首先，它可以帮助轻松地推动记录。此外，Apache Kafka还可以帮助你存储大量记录而不会遇到存储问题。最重要的是，Kafka能够处理到达的记录。这些功能显然将Kafka确立为可靠的分布式流媒体平台。