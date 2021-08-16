**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [简要介绍一下Elasticsearch？](#简要介绍一下elasticsearch)
- [什么是Elasticsearch？](#什么是elasticsearch)
- [安装 Elasticsearch 需要依赖什么组件吗？](#安装-elasticsearch-需要依赖什么组件吗)
- [如何启动 Elasticsearch 服务器？](#如何启动-elasticsearch-服务器)
- [ElasticSearch中的集群、节点、索引、文档、类型是什么？](#elasticsearch中的集群节点索引文档类型是什么)
- [Elasticsearch 支持哪些类型的查询？](#elasticsearch-支持哪些类型的查询)
- [精准匹配检索和全文检索匹配检索的不同？](#精准匹配检索和全文检索匹配检索的不同)
- [ElasticSearch中的分片是什么?](#elasticsearch中的分片是什么)
- [elasticsearch了解多少，说说你们公司es的集群架构，索引数据大小，分片有多少，以及一些调优手段 。](#elasticsearch了解多少说说你们公司es的集群架构索引数据大小分片有多少以及一些调优手段-)
  - [1.1 、设计阶段调优](#11-设计阶段调优)
  - [1.2 、写入调优](#12-写入调优)
  - [1.3 、查询调优](#13-查询调优)
  - [1.4 、其他调优](#14-其他调优)
- [elasticsearch 索引数据多了怎么办，如何调优，部署](#elasticsearch-索引数据多了怎么办如何调优部署)
- [请解释一下 Elasticsearch 中聚合？](#请解释一下-elasticsearch-中聚合)
- [解释一下Elasticsearch Cluster？](#解释一下elasticsearch-cluster)
- [解释一下 Elasticsearch Node？](#解释一下-elasticsearch-node)
- [我们可以在 Elasticsearch 中执行搜索的各种可能方式有哪些？](#我们可以在-elasticsearch-中执行搜索的各种可能方式有哪些)
- [解释一下 Elasticsearch 集群中的 Type 的概念 ？](#解释一下-elasticsearch-集群中的-type-的概念-)
- [解释一下 Elasticsearch 的 分片？](#解释一下-elasticsearch-的-分片)
- [定义副本、创建副本的好处是什么？](#定义副本创建副本的好处是什么)
- [Elasticsearch Analyzer 中的字符过滤器如何利用？](#elasticsearch-analyzer-中的字符过滤器如何利用)
- [REST API在 Elasticsearch 方面有哪些优势？](#rest-api在-elasticsearch-方面有哪些优势)
- [Elasticsearch 中常用的 cat命令有哪些？](#elasticsearch-中常用的-cat命令有哪些)
- [你能否列出与 Elasticsearch 有关的主要可用字段数据类型？](#你能否列出与-elasticsearch-有关的主要可用字段数据类型)
- [Elasticsearch了解多少，说说你们公司es的集群架构，索引数据大小，分片有多少，以及一些调优手段 。](#elasticsearch了解多少说说你们公司es的集群架构索引数据大小分片有多少以及一些调优手段-)
- [解释一下 Elasticsearch集群中的 索引的概念 ？](#解释一下-elasticsearch集群中的-索引的概念-)
- [Elasticsearch 索引数据多了怎么办，如何调优，部署](#elasticsearch-索引数据多了怎么办如何调优部署)
- [我们可以在 Elasticsearch 中执行搜索的各种可能方式有哪些？](#我们可以在-elasticsearch-中执行搜索的各种可能方式有哪些)
- [在 Elasticsearch 中删除索引的语法是什么？](#在-elasticsearch-中删除索引的语法是什么)
- [在 Elasticsearch 中列出集群的所有索引的语法是什么？](#在-elasticsearch-中列出集群的所有索引的语法是什么)
- [在索引中更新 Mapping 的语法？](#在索引中更新-mapping-的语法)
- [ES 写数据过程](#es-写数据过程)
- [ES 读数据过程](#es-读数据过程)
- [底层 lucene](#底层-lucene)
- [ES中的倒排索引是什么？](#es中的倒排索引是什么)
- [请解释在 Elasticsearch 集群中添加或创建索引的过程？](#请解释在-elasticsearch-集群中添加或创建索引的过程)
- [详细描述一下Elasticsearch索引文档的过程](#详细描述一下elasticsearch索引文档的过程)
- [详细描述一下Elasticsearch更新和删除文档的过程](#详细描述一下elasticsearch更新和删除文档的过程)
- [详细描述一下Elasticsearch搜索的过程](#详细描述一下elasticsearch搜索的过程)
- [Elasticsearch对于大数据量（上亿量级）的聚合如何实现？](#elasticsearch对于大数据量上亿量级的聚合如何实现)
- [你可以列出 Elasticsearch 各种类型的分析器吗？](#你可以列出-elasticsearch-各种类型的分析器吗)
- [ElaticSearch是如何实现master选举的？](#elaticsearch是如何实现master选举的)
- [Master 节点和 候选 Master节点有什么区别？](#master-节点和-候选-master节点有什么区别)
- [Elasticsearch中的属性 enabled, index 和 store 的功能是什么？](#elasticsearch中的属性-enabled-index-和-store-的功能是什么)
- [Elasticsearch中的节点（比如共20个），其中的10个选了一个master，另外10个选了另一个master，怎么办？](#elasticsearch中的节点比如共20个其中的10个选了一个master另外10个选了另一个master怎么办)
- [如何解决ES集群的脑裂问题](#如何解决es集群的脑裂问题)
- [详细描述一下ES索引文档的过程？](#详细描述一下es索引文档的过程)
- [详细描述一下ES更新和删除文档的过程？](#详细描述一下es更新和删除文档的过程)
- [详细描述一下ES搜索的过程？](#详细描述一下es搜索的过程)
- [在并发情况下，ES如果保证读写一致？](#在并发情况下es如果保证读写一致)
- [ES对于大数据量（上亿量级）的聚合如何实现？](#es对于大数据量上亿量级的聚合如何实现)
- [对于GC方面，在使用ES时要注意什么？](#对于gc方面在使用es时要注意什么)
- [说说你们公司ES的集群架构，索引数据大小，分片有多少，以及一些调优手段？](#说说你们公司es的集群架构索引数据大小分片有多少以及一些调优手段)
- [在并发情况下，Elasticsearch如果保证读写一致？](#在并发情况下elasticsearch如果保证读写一致)

<!-- /TOC -->

### 简要介绍一下Elasticsearch？

Elasticsearch 是一个分布式、RESTful 风格的搜索和数据分析引擎，能够解决不断涌现出的各种用例。作为 Elastic Stack 的核心，它集中存储您的数据，帮助您发现意料之中以及意料之外的情况。

ElasticSearch 是基于Lucene的搜索服务器。它提供了一个分布式多用户能力的全文搜索引擎，基于RESTful web接口。Elasticsearch是用Java开发的，并作为Apache许可条款下的开放源码发布，是当前流行的企业级搜索引擎。

核心特点如下：

- 分布式的实时文件存储，每个字段都被索引且可用于搜索。
- 分布式的实时分析搜索引擎，海量数据下近实时秒级响应。
- 简单的restful api，天生的兼容多语言开发。
- 易扩展，处理PB级结构化或非结构化数据。



### 什么是Elasticsearch？

Elasticsearch 是一个基于 Lucene 的搜索引擎。它提供了具有 HTTP Web 界面和无架构 JSON 文档的分布式，多租户能力的全文搜索引擎。
Elasticsearch 是用 Java 开发的，根据 Apache 许可条款作为开源发布。



### 安装 Elasticsearch 需要依赖什么组件吗？

ES 早期版本需要JDK，在7.X版本后已经集成了 JDK，已无需第三方依赖。



### 如何启动 Elasticsearch 服务器？

启动方式有很多种，一般 bin 路径下

```
./elasticsearch -d 
```

就可以后台启动。

打开浏览器输入 http://ES IP:9200 就能知道集群是否启动成功。

如果启动报错，日志里会有详细信息，逐条核对解决就可以。



### ElasticSearch中的集群、节点、索引、文档、类型是什么？

**群集**是一个或多个节点（服务器）的集合，它们共同保存您的整个数据，并提供跨所有节点的联合索引和搜索功能。群集由唯一名称标识，默认情况下为“elasticsearch”。此名称很重要，因为如果节点设置为按名称加入群集，则该节点只能是群集的一部分。



**节点**是属于集群一部分的单个服务器。它存储数据并参与群集索引和搜索功能。

**索引**就像关系数据库中的“数据库”。它有一个定义多种类型的映射。索引是逻辑名称空间，映射到一个或多个主分片，并且可以有零个或多个副本分片。 MySQL =>数据库 　　 ElasticSearch =>索引

**文档**类似于关系数据库中的一行。不同之处在于索引中的每个文档可以具有不同的结构（字段），但是对于通用字段应该具有相同的数据类型。 MySQL => Databases => 　 Tables => Columns / Rows ElasticSearch => Indices => Types =>具有属性的文档

**类型**是索引的逻辑类别/分区，其语义完全取决于用户。



### Elasticsearch 支持哪些类型的查询？

查询主要分为两种类型：精确匹配、全文检索匹配。

- 精确匹配，例如 term、exists、term set、 range、prefix、 ids、 wildcard、regexp、 fuzzy等。
- 全文检索，例如match、match_phrase、multi_match、match_phrase_prefix、query_string 等



### 精准匹配检索和全文检索匹配检索的不同？

两者的本质区别：

- 精确匹配用于：是否完全一致？

举例：邮编、身份证号的匹配往往是精准匹配。

- 全文检索用于：是否相关？

举例：类似B站搜索特定关键词如“马保国 视频”往往是模糊匹配，相关的都返回就可以。



### ElasticSearch中的分片是什么?

在大多数环境中，每个节点都在单独的盒子或虚拟机上运行。

索引 - 在Elasticsearch中，索引是文档的集合。
分片 -因为Elasticsearch是一个分布式搜索引擎，所以索引通常被分割成分布在多个节点上的被称为分片的元素。



### elasticsearch了解多少，说说你们公司es的集群架构，索引数据大小，分片有多少，以及一些调优手段 。

`面试官`：想了解应聘者之前公司接触的ES使用场景、规模，有没有做过比较大规模的索引设计、规划、调优。
`解答`：
如实结合自己的实践场景回答即可。
比如：ES集群架构13个节点，索引根据通道不同共20+索引，根据日期，每日递增20+，索引：10分片，每日递增1亿+数据，
每个通道每天索引大小控制：150GB之内。

仅索引层面调优手段：

##### 1.1、设计阶段调优

- 1）根据业务增量需求，采取基于日期模板创建索引，通过roll over API滚动索引；
- 2）使用别名进行索引管理；
- 3）每天凌晨定时对索引做force_merge操作，以释放空间；
- 4）采取冷热分离机制，热数据存储到SSD，提高检索效率；冷数据定期进行shrink操作，以缩减存储；
- 5）采取curator进行索引的生命周期管理；
- 6）仅针对需要分词的字段，合理的设置分词器；
- 7）Mapping阶段充分结合各个字段的属性，是否需要检索、是否需要存储等。 ……..

##### 1.2、写入调优

- 1）写入前副本数设置为0；
- 2）写入前关闭refresh_interval设置为-1，禁用刷新机制；
- 3）写入过程中：采取bulk批量写入；
- 4）写入后恢复副本数和刷新间隔；
- 5）尽量使用自动生成的id。

##### 1.3、查询调优

- 1）禁用wildcard；
- 2）禁用批量terms（成百上千的场景）；
- 3）充分利用倒排索引机制，能keyword类型尽量keyword；
- 4）数据量大时候，可以先基于时间敲定索引再检索；
- 5）设置合理的路由机制。

##### 1.4、其他调优

部署调优，业务调优等。

上面的提及一部分，面试者就基本对你之前的实践或者运维经验有所评估了。



### elasticsearch 索引数据多了怎么办，如何调优，部署

`面试官`：想了解大数据量的运维能力。
`解答`：索引数据的规划，应在前期做好规划，正所谓“设计先行，编码在后”，这样才能有效的避免突如其来的数据激增导致集群处理能力不足引发的线上客户检索或者其他业务受到影响。
如何调优，正如问题1所说，这里细化一下：

**动态索引层面**

基于`模板+时间+rollover api滚动`创建索引，举例：设计阶段定义：blog索引的模板格式为：blog_index_时间戳的形式，每天递增数据。

这样做的好处：不至于数据量激增导致单个索引数据量非常大，接近于上线2的32次幂-1，索引存储达到了TB+甚至更大。

一旦单个索引很大，存储等各种风险也随之而来，所以要提前考虑+及早避免。

 **存储层面**

`冷热数据分离存储`，热数据（比如最近3天或者一周的数据），其余为冷数据。
对于冷数据不会再写入新数据，可以考虑定期force_merge加shrink压缩操作，节省存储空间和检索效率。

**部署层面**

一旦之前没有规划，这里就属于应急策略。
结合ES自身的支持动态扩展的特点，动态新增机器的方式可以缓解集群压力，注意：如果之前主节点等`规划合理`，不需要重启集群也能完成动态新增的。



### 请解释一下 Elasticsearch 中聚合？

聚合有助于从搜索中使用的查询中收集数据，聚合为各种统计指标，便于统计信息或做其他分析。聚合可帮助回答以下问题：

- 我的网站平均加载时间是多少？
- 根据交易量，谁是我最有价值的客户？
- 什么会被视为我网络上的大文件？
- 每个产品类别中有多少个产品？

聚合的分三类：

主要查看7.10 的官方文档，早期是4个分类，别大意啊！

- 分桶 Bucket 聚合

根据字段值，范围或其他条件将文档分组为桶（也称为箱）。

- 指标 Metric 聚合

从字段值计算指标（例如总和或平均值）的指标聚合。

- 管道 Pipeline 聚合

子聚合，从其他聚合（而不是文档或字段）获取输入。



### 解释一下Elasticsearch Cluster？

Elasticsearch 集群是一组连接在一起的一个或多个 Elasticsearch 节点实例。

Elasticsearch 集群的功能在于在集群中的所有节点之间分配任务，进行搜索和建立索引。



### 解释一下 Elasticsearch Node？

节点是 Elasticsearch 的实例。实际业务中，我们会说：ES集群包含3个节点、7个节点。

这里节点实际就是：一个独立的 Elasticsearch 进程，一般将一个节点部署到一台独立的服务器或者虚拟机、容器中。

不同节点根据角色不同，可以划分为：

- 主节点

帮助配置和管理在整个集群中添加和删除节点。

- 数据节点

存储数据并执行诸如CRUD（创建/读取/更新/删除）操作，对数据进行搜索和聚合的操作。

- 客户端节点（或者说：协调节点） 将集群请求转发到主节点，将与数据相关的请求转发到数据节点
- 摄取节点

用于在索引之前对文档进行预处理。



### 我们可以在 Elasticsearch 中执行搜索的各种可能方式有哪些？

核心方式如下：

方式一：基于 DSL 检索（最常用） Elasticsearch提供基于JSON的完整查询DSL来定义查询。

```
GET /shirts/_search
{
  "query": {
    "bool": {
      "filter": [
        { "term": { "color": "red"   }},
        { "term": { "brand": "gucci" }}
      ]
    }
  }
}
```

方式二：基于 URL 检索

```
GET /my_index/_search?q=user:seina
```

方式三：类SQL 检索

```
POST /_sql?format=txt
{
  "query": "SELECT * FROM uint-2020-08-17 ORDER BY itemid DESC LIMIT 5"
}
```

功能还不完备，不推荐使用。



### 解释一下 Elasticsearch 集群中的 Type 的概念 ？

5.X 以及之前的 2.X、1.X 版本 ES支持一个索引多个type的，举例 ES 6.X 中的Join 类型在早期版本实际是多 Type 实现的。

在6.0.0 或 更高版本中创建的索引只能包含一个 Mapping 类型。

Type 将在Elasticsearch 7.0.0中的API中弃用，并在8.0.0中完全删除。



### 解释一下 Elasticsearch 的 分片？

当文档数量增加，硬盘容量和处理能力不足时，对客户端请求的响应将延迟。

在这种情况下，将索引数据分成小块的过程称为分片，可改善数据搜索结果的获取。



### 定义副本、创建副本的好处是什么？

副本是 分片的对应副本，用在极端负载条件下提高查询吞吐量或实现高可用性。

所谓高可用主要指：如果某主分片1出了问题，对应的副本分片1会提升为主分片，保证集群的高可用。



### Elasticsearch Analyzer 中的字符过滤器如何利用？

字符过滤器将原始文本作为字符流接收，并可以通过添加，删除或更改字符来转换字符流。

字符过滤分类如下：

- HTML Strip Character Filter.

用途：删除HTML元素，如<b>，并解码HTML实体，如＆amp 。

- Mapping Character Filter

用途：替换指定的字符。

- Pattern Replace Character Filter

用途：基于正则表达式替换指定的字符。



### REST API在 Elasticsearch 方面有哪些优势？

REST API是使用超文本传输协议的系统之间的通信，该协议以 XML 和 JSON格式传输数据请求。

REST 协议是无状态的，并且与带有服务器和存储数据的用户界面分开，从而增强了用户界面与任何类型平台的可移植性。它还提高了可伸缩性，允许独立实现组件，因此应用程序变得更加灵活。

REST API与平台和语言无关，只是用于数据交换的语言是XML或JSON。

借助：REST API 查看集群信息或者排查问题都非常方便。



### Elasticsearch 中常用的 cat命令有哪些？

面试时说几个核心的就可以，包含但不限于：

| 含义       | 命令                     |
| :--------- | :----------------------- |
| 别名       | GET _cat/aliases?v       |
| 分配相关   | GET _cat/allocation      |
| 计数       | GET _cat/count?v         |
| 字段数据   | GET _cat/fielddata?v     |
| 运行状况   | GET_cat/health?          |
| 索引相关   | GET _cat/indices?v       |
| 主节点相关 | GET _cat/master?v        |
| 节点属性   | GET _cat/nodeattrs?v     |
| 节点       | GET _cat/nodes?v         |
| 待处理任务 | GET _cat/pending_tasks?v |
| 插件       | GET _cat/plugins?v       |
| 恢复       | GET _cat / recovery?v    |
| 存储库     | GET _cat /repositories?v |
| 段         | GET _cat /segments?v     |
| 分片       | GET _cat/shards?v        |
| 快照       | GET _cat/snapshots?v     |
| 任务       | GET _cat/tasks?v         |
| 模板       | GET _cat/templates?v     |
| 线程池     | GET _cat/thread_pool?v   |



### 你能否列出与 Elasticsearch 有关的主要可用字段数据类型？

- 字符串数据类型，包括支持全文检索的 text 类型 和 精准匹配的 keyword 类型。
- 数值数据类型，例如字节，短整数，长整数，浮点数，双精度数，half_float，scaled_float。
- 日期类型，日期纳秒Date nanoseconds，布尔值，二进制（Base64编码的字符串）等。
- 范围（整数范围 integer_range，长范围 long_range，双精度范围 double_range，浮动范围 float_range，日期范围 date_range）。
- 包含对象的复杂数据类型，nested 、Object。
- GEO 地理位置相关类型。
- 特定类型如：数组（数组中的值应具有相同的数据类型）



### Elasticsearch了解多少，说说你们公司es的集群架构，索引数据大小，分片有多少，以及一些调优手段 。

如实结合自己的实践场景回答即可。
比如：ES集群架构13个节点，索引根据通道不同共20+索引，根据日期，每日递增20+，索引：10分片，每日递增1亿+数据，
每个通道每天索引大小控制：150GB之内。



**设计阶段调优**

1、根据业务增量需求，采取基于日期模板创建索引，通过roll over API滚动索引；

2、使用别名进行索引管理；

3、每天凌晨定时对索引做force_merge操作，以释放空间；

4、采取冷热分离机制，热数据存储到SSD，提高检索效率；冷数据定期进行shrink操作，以缩减存储；

5、采取curator进行索引的生命周期管理；

6、仅针对需要分词的字段，合理的设置分词器；

7、Mapping阶段充分结合各个字段的属性，是否需要检索、是否需要存储等。……..



**写入调优**

1、写入前副本数设置为0；

2、写入前关闭refresh_interval设置为-1，禁用刷新机制；

3、写入过程中：采取bulk批量写入；

4、写入后恢复副本数和刷新间隔；

5、尽量使用自动生成的id。



**查询调优**

1、禁用wildcard；

2、禁用批量terms（成百上千的场景）；

3、充分利用倒排索引机制，能keyword类型尽量keyword；

4、数据量大时候，可以先基于时间敲定索引再检索；

5、设置合理的路由机制。



**其他调优**

部署调优，业务调优等。

上面的提及一部分，面试者就基本对你之前的实践或者运维经验有所评估了。



### 解释一下 Elasticsearch集群中的 索引的概念 ？

Elasticsearch 集群可以包含多个索引，与关系数据库相比，它们相当于数据库表

其他类别概念，如下表所示，点到为止。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210401092050.png)

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210401092103.png)





### Elasticsearch 索引数据多了怎么办，如何调优，部署

索引数据的规划，应在前期做好规划，正所谓“设计先行，编码在后”，这样才能有效的避免突如其来的数据激增导致集群处理能力不足引发的线上客户检索或者其他业务受到影响。
如何调优，正如问题1所说，这里细化一下：

**动态索引层面**

基于`模板+时间+rollover api滚动`创建索引，举例：设计阶段定义：blog索引的模板格式为：blog_index_时间戳的形式，每天递增数据。

这样做的好处：不至于数据量激增导致单个索引数据量非常大，接近于上线2的32次幂-1，索引存储达到了TB+甚至更大。

一旦单个索引很大，存储等各种风险也随之而来，所以要提前考虑+及早避免。



**存储层面**

`冷热数据分离存储`，热数据（比如最近3天或者一周的数据），其余为冷数据。
对于冷数据不会再写入新数据，可以考虑定期force_merge加shrink压缩操作，节省存储空间和检索效率。



**部署层面**

一旦之前没有规划，这里就属于应急策略。
结合ES自身的支持动态扩展的特点，动态新增机器的方式可以缓解集群压力，注意：如果之前主节点等`规划合理`，不需要重启集群也能完成动态新增的。



### 我们可以在 Elasticsearch 中执行搜索的各种可能方式有哪些？

**方式一：**

基于 DSL 检索（最常用） Elasticsearch提供基于JSON的完整查询DSL来定义查询。

```
GET /shirts/_search
{
  "query": {
    "bool": {
      "filter": [
        { "term": { "color": "red"   }},
        { "term": { "brand": "gucci" }}
      ]
    }
  }
}
```



**方式二：**

基于 URL 检索

```
GET /my_index/_search?q=user:seina
```



**方式三：**

类SQL 检索

```
POST /_sql?format=txt
{
  "query": "SELECT * FROM uint-2020-08-17 ORDER BY itemid DESC LIMIT 5"
}
```

功能还不完备，不推荐使用。



### 在 Elasticsearch 中删除索引的语法是什么？

可以使用以下语法删除现有索引：

```
DELETE <index_name>
```

支持通配符删除：

```
DELETE my_*
```



### 在 Elasticsearch 中列出集群的所有索引的语法是什么？

```
GET _cat/indices
```



### 在索引中更新 Mapping 的语法？

```
PUT test_001/_mapping
{
  "properties": {
    "title":{
      "type":"keyword"
    }
  }
}
```





### ES 写数据过程

- 客户端选择一个 node 发送请求过去，这个 node 就是 `coordinating node`（协调节点）。
- `coordinating node` 对 document 进行路由，将请求转发给对应的 node（有 primary shard）。[路由的算法是？]
- 实际的 node 上的 `primary shard` 处理请求，然后将数据同步到 `replica node`。
- `coordinating node` 如果发现 `primary node` 和所有 `replica node` 都搞定之后，就返回响应结果给客户端。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210401090646.png)



### ES 读数据过程

可以通过 `doc id` 来查询，会根据 `doc id` 进行 hash，判断出来当时把 `doc id` 分配到了哪个 shard 上面去，从那个 shard 去查询。

- 客户端发送请求到任意一个 node，成为 `coordinate node`。
- `coordinate node` 对 `doc id` 进行哈希路由，将请求转发到对应的 node，此时会使用 `round-robin`随机轮询算法，在 `primary shard` 以及其所有 replica 中随机选择一个，让读请求负载均衡。
- 接收请求的 node 返回 document 给 `coordinate node`。
- `coordinate node` 返回 document 给客户端。

***写请求是写入 primary shard，然后同步给所有的 replica shard；读请求可以从 primary shard 或 replica shard 读取，采用的是随机轮询算法。***



### 底层 lucene

简单来说，lucene 就是一个 jar 包，里面包含了封装好的各种建立倒排索引的算法代码。我们用 Java 开发的时候，引入 lucene jar，然后基于 lucene 的 api 去开发就可以了。

通过 lucene，我们可以将已有的数据建立索引，lucene 会在本地磁盘上面，给我们组织索引的数据结构。



### ES中的倒排索引是什么？

传统的检索方式是通过文章，逐个遍历找到对应关键词的位置。
倒排索引，是通过分词策略，形成了词和文章的映射关系表，也称倒排表，这种词典 + 映射表即为**倒排索引**。

其中词典中存储词元，倒排表中存储该词元在哪些文中出现的位置。
有了倒排索引，就能实现 O(1) 时间复杂度的效率检索文章了，极大的提高了检索效率。

**加分项：**
倒排索引的底层实现是基于：FST（Finite State Transducer）数据结构。

Lucene 从 4+ 版本后开始大量使用的数据结构是 FST。FST 有两个优点：
**1、**空间占用小。通过对词典中单词前缀和后缀的重复利用，压缩了存储空间；
**2、**查询速度快。O(len(str)) 的查询时间复杂度。



### 请解释在 Elasticsearch 集群中添加或创建索引的过程？

要添加新索引，应使用创建索引 API 选项。创建索引所需的参数是索引的配置Settings，索引中的字段 Mapping 以及索引别名 Alias。

也可以通过模板 Template 创建索引。



### 详细描述一下Elasticsearch索引文档的过程

协调节点默认使用文档ID参与计算（也支持通过routing），以便为路由提供合适的分片。

shard = hash(document_id) % (num_of_primary_shards)

当分片所在的节点接收到来自协调节点的请求后，会将请求写入到Memory Buffer，然后定时（默认是每隔1秒）写入到Filesystem Cache，这个从Momery Buffer到Filesystem 　　Cache的过程就叫做refresh；

当然在某些情况下，存在Momery Buffer和Filesystem Cache的数据可能会丢失，ES是通过translog的机制来保证数据的可靠性的。其实现机制是接收到请求后，同时也会写入到translog中，当Filesystem cache中的数据写入到磁盘中时，才会清除掉，这个过程叫做flush；

在flush过程中，内存中的缓冲将被清除，内容被写入一个新段，段的fsync将创建一个新的提交点，并将内容刷新到磁盘，旧的translog将被删除并开始一个新的translog。

flush触发的时机是定时触发（默认30分钟）或者translog变得太大（默认为512M）时；



### 详细描述一下Elasticsearch更新和删除文档的过程

删除和更新也都是写操作，但是Elasticsearch中的文档是不可变的，因此不能被删除或者改动以展示其变更；

磁盘上的每个段都有一个相应的.del文件。当删除请求发送后，文档并没有真的被删除，而是在.del文件中被标记为删除。该文档依然能匹配查询，但是会在结果中被过滤掉。当段合并时，在.del文件中被标记为删除的文档将不会被写入新段。

在新的文档被创建时，Elasticsearch会为该文档指定一个版本号，当执行更新时，旧版本的文档在.del文件中被标记为删除，新版本的文档被索引到一个新段。旧版本的文档依然能匹配查询，但是会在结果中被过滤掉。



### 详细描述一下Elasticsearch搜索的过程

搜索被执行成一个两阶段过程，我们称之为 Query Then Fetch；

在初始查询阶段时，查询会广播到索引中每一个分片拷贝（主分片或者副本分片）。 每个分片在本地执行搜索并构建一个匹配文档的大小为 from + size 的优先队列。PS：在搜索的时候是会查询Filesystem Cache的，但是有部分数据还在Memory Buffer，所以搜索是近实时的。

每个分片返回各自优先队列中 所有文档的 ID 和排序值 给协调节点，它合并这些值到自己的优先队列中来产生一个全局排序后的结果列表。

接下来就是 取回阶段，协调节点辨别出哪些文档需要被取回并向相关的分片提交多个 GET 请求。每个分片加载并 丰富 文档，如果有需要的话，接着返回文档给协调节点。一旦所有的文档都被取回了，协调节点返回结果给客户端。

补充：Query Then Fetch的搜索类型在文档相关性打分的时候参考的是本分片的数据，这样在文档数量较少的时候可能不够准确，DFS Query Then Fetch增加了一个预查询的处理，询问Term和Document frequency，这个评分更准确，但是性能会变差。



### Elasticsearch对于大数据量（上亿量级）的聚合如何实现？

Elasticsearch 提供的首个近似聚合是cardinality 度量。它提供一个字段的基数，即该字段的distinct或者unique值的数目。它是基于HLL算法的。HLL 会先对我们的输入作哈希运算，然后根据哈希运算的结果中的 bits 做概率估算从而得到基数。其特点是：可配置的精度，用来控制内存的使用（更精确 ＝ 更多内存）；小的数据集精度是非常高的；我们可以通过配置参数，来设置去重需要的固定内存使用量。无论数千还是数十亿的唯一值，内存使用量只与你配置的精确度相关 .



### 你可以列出 Elasticsearch 各种类型的分析器吗？

Elasticsearch Analyzer 的类型为内置分析器和自定义分析器。

- **Standard Analyzer**

标准分析器是默认分词器，如果未指定，则使用该分词器。

它基于Unicode文本分割算法，适用于大多数语言。

- **Whitespace Analyzer**

基于空格字符切词。

- **Stop Analyzer**

在simple Analyzer的基础上，移除停用词。

- **Keyword Analyzer**

不切词，将输入的整个串一起返回。

自定义分词器的模板

自定义分词器的在Mapping的Setting部分设置：

```
PUT my_custom_index
{
 "settings":{
  "analysis":{
  "char_filter":{},
  "tokenizer":{},
  "filter":{},
  "analyzer":{}
  }
 }
}
```

脑海中还是上面的三部分组成的图示。其中：

“char_filter”:{},——对应字符过滤部分；

“tokenizer”:{},——对应文本切分为分词部分；

“filter”:{},——对应分词后再过滤部分；

“analyzer”:{}——对应分词器组成部分，其中会包含：1. 2. 3。





### ElaticSearch是如何实现master选举的？

**前置条件：**
**1、**只有是候选主节点（master：true）的节点才能成为主节点。
**2、**最小主节点数（min_master_nodes）的目的是防止脑裂。

Elasticsearch 的选主是 ZenDiscovery 模块负责的，主要包含 Ping（节点之间通过这个RPC来发现彼此）和 Unicast（单播模块包含一个主机列表以控制哪些节点需要 ping 通）这两部分；
获取主节点的核心入口为 findMaster，选择主节点成功返回对应 Master，否则返回 null。

选举流程大致描述如下：
第一步：确认候选主节点数达标，elasticsearch.yml 设置的值 discovery.zen.minimum_master_nodes;
第二步：对所有候选主节点根据nodeId字典排序，每次选举每个节点都把自己所知道节点排一次序，然后选出第一个（第0位）节点，暂且认为它是master节点。
第三步：如果对某个节点的投票数达到一定的值（候选主节点数n/2+1）并且该节点自己也选举自己，那这个节点就是master。否则重新选举一直到满足上述条件。

- 补充：
  - 这里的 id 为 string 类型。
  - master 节点的职责主要包括集群、节点和索引的管理，不负责文档级别的管理；data 节点可以关闭 http 功能。



### Master 节点和 候选 Master节点有什么区别？

主节点负责集群相关的操作，例如创建或删除索引，跟踪哪些节点是集群的一部分，以及决定将哪些分片分配给哪些节点。

拥有稳定的主节点是衡量集群健康的重要标志。

而候选主节点是被选具备候选资格，可以被选为主节点的那些节点。



### Elasticsearch中的属性 enabled, index 和 store 的功能是什么？

- enabled：false，启用的设置仅可应用于顶级映射定义和 Object 对象字段，导致 Elasticsearch 完全跳过对字段内容的解析。

仍然可以从_source字段中检索JSON，但是无法搜索或以其他任何方式存储JSON。

如果对非全局或者 Object 类型，设置 enable : false 会报错如下：

```
 "type": "mapper_parsing_exception",
 "reason": "Mapping definition for [user_id] has unsupported parameters:  [enabled : false]"
```

- index：false, 索引选项控制是否对字段值建立索引。它接受true或false，默认为true。未索引的字段不可查询。

如果非要检索，报错如下：

```
 "type": "search_phase_execution_exception",
  "reason": "Cannot search on field [user_id] since it is not indexed."
```

- store：

  某些特殊场景下，如果你只想检索单个字段或几个字段的值，而不是整个_source的值，则可以使用源过滤来实现；

  这个时候， store 就派上用场了。

![图片](https://mmbiz.qpic.cn/mmbiz_png/mjl8GCpsL9aMyWNwLib6YkaORqxb5FTNAGa2TsAbicyHFRASJVknlY2yZib2o8AGicK3HnMf6iciaD31dsrib9SL1Wrgw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### Elasticsearch中的节点（比如共20个），其中的10个选了一个master，另外10个选了另一个master，怎么办？

当集群master候选数量不小于3个时，可以通过设置最少投票通过数量（discovery.zen.minimum_master_nodes）超过所有候选节点一半以上来解决脑裂问题；
当候选数量为两个时，只能修改为唯一的一个master候选，其他作为data节点，避免脑裂问题。



### 如何解决ES集群的脑裂问题

所谓集群脑裂，是指 Elasticsearch 集群中的节点（比如共 20 个），其中的 10 个选了一个 master，另外 10 个选了另一个 master 的情况。

当集群 master 候选数量不小于 3 个时，可以通过设置最少投票通过数量（discovery.zen.minimum_master_nodes）超过所有候选节点一半以上来解决脑裂问题；
当候选数量为两个时，只能修改为唯一的一个 master 候选，其他作为 data 节点，避免脑裂问题。



### 详细描述一下ES索引文档的过程？

这里的索引文档应该理解为文档写入 ES，创建索引的过程。

**第一步：**

客户端向集群某节点写入数据，发送请求。（如果没有指定路由/协调节点，请求的节点扮演协调节点的角色。）



**第二步：**

协调节点接受到请求后，默认使用文档 ID 参与计算（也支持通过 routing），得到该文档属于哪个分片。随后请求会被转到另外的节点。

```java
bash# 路由算法：根据文档id或路由计算目标的分片id
shard = hash(document_id) % (num_of_primary_shards)
```



**第三步：**

当分片所在的节点接收到来自协调节点的请求后，会将请求写入到 Memory Buffer，然后定时（默认是每隔 1 秒）写入到F ilesystem Cache，这个从 Momery Buffer 到 Filesystem Cache 的过程就叫做 refresh；

**第四步：**

当然在某些情况下，存在 Memery Buffer 和 Filesystem Cache 的数据可能会丢失，ES 是通过 translog 的机制来保证数据的可靠性的。其实现机制是接收到请求后，同时也会写入到 translog 中，当 Filesystem cache 中的数据写入到磁盘中时，才会清除掉，这个过程叫做 flush；

**第五步：**

在 flush 过程中，内存中的缓冲将被清除，内容被写入一个新段，段的 fsync 将创建一个新的提交点，并将内容刷新到磁盘，旧的 translog 将被删除并开始一个新的 translog。

**第六步：**

flush 触发的时机是定时触发（默认 30 分钟）或者 translog 变得太大（默认为 512 M）时。

![elasticsearch_index_process.jpg](https://www.wenyuanblog.com/medias/blogimages/elasticsearch_index_process.jpg)



- 补充：关于 Lucene 的 Segement
  - Lucene 索引是由多个段组成，段本身是一个功能齐全的倒排索引。
  - 段是不可变的，允许 Lucene 将新的文档增量地添加到索引中，而不用从头重建索引。
  - 对于每一个搜索请求而言，索引中的所有段都会被搜索，并且每个段会消耗 CPU 的时钟周、文件句柄和内存。这意味着段的数量越多，搜索性能会越低。
  - 为了解决这个问题，Elasticsearch 会合并小段到一个较大的段，提交新的合并段到磁盘，并删除那些旧的小段。（段合并）



### 详细描述一下ES更新和删除文档的过程？

删除和更新也都是写操作，但是 Elasticsearch 中的文档是不可变的，因此不能被删除或者改动以展示其变更。

磁盘上的每个段都有一个相应的 .del 文件。当删除请求发送后，文档并没有真的被删除，而是在 .del 文件中被标记为删除。该文档依然能匹配查询，但是会在结果中被过滤掉。当段合并时，在 .del 文件中被标记为删除的文档将不会被写入新段。

在新的文档被创建时，Elasticsearch 会为该文档指定一个版本号，当执行更新时，旧版本的文档在 .del 文件中被标记为删除，新版本的文档被索引到一个新段。旧版本的文档依然能匹配查询，但是会在结果中被过滤掉。



### 详细描述一下ES搜索的过程？

搜索被执行成一个两阶段过程，即 Query Then Fetch；
Query阶段：
查询会广播到索引中每一个分片拷贝（主分片或者副本分片）。每个分片在本地执行搜索并构建一个匹配文档的大小为 from + size 的优先队列。PS：在搜索的时候是会查询Filesystem Cache的，但是有部分数据还在Memory Buffer，所以搜索是近实时的。
每个分片返回各自优先队列中 **所有文档的 ID 和排序值** 给协调节点，它合并这些值到自己的优先队列中来产生一个全局排序后的结果列表。
Fetch阶段：
协调节点辨别出哪些文档需要被取回并向相关的分片提交多个 GET 请求。每个分片加载并 丰富 文档，如果有需要的话，接着返回文档给协调节点。一旦所有的文档都被取回了，协调节点返回结果给客户端。

![elasticsearch_query_process.jpg](https://www.wenyuanblog.com/medias/blogimages/elasticsearch_query_process.jpg)



### 在并发情况下，ES如果保证读写一致？

可以通过版本号使用乐观并发控制，以确保新版本不会被旧版本覆盖，由应用层来处理具体的冲突；
另外对于写操作，一致性级别支持quorum/one/all，默认为quorum，即只有当大多数分片可用时才允许写操作。但即使大多数可用，也可能存在因为网络等原因导致写入副本失败，这样该副本被认为故障，分片将会在一个不同的节点上重建。
对于读操作，可以设置replication为sync(默认)，这使得操作在主分片和副本分片都完成后才会返回；如果设置replication为async时，也可以通过设置搜索请求参数_preference为primary来查询主分片，确保文档是最新版本。

### ES对于大数据量（上亿量级）的聚合如何实现？

Elasticsearch 提供的首个近似聚合是cardinality 度量。它提供一个字段的基数，即该字段的distinct或者unique值的数目。它是基于HLL算法的。HLL 会先对我们的输入作哈希运算，然后根据哈希运算的结果中的 bits 做概率估算从而得到基数。其特点是：可配置的精度，用来控制内存的使用（更精确 ＝ 更多内存）；小的数据集精度是非常高的；我们可以通过配置参数，来设置去重需要的固定内存使用量。无论数千还是数十亿的唯一值，内存使用量只与你配置的精确度相关。

### 对于GC方面，在使用ES时要注意什么？

1）倒排词典的索引需要常驻内存，无法GC，需要监控data node上segment memory增长趋势。
2）各类缓存，field cache, filter cache, indexing cache, bulk queue等等，要设置合理的大小，并且要应该根据最坏的情况来看heap是否够用，也就是各类缓存全部占满的时候，还有heap空间可以分配给其他任务吗？避免采用clear cache等“自欺欺人”的方式来释放内存。
3）避免返回大量结果集的搜索与聚合。确实需要大量拉取数据的场景，可以采用scan & scroll api来实现。
4）cluster stats驻留内存并无法水平扩展，超大规模集群可以考虑分拆成多个集群通过tribe node连接。
5）想知道heap够不够，必须结合实际应用场景，并对集群的heap使用情况做持续的监控。

### 说说你们公司ES的集群架构，索引数据大小，分片有多少，以及一些调优手段？

根据实际情况回答即可，如果是我的话会这么回答：
我司有多个ES集群，下面列举其中一个。该集群有20个节点，根据数据类型和日期分库，每个索引根据数据量分片，比如日均1亿+数据的，控制单索引大小在200GB以内。　
下面重点列举一些调优策略，仅是我做过的，不一定全面，如有其它建议或者补充欢迎留言。
部署层面：
1）最好是64GB内存的物理机器，但实际上32GB和16GB机器用的比较多，但绝对不能少于8G，除非数据量特别少，这点需要和客户方面沟通并合理说服对方。
2）多个内核提供的额外并发远胜过稍微快一点点的时钟频率。
3）尽量使用SSD，因为查询和索引性能将会得到显著提升。
4）避免集群跨越大的地理距离，一般一个集群的所有节点位于一个数据中心中。
5）设置堆内存：节点内存/2，不要超过32GB。一般来说设置export ES_HEAP_SIZE=32g环境变量，比直接写-Xmx32g -Xms32g更好一点。
6）关闭缓存swap。内存交换到磁盘对服务器性能来说是致命的。如果内存交换到磁盘上，一个100微秒的操作可能变成10毫秒。 再想想那么多10微秒的操作时延累加起来。不难看出swapping对于性能是多么可怕。
7）增加文件描述符，设置一个很大的值，如65535。Lucene使用了大量的文件，同时，Elasticsearch在节点和HTTP客户端之间进行通信也使用了大量的套接字。所有这一切都需要足够的文件描述符。
8）不要随意修改垃圾回收器（CMS）和各个线程池的大小。
9）通过设置gateway.recover_after_nodes、gateway.expected_nodes、gateway.recover_after_time可以在集群重启的时候避免过多的分片交换，这可能会让数据恢复从数个小时缩短为几秒钟。
索引层面：
1）使用批量请求并调整其大小：每次批量数据 5–15 MB 大是个不错的起始点。
2）段合并：Elasticsearch默认值是20MB/s，对机械磁盘应该是个不错的设置。如果你用的是SSD，可以考虑提高到100-200MB/s。如果你在做批量导入，完全不在意搜索，你可以彻底关掉合并限流。另外还可以增加 index.translog.flush_threshold_size 设置，从默认的512MB到更大一些的值，比如1GB，这可以在一次清空触发的时候在事务日志里积累出更大的段。
3）如果你的搜索结果不需要近实时的准确度，考虑把每个索引的index.refresh_interval 改到30s。
4）如果你在做大批量导入，考虑通过设置index.number_of_replicas: 0 关闭副本。
5）需要大量拉取数据的场景，可以采用scan & scroll api来实现，而不是from/size一个大范围。
存储层面：
1）基于数据+时间滚动创建索引，每天递增数据。控制单个索引的量，一旦单个索引很大，存储等各种风险也随之而来，所以要提前考虑+及早避免。
2）冷热数据分离存储，热数据（比如最近3天或者一周的数据），其余为冷数据。对于冷数据不会再写入新数据，可以考虑定期force_merge加shrink压缩操作，节省存储空间和检索效率



### 在并发情况下，Elasticsearch如果保证读写一致？

可以通过版本号使用乐观并发控制，以确保新版本不会被旧版本覆盖，由应用层来处理具体的冲突；

另外对于写操作，一致性级别支持quorum/one/all，默认为quorum，即只有当大多数分片可用时才允许写操作。但即使大多数可用，也可能存在因为网络等原因

导致写入副本失败，这样该副本被认为故障，分片将会在一个不同的节点上重建。

对于读操作，可以设置replication为sync(默认)，这使得操作在主分片和副本分片都完成后才会返回；如果设置replication为async时，也可以通过设置搜索请求参数_preference为primary来查询主分片，确保文档是最新版本。