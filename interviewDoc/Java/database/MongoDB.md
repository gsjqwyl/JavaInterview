**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [Mongodb是什么？](#mongodb是什么)
- [Mongodb有哪些特点？](#mongodb有哪些特点)
- [什么是非关系型数据库](#什么是非关系型数据库)
- [非关系型数据库有哪些类型](#非关系型数据库有哪些类型)
- [Mongodb的结构介绍](#mongodb的结构介绍)
- [MongoDB成为最好NoSQL数据库的原因是什么?](#mongodb成为最好nosql数据库的原因是什么)
- [MongoDB的优势有哪些](#mongodb的优势有哪些)
- [MySQL与MongoDB之间最基本的差别是什么?](#mysql与mongodb之间最基本的差别是什么)
- [什么是集合](#什么是集合)
- [什么是文档](#什么是文档)
- [什么是NoSQL数据库?NoSQL与RDBMS直接有什么区别?为什么要使用和不使用NoSQL数据库?说一说NoSQL数据库的几个优点?](#什么是nosql数据库nosql与rdbms直接有什么区别为什么要使用和不使用nosql数据库说一说nosql数据库的几个优点)
- [NoSQL数据库有哪些类型?](#nosql数据库有哪些类型)
- [分析器在MongoDB中的作用是什么?](#分析器在mongodb中的作用是什么)
- [MySQL与MongoDB之间最基本的差别是什么?](#mysql与mongodb之间最基本的差别是什么)
- [你怎么比较MongoDB、CouchDB及CouchBase?](#你怎么比较mongodbcouchdb及couchbase)
- [MongoDB成为最好NoSQL数据库的原因是什么?](#mongodb成为最好nosql数据库的原因是什么)
- ["ObjectID"有哪些部分组成](#objectid有哪些部分组成)
- [如何使用"AND"或"OR"条件循环查询集合中的文档](#如何使用and或or条件循环查询集合中的文档)
- [在MongoDB中如何排序？](#在mongodb中如何排序)
- [如何执行事务/加锁?](#如何执行事务加锁)
- [journal回放在条目(entry)不完整时(比如恰巧有一个中途故障了)会遇到问题吗?](#journal回放在条目entry不完整时比如恰巧有一个中途故障了会遇到问题吗)
- [分析器在MongoDB中的作用是什么?](#分析器在mongodb中的作用是什么)
- [如果用户移除对象的属性，该属性是否从存储层中删除?](#如果用户移除对象的属性该属性是否从存储层中删除)
- [能否使用日志特征进行安全备份?](#能否使用日志特征进行安全备份)
- [允许空值null吗?](#允许空值null吗)
- [MongoDB更新操作立刻fsync到磁盘?](#mongodb更新操作立刻fsync到磁盘)
- [如何执行事务/加锁?](#如何执行事务加锁)
- [为什么我的数据文件如此庞大?](#为什么我的数据文件如此庞大)
- [启用备份故障恢复需要多久?](#启用备份故障恢复需要多久)
- [什么是master或primary?](#什么是master或primary)
- [什么是secondary或slave?](#什么是secondary或slave)
- [必须调用getLastError来确保写操作生效了么?](#必须调用getlasterror来确保写操作生效了么)
- [MongoDB副本集选举条件有那些？](#mongodb副本集选举条件有那些)
- [简单的描述下MongoDB选举流程](#简单的描述下mongodb选举流程)
- [我应该启动一个集群分片(sharded)还是一个非集群分片的 MongoDB 环境?](#我应该启动一个集群分片sharded还是一个非集群分片的-mongodb-环境)
- [什么是MongoDB分片集群?](#什么是mongodb分片集群)
- [Monogodb中的分片什么意思？](#monogodb中的分片什么意思)
- [MongoDB中为何需要水平分片？](#mongodb中为何需要水平分片)
- [什么情况下需要用到MongoDB的分片？](#什么情况下需要用到mongodb的分片)
- [MongoDB中分片键的意义何在？](#mongodb中分片键的意义何在)
- [分片(sharding)和复制(replication)是怎样工作的?](#分片sharding和复制replication是怎样工作的)
- [构建一个分片集群需要用的那些角色？分别是什么？](#构建一个分片集群需要用的那些角色分别是什么)
- [副本集角色有那些？做是什么？](#副本集角色有那些做是什么)
- [数据在什么时候才会扩展到多个分片(shard)里?](#数据在什么时候才会扩展到多个分片shard里)
- [当我试图更新一个正在被迁移的块(chunk)上的文档时会发生什么?](#当我试图更新一个正在被迁移的块chunk上的文档时会发生什么)
- [如果在一个分片(shard)停止或者很慢的时候，我发起一个查询会怎样?](#如果在一个分片shard停止或者很慢的时候我发起一个查询会怎样)
- [我可以把moveChunk目录里的旧文件删除吗?](#我可以把movechunk目录里的旧文件删除吗)
- [怎么查看 Mongo 正在使用的链接?](#怎么查看-mongo-正在使用的链接)
- [如果块移动操作(moveChunk)失败了，我需要手动清除部分转移的文档吗?](#如果块移动操作movechunk失败了我需要手动清除部分转移的文档吗)
- [如果我在使用复制技术(replication)，可以一部分使用日志(journaling)而其他部分则不使用吗?](#如果我在使用复制技术replication可以一部分使用日志journaling而其他部分则不使用吗)
- [MongoDB在A:{B,C}上建立索引，查询A:{B,C}和A:{C,B}都会使用索引吗？](#mongodb在abc上建立索引查询abc和acb都会使用索引吗)
- [如果一个分片（Shard）停止或很慢的时候，发起一个查询会怎样？](#如果一个分片shard停止或很慢的时候发起一个查询会怎样)
- [MongoDB支持存储过程吗？如果支持的话，怎么用？](#mongodb支持存储过程吗如果支持的话怎么用)
- [解释一下什么是MongoDB中的GridFS ?](#解释一下什么是mongodb中的gridfs-)
- [如何理解MongoDB中的GridFS机制，MongoDB为何使用GridFS来存储文件？](#如何理解mongodb中的gridfs机制mongodb为何使用gridfs来存储文件)
- [MongoDB支持存储过程吗？如果支持的话，怎么用？](#mongodb支持存储过程吗如果支持的话怎么用)
- [如何理解MongoDB中的GridFS机制，MongoDB为何使用GridFS来存储文件？](#如何理解mongodb中的gridfs机制mongodb为何使用gridfs来存储文件)
- [为什么MongoDB的数据文件很大？](#为什么mongodb的数据文件很大)
- [MongoDB在A:{B,C}上建立索引，查询A:{B,C}和A:{C,B}都会使用索引吗？](#mongodb在abc上建立索引查询abc和acb都会使用索引吗)
- [如果用户移除对象的属性，该属性是否从存储层中删除？](#如果用户移除对象的属性该属性是否从存储层中删除)
- [能否使用日志特征进行安全备份？](#能否使用日志特征进行安全备份)
- [更新操作立刻fsync到磁盘？](#更新操作立刻fsync到磁盘)
- [如何执行事务/加锁？](#如何执行事务加锁)
- [什么是master或primary？](#什么是master或primary)
- [getLastError的作用](#getlasterror的作用)
- [分片（sharding）和复制（replication）是怎样工作的？](#分片sharding和复制replication是怎样工作的)
- [数据在什么时候才会扩展到多个分片（shard）里？](#数据在什么时候才会扩展到多个分片shard里)
- [什么是”mongod“](#什么是mongod)
- ["mongod"参数有什么](#mongod参数有什么)
- [什么是"mongo"](#什么是mongo)
- [MongoDB哪个命令可以切换数据库](#mongodb哪个命令可以切换数据库)
- [为什么用MOngoDB？](#为什么用mongodb)
- [MongoDB适合应用在那些场景?](#mongodb适合应用在那些场景)
- [在哪些场景使用MongoDB](#在哪些场景使用mongodb)
- [MongoDB中的命名空间是什么意思?](#mongodb中的命名空间是什么意思)
- [哪些语言支持MongoDB?](#哪些语言支持mongodb)
- [在MongoDB中如何创建一个新的数据库](#在mongodb中如何创建一个新的数据库)
- [在MongoDB中如何查看数据库列表](#在mongodb中如何查看数据库列表)
- [MongoDB中的分片是什么意思](#mongodb中的分片是什么意思)
- [如何查看使用MongoDB的连接Sharding - MongoDB Manual21.如何查看使用MongoDB的连接](#如何查看使用mongodb的连接sharding---mongodb-manual21如何查看使用mongodb的连接)
- [什么是复制](#什么是复制)
- [在MongoDB中如何在集合中插入一个文档](#在mongodb中如何在集合中插入一个文档)
- [在MongoDB中如何除去一个数据库Collection Methods24.在MongoDB中如何除去一个数据库](#在mongodb中如何除去一个数据库collection-methods24在mongodb中如何除去一个数据库)
- [在MongoDB中如何查看一个已经创建的集合](#在mongodb中如何查看一个已经创建的集合)
- [在MongoDB中如何删除一个集合](#在mongodb中如何删除一个集合)
- [为什么要在MongoDB中使用分析器](#为什么要在mongodb中使用分析器)
- [分析器在MongoDB中的作用是什么?](#分析器在mongodb中的作用是什么)
- [MongoDB支持主键外键关系吗](#mongodb支持主键外键关系吗)
- [MongoDB支持哪些数据类型](#mongodb支持哪些数据类型)
- [为什么要在MongoDB中用"Code"数据类型](#为什么要在mongodb中用code数据类型)
- [为什么要在MongoDB中用"Regular Expression"数据类型](#为什么要在mongodb中用regular-expression数据类型)
- [为什么在MongoDB中使用"Object ID"数据类型](#为什么在mongodb中使用object-id数据类型)
- ["ObjectID"由哪些部分组成](#objectid由哪些部分组成)
- [在MongoDb中什么是索引](#在mongodb中什么是索引)
- [如何添加索引](#如何添加索引)
- [用什么方法可以格式化输出结果](#用什么方法可以格式化输出结果)
- [如何使用"AND"或"OR"条件循环查询集合中的文档](#如何使用and或or条件循环查询集合中的文档)
- [在MongoDB中如何更新数据](#在mongodb中如何更新数据)
- [如何删除文档](#如何删除文档)
- [在MongoDB中如何排序](#在mongodb中如何排序)
- [什么是聚合](#什么是聚合)
- [在MongoDB中什么是副本集](#在mongodb中什么是副本集)

<!-- /TOC -->

### Mongodb是什么？

MongoDB 是由 C++语言编写的，是一个基于分布式文件存储的开源数据库系统。在高负载的情况下，添加更多的节点，可以保证服务器性能。MongoDB 旨在给 WEB 应用提供可扩展的高性能数据存储解决方案。

MongoDB 将数据存储给一个文档，数据结构由键值(key=>value)对组成。MongoDB 文档类似于 JSON 对象。字段值可以包含其他文档，数组及文档数组。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210326004314.png)

### Mongodb有哪些特点？

**1、**MongoDB 是一个面向文档存储的数据库，操作起来比较简单和容易。

**2、**你可以在 MongoDB 记录中设置任何属性的索引 (如：FirstName="Sameer",Address="8 Gandhi Road")来实现更快的排序。

**3、**你可以通过本地或者网络创建数据镜像，这使得 MongoDB 有更强的扩展性。

**4、**如果负载的增加（需要更多的存储空间和更强的处理能力） ，它可以分布在计算机网络中的其他节点上这就是所谓的分片。

**5、**Mongo 支持丰富的查询表达式。查询指令使用 JSON 形式的标记，可轻易查询文档中内嵌的对象及数组。

**6、**MongoDb 使用 update()命令可以实现替换完成的文档（数据）或者一些指定的数据字段 。

**7、**Mongodb 中的 Map/reduce 主要是用来对数据进行批量处理和聚合操作。

**8、**Map 和 Reduce。Map 函数调用 emit(key,value)遍历集合中所有的记录，将 key 与 value 传给 Reduce 函数进行处理。

**9、**Map 函数和 Reduce 函数是使用 Javascript 编写的，并可以通过 db.runCommand 或 mapreduce 命令来执行 MapReduce 操作。

**10、**GridFS 是 MongoDB 中的一个内置功能，可以用于存放大量小文件。

**11、**MongoDB 允许在服务端执行脚本， 可以用 Javascript 编写某个函数，直接在服务端执行，也可以把函数的定义存储在服务端，下次直接调用即可。



### 什么是非关系型数据库

非关系型数据库是对不同于传统关系型数据库的统称。非关系型数据库的显著特点是不使用SQL作为查询语言，数据存储不需要特定的表格模式。由于简单的设计和非常好的性能所以被用于大数据和Web Apps等



### 非关系型数据库有哪些类型

- **-Key-Value 存储：Amazon S3**
- **图表：Neo4J**
- **文档存储：MongoDB**
- **基于列存储：Cassandra**



### Mongodb的结构介绍

数据库中存储的对象设计bson，一种类似json的二进制文件，由键值对组成



### MongoDB成为最好NoSQL数据库的原因是什么?

以下特点使得MongoDB成为最好的NoSQL数据库：

面向文件的

高性能

高可用性

易扩展性

丰富的查询语言



### MongoDB的优势有哪些

- 面向文档的存储：以 JSON 格式的文档保存数据。
- 任何属性都可以建立索引。
- 复制以及高可扩展性。
- 自动分片。
- 丰富的查询功能。
- 快速的即时更新。
- 来自 MongoDB 的专业支持。



### MySQL与MongoDB之间最基本的差别是什么?

MySQL和MongoDB两者都是免费开源的数据库。MySQL和MongoDB有许多基本差别包括数据的表示(data representation)，查询，关系，事务，schema的设计和定义，标准化(normalization)，速度和性能。

通过比较MySQL和MongoDB，实际上我们是在比较关系型和非关系型数据库，即数据存储结构不同。详细阅读



### 什么是集合

集合就是一组 MongoDB 文档。它相当于关系型数据库（RDBMS）中的表这种概念。集合位于单独的一个数据库中。一个集合内的多个文档可以有多个不同的字段。一般来说，集合中的文档都有着相同或相关的目的。



### 什么是文档

文档由一组key value组成。文档是动态模式,这意味着同一集合里的文档不需要有相同的字段和结构。在关系型数据库中table中的每一条记录相当于MongoDB中的一个文档。





### 什么是NoSQL数据库?NoSQL与RDBMS直接有什么区别?为什么要使用和不使用NoSQL数据库?说一说NoSQL数据库的几个优点?

NoSQL是非关系型数据库，NoSQL = Not Only SQL。

关系型数据库采用的结构化的数据，NoSQL采用的是键值对的方式存储数据。

在处理非结构化/半结构化的大数据时；在水平方向上进行扩展时；随时应对动态增加的数据项时可以优先考虑使用NoSQL数据库。

再考虑数据库的成熟度；支持；分析和商业智能；管理及专业性等问题时，应优先考虑关系型数据库。



### NoSQL数据库有哪些类型?

NoSQL数据库的类型

例如：MongoDB, Cassandra, CouchDB, Hypertable, Redis, Riak, HBASE, Memcache



### 分析器在MongoDB中的作用是什么?

MongoDB中包括了一个可以显示数据库中每个操作性能特点的数据库分析器。通过这个分析器你可以找到比预期慢的查询(或写操作);利用这一信息，比如，可以确定是否需要添加索引。

 

### MySQL与MongoDB之间最基本的差别是什么?

MySQL和MongoDB两者都是免费开源的数据库。MySQL和MongoDB有许多基本差别包括数据的表示(data representation)，查询，关系，事务，schema的设计和定义，标准化(normalization)，速度和性能。

通过比较MySQL和MongoDB，实际上我们是在比较关系型和非关系型数据库，即数据存储结构不同。



### 你怎么比较MongoDB、CouchDB及CouchBase?

MongoDB和CouchDB都是面向文档的数据库。MongoDB和CouchDB都是开源NoSQL数据库的最典型代表。除了都以文档形式存储外它

们没有其他的共同点。

MongoDB和CouchDB在数据模型实现、接口、对象存储以及复制方法等方面有很多不同。



### MongoDB成为最好NoSQL数据库的原因是什么?

以下特点使得MongoDB成为最好的NoSQL数据库：

- 面向文件的
- 高性能
- 高可用性
- 易扩展性
- 丰富的查询语言



### "ObjectID"有哪些部分组成

一共有四部分组成:时间戳、客户端ID、客户进程ID、三个字节的增量计数器。
_id是一个 12 字节长的十六进制数，它保证了每一个文档的唯一性。在插入文档时，需要提供_id。如果你不提供，那么 MongoDB 就会为每一文档提供一个唯一的 id。_id的头 4 个字节代表的是当前的时间戳，接着的后 3 个字节表示的是机器 id 号，接着的 2 个字节表示 MongoDB 服务器进程 id，最后的 3 个字节代表递增值。



### 如何使用"AND"或"OR"条件循环查询集合中的文档

在 find() 方法中，如果传入多个键，并用逗号( , )分隔它们，那么 MongoDB 会把它看成是AND条件。

>db.mycol.find({key1:value1, key2:value2}).pretty()
若基于OR条件来查询文档，可以使用关键字$or。

db.mycol.find(
{
$or: [
  {key1: value1}, {key2:value2}
]
}
).pretty()



### 在MongoDB中如何排序？

MongoDB 中的文档排序是通过 sort() 方法来实现的。sort() 方法可以通过一些参数来指定要进行排序的字段，并使用 1 和 -1 来指定排序方式，其中 1 表示升序，而 -1 表示降序。

> db.connectionName.find({key:value}).sort({columnName:1})



### 如何执行事务/加锁?

MongoDB没有使用传统的锁或者复杂的带回滚的事务，因为它设计的宗旨是轻量，快速以及可预计的高性能。可以把它类比成MySQL MylSAM的自动提交模式。通过精简对事务的支持，性能得到了提升，特别是在一个可能会穿过多个服务器的系统里。



### journal回放在条目(entry)不完整时(比如恰巧有一个中途故障了)会遇到问题吗?

每个journal (group)的写操作都是一致的，除非它是完整的否则在恢复过程中它不会回放。



### 分析器在MongoDB中的作用是什么?

MongoDB中包括了一个可以显示数据库中每个操作性能特点的数据库分析器。通过这个分析器你可以找到比预期慢的查询(或写操作);

利用这一信息，比如，可以确定是否需要添加索引。



### 如果用户移除对象的属性，该属性是否从存储层中删除?

是的，用户移除属性然后对象会重新保存(re-save())。



### 能否使用日志特征进行安全备份?

是的。



### 允许空值null吗?

对于对象成员而言，是的。然而用户不能够添加空值(null)到数据库丛集(collection)因为空值不是对象。然而用户能够添加空对象{}。



### MongoDB更新操作立刻fsync到磁盘?

不会，磁盘写操作默认是延迟执行的。写操作可能在两三秒(默认在60秒内)后到达磁盘。

例如，如果一秒内数据库收到一千个对一个对象递增的操作，仅刷新磁盘一次。(注意，尽管fsync选项在命令行和经过getLastError_old是有效的)



### 如何执行事务/加锁?

MongoDB没有使用传统的锁或者复杂的带回滚的事务，因为它设计的宗旨是轻量，快速以及可预计的高性能。可以把它类比成MySQLMylSAM的自动提交模式。通过精简对事务的支持，性能得到了提升，特别是在一个可能会穿过多个服务器的系统里。



### 为什么我的数据文件如此庞大?

MongoDB会积极的预分配预留空间来防止文件系统碎片。



### 启用备份故障恢复需要多久?

从备份数据库声明主数据库宕机到选出一个备份数据库作为新的主数据库将花费10到30秒时间。

这期间在主数据库上的操作将会失败--包括写入和强一致性读取(strong consistent read)操作。

然而，你还能在第二数据库上执行最终一致性查询(eventually consistent query)(在slaveOk模式下)，即使在这段时间里。



### 什么是master或primary?

它是当前备份集群(replica set)中负责处理所有写入操作的主要节点/成员。

在一个备份集群中，当失效备援(failover)事件发生时，一个另外的成员会变成primary。



### 什么是secondary或slave?

Seconday从当前的primary上复制相应的操作。它是通过跟踪复制oplog(local.oplog.rs)做到的。



### 必须调用getLastError来确保写操作生效了么?

不用。不管你有没有调用getLastError(又叫"Safe Mode")服务器做的操作都一样。调用getLastError只是为了确认写操作成功提交了。当然，你经常想得到确认，但是写操作的安全性和是否生效不是由这个决定的。



### MongoDB副本集选举条件有那些？

1.复制集初始化。
2.主节点挂掉。
3.主节点脱离副本集（可能是网络原因）。
4.参与选举的节点数量必须大于副本集总节点数量的一半，如果已经小于一半了所有节点保持只读状态。 



### 简单的描述下MongoDB选举流程

**1、** 副本集中的主节点选举必须满足“大多数”的原则，所谓“大多数”是指副本中一半以上的成员。副本集中成员只有在得到大多数成员投票支持时，才能成为主节点。例如：有N个副本集成员节点，必须有N/2+1个成员投票支持某个节点，此节点才能成为主节点。注意：副本集中若有成员节点处于不可用状态，并不会影响副本集中的“大多数”，“大多数”是以副本集的配置来计算的。

**2、** 仲裁节点（Arbiter）它并不保存数据，并且不能被选举为主节点，但是具有投票权。仲裁节点使用最小的资源，不能将Arbiter部署在同一个数据集节点中。

**3、** 副本集中最好是有奇数个成员节点，如果有偶数个节点，最好加一个仲裁节点。若副本集中有偶数个成员节点，如图2所示，IDC1网络连不通IDC2，IDC1和IDC2内的成员节点分别会发生选举主节点的行为，然而选举因都无法满足大多数的原则，都不能选出主节点；加入一个仲裁节点之后，则副本集就能满足大多数原则，从中选出主节点了。

**4、** 如果副本集成员节点数量是奇数，就不再需要仲裁者。但是如果在成员节点是奇数时，强行使用仲裁者，会导致选举耗时变长。由于添加了仲裁者就可能出现两个成员节点票数相同的情况，从而导致选举耗时变长。

**5、** 若在一轮投票中，副本集中成员节点被投了反对票，则本轮不能被选为主节点。例如，在一个10个成员节点的副本集，某轮投票中，成员节点A由于数据延迟较大被某个成员节点投了反对票，则A同时收到了9票赞成票，然而A仍然不能被选为主节点。

**6、** 集群中的优先级为0的节点不能成为主节点，并且不能触发选举，但是具有投票权，并且拥有与主节点一致的数据集。



### 我应该启动一个集群分片(sharded)还是一个非集群分片的 MongoDB 环境?

为开发便捷起见，我们建议以非集群分片(unsharded)方式开始一个 MongoDB 环境，除非一台服务器不足以存放你的初始数据集。从非集群分片升级到集群分片(sharding)是无缝的，所以在你的数据集还不是很大的时候没必要考虑集群分片(sharding)。



### 什么是MongoDB分片集群?

Sharding cluster是一种可以水平扩展的模式,在数据量很大时特给力,实际大规模应用一般会采用这种架 构去构建。sharding分片很好的解决了单台服务器磁盘空间、内存、cpu等硬件资源的限制问题，把数据水 平拆分出去，降低单节点的访问压力。每个分片都是一个独立的数据库，所有的分片组合起来构成一个逻辑上 的完整的数据库。因此，分片机制降低了每个分片的数据操作量及需要存储的数据量，达到多台服务器来应对 不断增加的负载和数据的效果。



### Monogodb中的分片什么意思？

分片是将数据水平切分到不同的物理节点，当应用数据越来越大的时候，数据量也会越来越大。当数据量增长时，单台机器有可能无法存储数据或可接受的读取写入吞吐量，利用分片技术可以添加更多的机器来应对数据量增加以及读写操作的要求。



### MongoDB中为何需要水平分片？

1）减少单机请求数,将单机负载,提高总负载

2）减少单机的存储空间,提高总存空间



### 什么情况下需要用到MongoDB的分片？

**1、** 机器的磁盘不够用了。使用分片解决磁盘空间的问题。

**2、** 单个mongod已经不能满足写数据的性能要求。通过分片让写压力分散到各个分片上面,使用分片服务器自 身的资源。

**3、** 想把大量数据放到内存里提高性能。和上面一样,通过分片使用分片服务器自身的资源。



### MongoDB中分片键的意义何在？

**1、** 一个好的片键对分片至关重要。片键必须是一个索引 ,通 过 sh.shardCollection 加会自动创建索 引。一个自增的片键对写入和数据均匀分布就不是很好, 因为自增的片键总会在一个分片上写入,后续达到某 个阀值可能会写到别的分片。但是按照片键查询会非常高效。随机片键对数据的均匀分布效果很好。注意尽量 避免在多个分片上进行查询。

**2、** 在所有分片上查询,mongos 会对结果进行归并排序，提高查询效率和速度



### 分片(sharding)和复制(replication)是怎样工作的?

每一个分片(shard)是一个分区数据的逻辑集合。分片可能由单一服务器或者集群组成，我们推荐为每一个分片(shard)使用集群。



### 构建一个分片集群需要用的那些角色？分别是什么？

**1、分片服务器（Shard Server）**  mongod 实例,用于存储实际的数据块,实际生产环境中一个 shard server 角色可由几台机器组个一 个 relica set 承担,防止主机单点故障  这是一个独立普通的mongod进程,保存数据信息。可以是一个副本集也可以是单独的一台服务器。

**2、配置服务器（Config Server）**  mongod 实例,存储了整个 Cluster Metadata,其中包括 chunk 信息。 这是一个独立的mongod进程,保存集群和分片的元数据,即各分片包含了哪些数据的信息。最先开始建立, 启用日志功能。像启动普通的 mongod 一样启动  配置服务器,指定configsvr 选项。不需要太多的空间和资源,配置服务器的 1KB 空间相当于真是数据 的 200MB。保存的只是数据的分布表。

**3、路由服务器（Route Server）**  mongos实例,前端路由,客户端由此接入,且让整个集群看上去像单一数据库,前端应用  起到一个路由的功能,供程序连接。本身不保存数据,在启动时从配置服务器加载集群信息,开启 mongos 进程需要知道配置服务器的地址,指定configdb选项。



### 副本集角色有那些？做是什么？

**1、主节点（Primary）**

接收所有的写请求，然后把修改同步到所有Secondary。一个Replica Set只能有一个Primary节点，当 Primary挂掉后，其他Secondary或者Arbiter节点会重新选举出来一个主节点。默认读请求也是发到Primary节点处理的，可以通过修改客户端连接配置以支持读取Secondary节点。

**2、副本节点（Secondary）**

与主节点保持同样的数据集。当主节点挂掉的时候，参与选主。

**3、仲裁者（Arbiter）**

不保有数据，不参与选主，只进行选主投票。使用Arbiter可以减轻数据存储的硬件需求，Arbiter几乎没什 么大的硬件资源需求，但重要的一点是，在生产环境下它和其他数据节点不要部署在同一台机器上。



### 数据在什么时候才会扩展到多个分片(shard)里?

MongoDB 分片是基于区域(range)的。所以一个集合(collection)中的所有的对象都被存放到一个块(chunk)中。只有当存在多余一个块的时候，才会有多个分片获取数据的选项。现在，每个默认块的大小是 64Mb，所以你需要至少 64 Mb 空间才可以实施一个迁移。



### 当我试图更新一个正在被迁移的块(chunk)上的文档时会发生什么?

更新操作会立即发生在旧的分片(shard)上，然后更改才会在所有权转移(ownership transfers)前复制到新的分片上。



### 如果在一个分片(shard)停止或者很慢的时候，我发起一个查询会怎样?

如果一个分片(shard)停止了，除非查询设置了“Partial”选项，否则查询会返回一个错误。如果一个分片(shard)响应很慢，MongoDB则会等待它的响应。



### 我可以把moveChunk目录里的旧文件删除吗?

没问题，这些文件是在分片(shard)进行均衡操作(balancing)的时候产生的临时文件。一旦这些操作已经完成，相关的临时文件也应该被删除掉。但目前清理工作是需要手动的，所以请小心地考虑再释放这些文件的空间。



### 怎么查看 Mongo 正在使用的链接?

db._adminCommand("connPoolStats");



### 如果块移动操作(moveChunk)失败了，我需要手动清除部分转移的文档吗?

不需要，移动操作是一致(consistent)并且是确定性的(deterministic);一次失败后，移动操作会不断重试;当完成后，数据只会出现在新的分片里(shard)。



### 如果我在使用复制技术(replication)，可以一部分使用日志(journaling)而其他部分则不使用吗?

可以。



### MongoDB在A:{B,C}上建立索引，查询A:{B,C}和A:{C,B}都会使用索引吗？

不会，只会在A:{B,C}上使用索引。



### 如果一个分片（Shard）停止或很慢的时候，发起一个查询会怎样？

如果一个分片停止了，除非查询设置了“Partial”选项，否则查询会返回一个错误。如果一个分片响应很慢，MongoDB会等待它的响应。



### MongoDB支持存储过程吗？如果支持的话，怎么用？

MongoDB支持存储过程，它是javascript写的，保存在db.system.js表中。



### 解释一下什么是MongoDB中的GridFS ?

为了存储和检索大文件，例如图像，视频文件和音频文件，使用GridFS。默认情况下，它使用两个文件fs.files和fs.chunks来存储文件的元数据和块。



### 如何理解MongoDB中的GridFS机制，MongoDB为何使用GridFS来存储文件？

GridFS是一种将大型文件存储在MongoDB中的文件规范。使用GridFS可以将大文件分隔成多个小文档存放，这样我们能够有效的保存大文档，而且解决了BSON对象有限制的问题。



### MongoDB支持存储过程吗？如果支持的话，怎么用？

MongoDB支持存储过程，它是javascript写的，保存在db.system.js表中。



### 如何理解MongoDB中的GridFS机制，MongoDB为何使用GridFS来存储文件？

GridFS是一种将大型文件存储在MongoDB中的文件规范。使用GridFS可以将大文件分隔成多个小文档存放，这样我们能够有效的保存大文档，而且解决了BSON对象有限制的问题。



### 为什么MongoDB的数据文件很大？

MongoDB采用的预分配空间的方式来防止文件碎片。



### MongoDB在A:{B,C}上建立索引，查询A:{B,C}和A:{C,B}都会使用索引吗？

不会，只会在A:{B,C}上使用索引。



### 如果用户移除对象的属性，该属性是否从存储层中删除？

是的，用户移除属性然后对象会重新保存（re-save()）。



### 能否使用日志特征进行安全备份？

是的



### 更新操作立刻fsync到磁盘？

一般磁盘的写操作都是延迟执行的



### 如何执行事务/加锁？

MongoDB没有使用传统的锁或者复杂的带回滚的事务，因为它设计的宗旨是轻量，快速以及可预计的高性能。可以把它类比成MySQL MylSAM的自动提交模式。通过精简对事务的支持，性能得到了提升，特别是在一个可 能会穿过多个服务器的系统里。



### 什么是master或primary？

它是当前备份集群(replica set)中负责处理所有写入操作的主要节点/成员。在一个备份集群中，当失效备援(failover)事件发生时，一个另外的成员会变成primary。

### getLastError的作用

调用getLastError 可以确认当前的写操作是否成功的提交



### 分片（sharding）和复制（replication）是怎样工作的？

分片可能是单一的服务器或者集群组成，推荐使用集群



### 数据在什么时候才会扩展到多个分片（shard）里？

mongodb分片是基于区域的，所以一个集合的所有对象都放置在同一个块中，只有当存在多余一个块的时候，才会有多个分片获取数据的选项



### 什么是”mongod“

mongod是处理MongoDB系统的主要进程。它处理数据请求，管理数据存储，和执行后台管理操作。当我们运行mongod命令意味着正在启动MongoDB进程,并且在后台运行。



### "mongod"参数有什么

- 传递数据库存储路径，默认是"/data/db"
- 端口号 默认是 "27017"



### 什么是"mongo"

它是一个命令行工具用于连接一个特定的mongod实例。当我们没有带参数运行mongo命令它将使用默认的端口号和localhost连接



### MongoDB哪个命令可以切换数据库

MongoDB 用 use +数据库名称的方式来创建数据库。use 会创建一个新的数据库，如果该数据库存在，则返回这个数据库。





### 为什么用MOngoDB？

**1、**架构简单

**2、**没有复杂的连接

**3、**深度查询能力,MongoDB支持动态查询。

**4、**容易调试

**5、**容易扩展

**6、**不需要转化/映射应用对象到数据库对象

**7、**使用内部内存作为存储工作区,以便更快的存取数据。



### MongoDB适合应用在那些场景?

从目前阿里云 MongoDB 云数据库上的用户看，MongoDB 的应用已经渗透到各个领域，比如游戏、物流、电商、内容管理、社交、物联网、视频直播等，以下是几个实际的应用案例。

游戏场景，使用 MongoDB 存储游戏用户信息，用户的装备、积分等直接以内嵌文档的形式存储，方便查询、更新

物流场景，使用 MongoDB 存储订单信息，订单状态在运送过程中会不断更新，以 MongoDB 内嵌数组的形式来存储，一次查询就能将订单所有的变更读取出来。

社交场景，使用 MongoDB 存储存储用户信息，以及用户发表的朋友圈信息，通过地理位置索引实现附近的人、地点等功能

物联网场景，使用 MongoDB 存储所有接入的智能设备信息，以及设备汇报的日志信息，并对这些信息进行多维度的分析

视频直播，使用 MongoDB 存储用户信息、礼物信息等



### 在哪些场景使用MongoDB

- 大数据
- 内容管理系统
- 移动端Apps
- 数据管理



### MongoDB中的命名空间是什么意思?

MongoDB内部有预分配空间的机制，每个预分配的文件都用0进行填充。

数据文件每新分配一次，它的大小都是上一个数据文件大小的2倍，每个数据文件最大2G。欢迎关注公种浩：程序员追风，回复003领取一套200页的2020最新的Java面试题手册。

MongoDB每个集合和每个索引都对应一个命名空间，这些命名空间的元数据集中在16M的*.ns文件中，平均每个命名占用约 628 字节，也即整个数据库的命名空间的上限约为24000。

如果每个集合有一个索引（比如默认的_id索引），那么最多可以创建12000个集合。如果索引数更多，则可创建的集合数就更少了。同时，如果集合数太多，一些操作也会变慢。

要建立更多的集合的话，MongoDB 也是支持的，只需要在启动时加上“--nssize”参数，这样对应数据库的命名空间文件就可以变得更大以便保存更多的命名。这个命名空间文件（.ns文件）最大可以为 2G。

每个命名空间对应的盘区不一定是连续的。与数据文件增长相同，每个命名空间对应的盘区大小都是随分配次数不断增长的。目的是为了平衡命名空间浪费的空间与保持一个命名空间数据的连续性。

需要注意的一个命名空间![图片](https://mmbiz.qpic.cn/mmbiz_svg/cGNScwnYvk6sMgiawlESrp2FqDuaIQiaDst1AGMibLuVib4zKQPn1iaaPMn7FQia2bB9GCmibw5DUz58yWoR9bft6wuuqicv7V8kAJ8u/640?wx_fmt=svg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)freelist是否有大小合适的盘区可以使用，如果有就回收空闲的磁盘空间。



### 哪些语言支持MongoDB?

C、C++、C#、Java、Node.js、Perl、Php 等



### 在MongoDB中如何创建一个新的数据库

MongoDB 用 use + 数据库名称 的方式来创建数据库。use 会创建一个新的数据库，如果该数据库存在，则返回这个数据库。



### 在MongoDB中如何查看数据库列表

使用命令"show dbs"



### MongoDB中的分片是什么意思

分片是将数据水平切分到不同的物理节点。当应用数据越来越大的时候，数据量也会越来越大。当数据量增长时，单台机器有可能无法存储数据或可接受的读取写入吞吐量。利用分片技术可以添加更多的机器来应对数据量增加以及读写操作的要求。



### 如何查看使用MongoDB的连接Sharding - MongoDB Manual21.如何查看使用MongoDB的连接

使用命令"db.adminCommand(“connPoolStats”)"

<pre language="javascript" code_block="true">>db.adminCommand(“connPoolStats”)</pre>



### 什么是复制

复制是将数据同步到多个服务器的过程，通过多个数据副本存储到多个服务器上增加数据可用性。复制可以保障数据的安全性，灾难恢复，无需停机维护（如备份，重建索引，压缩），分布式读取数据。



### 在MongoDB中如何在集合中插入一个文档

要想将数据插入 MongoDB 集合中，需要使用 insert() 或 save() 方法。

```
db.collectionName.insert({"key":"value"})
db.collectionName.save({"key":"value"})
```



### 在MongoDB中如何除去一个数据库Collection Methods24.在MongoDB中如何除去一个数据库

MongoDB 的 dropDatabase() 命令用于删除已有数据库。

```
db.dropDatabase()
```



### 在MongoDB中如何查看一个已经创建的集合

可以使用show collections 查看当前数据库中的所有集合清单

```
show collections
```



### 在MongoDB中如何删除一个集合

MongoDB 利用 db.collection.drop() 来删除数据库中的集合。

```
db.CollectionName.drop()
```



### 为什么要在MongoDB中使用分析器

数据库分析工具(Database Profiler)会针对正在运行的mongod实例收集数据库命令执行的相关信息。包括增删改查的命令以及配置和管理命令。分析器(profiler)会写入所有收集的数据到 system.profile集合，一个capped集合在管理员数据库。分析器默认是关闭的你能通过per数据库或per实例开启。



### 分析器在MongoDB中的作用是什么?

MongoDB中包括了一个可以显示数据库中每个操作性能特点的数据库分析器。通过这个分析器你可以找到比预期慢的查询(或写操作);利用这一信息，比如，可以确定是否需要添加索引。



### MongoDB支持主键外键关系吗

默认MongoDB不支持主键和外键关系。用Mongodb本身的API需要硬编码才能实现外键关联，不够直观且难度较大。



### MongoDB支持哪些数据类型

String、Integer、Double、Boolean、Object、Object ID、Arrays、Min/Max Keys、Datetime、Code、Regular Expression等



### 为什么要在MongoDB中用"Code"数据类型

"Code"类型用于在文档中存储 JavaScript 代码。



### 为什么要在MongoDB中用"Regular Expression"数据类型

"Regular Expression"类型用于在文档中存储正则表达式



### 为什么在MongoDB中使用"Object ID"数据类型

"ObjectID"数据类型用于存储文档id



### "ObjectID"由哪些部分组成

一共有四部分组成:时间戳、客户端ID、客户进程ID、三个字节的增量计数器

_id是一个 12 字节长的十六进制数，它保证了每一个文档的唯一性。在插入文档时，需要提供 _id 。如果你不提供，那么 MongoDB 就会为每一文档提供一个唯一的 id。_id 的头 4 个字节代表的是当前的时间戳，接着的后 3 个字节表示的是机器 id 号，接着的 2 个字节表示MongoDB 服务器进程 id，最后的 3 个字节代表递增值。



### 在MongoDb中什么是索引

索引用于高效的执行查询.没有索引MongoDB将扫描查询整个集合中的所有文档这种扫描效率很低，需要处理大量数据。索引是一种特殊的数据结构，将一小块数据集保存为容易遍历的形式。索引能够存储某种特殊字段或字段集的值，并按照索引指定的方式将字段值进行排序。



### 如何添加索引

使用 db.collection.createIndex() 在集合中创建一个索引

```
db.collectionName.createIndex({columnName:1})
```



### 用什么方法可以格式化输出结果

使用pretty() 方法可以格式化显示结果

```
>db.collectionName.find().pretty()
```



### 如何使用"AND"或"OR"条件循环查询集合中的文档

在 find() 方法中，如果传入多个键，并用逗号( , )分隔它们，那么 MongoDB 会把它看成是AND条件。

```
>db.mycol.find({key1:value1, key2:value2}).pretty()
```

若基于OR条件来查询文档，可以使用关键字$or。

```
>db.mycol.find(
 {
  $or: [
    {key1: value1}, {key2:value2}
  ]
 }
).pretty()
```



### 在MongoDB中如何更新数据

update() 与 save() 方法都能用于更新集合中的文档。update() 方法更新已有文档中的值，而 save() 方法则是用传入该方法的文档来替换已有文档。



### 如何删除文档

MongoDB 利用 remove() 方法 清除集合中的文档。它有 2 个可选参数：

- deletion criteria：（可选）删除文档的标准。
- justOne：（可选）如果设为 true 或 1，则只删除一个文档。

```
>db.collectionName.remove({key:value})
```



### 在MongoDB中如何排序

MongoDB 中的文档排序是通过 sort() 方法来实现的。sort() 方法可以通过一些参数来指定要进行排序的字段，并使用 1 和 -1 来指定排序方式，其中 1 表示升序，而 -1 表示降序。

```
>db.connectionName.find({key:value}).sort({columnName:1})
```



### 什么是聚合

聚合操作能够处理数据记录并返回计算结果。聚合操作能将多个文档中的值组合起来，对成组数据执行各种操作，返回单一的结果。它相当于 SQL 中的 count(*) 组合 group by。对于 MongoDB 中的聚合操作，应该使用 aggregate() 方法。

```
>db.COLLECTION_NAME.aggregate(AGGREGATE_OPERATION)
```



### 在MongoDB中什么是副本集

在MongoDB中副本集由一组MongoDB实例组成，包括一个主节点多个次节点，MongoDB客户端的所有数据都写入主节点(Primary),副节点从主节点同步写入数据，以保持所有复制集内存储相同的数据，提高数据可用性。