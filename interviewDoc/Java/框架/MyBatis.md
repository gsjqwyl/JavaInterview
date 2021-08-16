**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [什么是Mybatis？](#什么是mybatis)
- [Mybaits的优点：](#mybaits的优点)
- [MyBatis框架的缺点：](#mybatis框架的缺点)
- [MyBatis框架适用场合：](#mybatis框架适用场合)
- [MyBatis与Hibernate有哪些不同？](#mybatis与hibernate有哪些不同)
- [Mybatis 比 IBatis 比较大的几个改进是什么？](#mybatis-比-ibatis-比较大的几个改进是什么)
- [ORM是什么](#orm是什么)
- [传统JDBC开发存在的问题](#传统jdbc开发存在的问题)
- [为什么说Mybatis是半自动ORM映射工具？它与全自动的区别在哪里？](#为什么说mybatis是半自动orm映射工具它与全自动的区别在哪里)
- [传统JDBC开发存在什么问题？](#传统jdbc开发存在什么问题)
- [JDBC编程有哪些不足之处，MyBatis是如何解决的？](#jdbc编程有哪些不足之处mybatis是如何解决的)
- [JDBC编程有哪些不足之处，MyBatis 是如何解决这些问题的？](#jdbc编程有哪些不足之处mybatis-是如何解决这些问题的)
- [MyBatis编程步骤是什么样的？](#mybatis编程步骤是什么样的)
- [请说说MyBatis的工作原理](#请说说mybatis的工作原理)
- [MyBatis的功能架构是怎样的](#mybatis的功能架构是怎样的)
- [MyBatis的框架架构设计是怎么样的](#mybatis的框架架构设计是怎么样的)
- [什么是DBMS](#什么是dbms)
- [为什么需要预编译](#为什么需要预编译)
- [#{}和${}的区别是什么？](#和的区别是什么)
- [当实体类中的属性名和表中的字段名不一样 ，怎么办 ？](#当实体类中的属性名和表中的字段名不一样-怎么办-)
- [模糊查询like语句该怎么写?](#模糊查询like语句该怎么写)
- [Mybatis都有哪些Executor执行器？它们之间的区别是什么？](#mybatis都有哪些executor执行器它们之间的区别是什么)
- [Mybatis中如何指定使用哪一种Executor执行器？](#mybatis中如何指定使用哪一种executor执行器)
- [通常一个Xml映射文件，都会写一个Dao接口与之对应，请问，这个Dao接口的工作原理是什么？Dao接口里的方法，参数不同时，方法能重载吗？](#通常一个xml映射文件都会写一个dao接口与之对应请问这个dao接口的工作原理是什么dao接口里的方法参数不同时方法能重载吗)
- [Mybatis是如何进行分页的？分页插件的原理是什么？](#mybatis是如何进行分页的分页插件的原理是什么)
- [Mybatis是如何将sql执行结果封装为目标对象并返回的？都有哪些映射形式？](#mybatis是如何将sql执行结果封装为目标对象并返回的都有哪些映射形式)
- [如何获取自动生成的(主)键值?](#如何获取自动生成的主键值)
- [在mapper中如何传递多个参数?](#在mapper中如何传递多个参数)
- [Mybatis是否支持延迟加载？如果支持，它的实现原理是什么？](#mybatis是否支持延迟加载如果支持它的实现原理是什么)
- [Mybatis动态sql有什么用？执行原理？有哪些动态sql？](#mybatis动态sql有什么用执行原理有哪些动态sql)
- [Xml映射文件中，除了常见的select|insert|updae|delete标签之外，还有哪些标签？](#xml映射文件中除了常见的selectinsertupdaedelete标签之外还有哪些标签)
- [Mybatis的Xml映射文件中，不同的Xml映射文件，id是否可以重复？](#mybatis的xml映射文件中不同的xml映射文件id是否可以重复)
- [为什么说Mybatis是半自动ORM映射工具？它与全自动的区别在哪里？](#为什么说mybatis是半自动orm映射工具它与全自动的区别在哪里)
- [一对一、一对多的关联查询 ？](#一对一一对多的关联查询-)
- [MyBatis 里面的动态 Sql 是怎么设定的?用什么语法?](#mybatis-里面的动态-sql-是怎么设定的用什么语法)
- [Mybatis 能执行一对一、一对多的关联查询吗？都有哪些实现方式，以及它们之间的区别？](#mybatis-能执行一对一一对多的关联查询吗都有哪些实现方式以及它们之间的区别)
- [MyBatis实现一对一有几种方式?具体怎么操作的？](#mybatis实现一对一有几种方式具体怎么操作的)
- [MyBatis实现一对多有几种方式,怎么操作的？](#mybatis实现一对多有几种方式怎么操作的)
- [Mybatis是否支持延迟加载？如果支持，它的实现原理是什么？](#mybatis是否支持延迟加载如果支持它的实现原理是什么)
- [Mybatis的一级、二级缓存:](#mybatis的一级二级缓存)
- [什么是MyBatis的接口绑定？有哪些实现方式？](#什么是mybatis的接口绑定有哪些实现方式)
- [接口绑定有几种实现方式,分别是怎么实现的?](#接口绑定有几种实现方式分别是怎么实现的)
- [什么情况下用注解绑定,什么情况下用 xml 绑定？](#什么情况下用注解绑定什么情况下用-xml-绑定)
- [使用MyBatis的mapper接口调用时有哪些要求？](#使用mybatis的mapper接口调用时有哪些要求)
- [Mybais 常用注解 ？](#mybais-常用注解-)
- [Mapper编写有哪几种方式？](#mapper编写有哪几种方式)
- [Mybatis 映射文件中，如果 A 标签通过 include 引用了 B 标签的内容，请问，B 标签能****否定义在 A 标签的后面，还是说必须定义在 A 标签的前面？](#mybatis-映射文件中如果-a-标签通过-include-引用了-b-标签的内容请问b-标签能否定义在-a-标签的后面还是说必须定义在-a-标签的前面)
- [简述Mybatis的插件运行原理，以及如何编写一个插件。](#简述mybatis的插件运行原理以及如何编写一个插件)
- [Mybatis 动态 sql 是做什么的？都有哪些动态 sql？能简述一下动态 sql 的执行原理不？](#mybatis-动态-sql-是做什么的都有哪些动态-sql能简述一下动态-sql-的执行原理不)
- [简述 Mybatis 的 Xml 映射文件和 Mybatis 内部数据结构之间的映射关系？](#简述-mybatis-的-xml-映射文件和-mybatis-内部数据结构之间的映射关系)

<!-- /TOC -->


### 什么是Mybatis？

**1、** Mybatis是一个半ORM（对象关系映射）框架，它内部封装了JDBC，开发时只需要关注SQL语句本身，不需要花费精力去处理加载驱动、创建连接、创建statement等繁杂的过程。程序员直接编写原生态sql，可以严格控制sql执行性能，灵活度高。

**2、** MyBatis 可以使用 XML 或注解来配置和映射原生信息，将 POJO映射成数据库中的记录，避免了几乎所有的 JDBC 代码和手动设置参数以及获取结果集。

**3、** 通过xml 文件或注解的方式将要执行的各种 statement 配置起来，并通过java对象和 statement中sql的动态参数进行映射生成最终执行的sql语句，最后由mybatis框架执行sql并将结果映射为java对象并返回。（从执行sql到返回result的过程）。



### Mybaits的优点：

**1、** 基于SQL语句编程，相当灵活，不会对应用程序或者数据库的现有设计造成任何影响，SQL写在XML里，解除sql与程序代码的耦合，便于统一管理；提供XML标签，支持编写动态SQL语句，并可重用。

**2、 **与JDBC相比，减少了50%以上的代码量，消除了JDBC大量冗余的代码，不需要手动开关连接；

**3、 **很好的与各种数据库兼容（因为MyBatis使用JDBC来连接数据库，所以只要JDBC支持的数据库MyBatis都支持）。

**4、** 能够与Spring很好的集成；

**5、 ** 提供映射标签，支持对象与数据库的ORM字段关系映射；提供对象关系映射标签，支持对象关系组件维护。



### MyBatis框架的缺点：

**1、 ** SQL语句的编写工作量较大，尤其当字段多、关联表多时，对开发人员编写SQL语句的功底有一定要求。

**2、 ** SQL语句依赖于数据库，导致数据库移植性差，不能随意更换数据库。



### MyBatis框架适用场合：

**1、** MyBatis专注于SQL本身，是一个足够灵活的DAO层解决方案。

**2、** 对性能的要求很高，或者需求变化较多的项目，如互联网项目，MyBatis将是不错的选择。



### MyBatis与Hibernate有哪些不同？

**相同点**

- 都是对jdbc的封装，都是持久层的框架，都用于dao层的开发。

**不同点**

- 映射关系
  - MyBatis 是一个半自动映射的框架，配置Java对象与sql语句执行结果的对应关系，多表关联关系配置简单
  - Hibernate 是一个全表映射的框架，配置Java对象与数据库表的对应关系，多表关联关系配置复杂

**SQL优化和移植性**

- Hibernate 对SQL语句封装，提供了日志、缓存、级联（级联比 MyBatis 强大）等特性，此外还提供 HQL（Hibernate Query Language）操作数据库，数据库无关性支持好，但会多消耗性能。如果项目需要支持多种数据库，代码开发量少，但SQL语句优化困难。
- MyBatis 需要手动编写 SQL，支持动态 SQL、处理列表、动态生成表名、支持存储过程。开发工作量相对大些。直接使用SQL语句操作数据库，不支持数据库无关性，但sql语句优化容易。



### Mybatis 比 IBatis 比较大的几个改进是什么？

**1、** 有接口绑定,包括注解绑定 sql 和 xml 绑定 Sql

**2、** 动态 sql 由原来的节点配置变成 OGNL 表达式 3） 在一对一,一对多的时候引进了association,在一对多的时候引入了 collection 节点,不过都是在 resultMap 里面配置



### ORM是什么

ORM（Object Relational Mapping），对象关系映射，是一种为了解决关系型数据库数据与简单Java对象（POJO）的映射关系的技术。简单的说，ORM是通过使用描述对象和数据库之间映射的元数据，将程序中的对象自动持久化到关系型数据库中。



### 传统JDBC开发存在的问题

**1、** 频繁创建数据库连接对象,释放造成系统浪费,影响性能. 使用连接池解决这问题但是需要自己实现连接池

**2、 **sql语句,参数设置,结果集处理存在硬编码,代码不易维护,sql变动需要修改java代码

**3、** 使用perparedStatement 向占有位符号传参存在硬编码,

**4、** 结果集处理存在重复代码,处理麻烦



### 为什么说Mybatis是半自动ORM映射工具？它与全自动的区别在哪里？

- Hibernate属于全自动ORM映射工具，使用Hibernate查询关联对象或者关联集合对象时，可以根据对象关系模型直接获取，所以它是全自动的。
- 而Mybatis在查询关联对象或关联集合对象时，需要手动编写sql来完成，所以，称之为半自动ORM映射工具。



### 传统JDBC开发存在什么问题？

- 频繁创建数据库连接对象、释放，容易造成系统资源浪费，影响系统性能。可以使用连接池解决这个问题。但是使用jdbc需要自己实现连接池。
- sql语句定义、参数设置、结果集处理存在硬编码。实际项目中sql语句变化的可能性较大，一旦发生变化，需要修改java代码，系统需要重新编译，重新发布。不好维护。
- 使用preparedStatement向占有位符号传参数存在硬编码，因为sql语句的where条件不一定，可能多也可能少，修改sql还要修改代码，系统不易维护。
- 结果集处理存在重复代码，处理麻烦。如果可以映射成Java对象会比较方便。



### JDBC编程有哪些不足之处，MyBatis是如何解决的？

**1、**数据库链接创建、释放频繁造成系统资源浪费从而影响系统性能，如果使用数据库连接池可解决此问题。

- 解决：在mybatis-config.xml中配置数据链接池，使用连接池管理数据库连接。

**2、**Sql语句写在代码中造成代码不易维护，实际应用sql变化的可能较大，sql变动需要改变java代码。-

- 解决：将Sql语句配置在XXXXmapper.xml文件中与java代码分离。

**3、**向sql语句传参数麻烦，因为sql语句的where条件不一定，可能多也可能少，占位符需要和参数一一对应。

- 解决： Mybatis自动将java对象映射至sql语句。

**4、**对结果集解析麻烦，sql变化导致解析代码变化，且解析前需要遍历，如果能将数据库记录封装成pojo对象解析比较方便。

- 解决：Mybatis自动将sql执行结果映射至java对象。



### JDBC编程有哪些不足之处，MyBatis 是如何解决这些问题的？

mybatis-config.xml中配置数据库连接池,使用连接池管理数据可连接,解决频繁创建数据库连接对象

mapper.xml中编写sql语句与java代码分离

mybatis自动将java对象映射到sql语句

mybatis自动将结果集映射大java对象



### MyBatis编程步骤是什么样的？

**1、** 创建SqlSessionFactory

**2、** 通过SqlSessionFactory创建SqlSession

**3、** 通过sqlsession执行数据库操作

**4、** 调用session.commit()提交事务

**5、** 调用session.close()关闭会话



### 请说说MyBatis的工作原理

 ![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330012029.png)

**1、** 读取 MyBatis 配置文件：mybatis-config.xml 为 MyBatis 的全局配置文件，配置了 MyBatis 的运行环境等信息，例如数据库连接信息。

**2、** 加载映射文件。映射文件即 SQL 映射文件，该文件中配置了操作数据库的 SQL 语句，需要在 MyBatis 配置文件 mybatis-config.xml 中加载。mybatis-config.xml 文件可以加载多个映射文件，每个文件对应数据库中的一张表。

**3、** 构造会话工厂：通过 MyBatis 的环境等配置信息构建会话工厂 SqlSessionFactory。

**4、** 创建会话对象：由会话工厂创建 SqlSession 对象，该对象中包含了执行 SQL 语句的所有方法。

**5、** Executor 执行器：MyBatis 底层定义了一个 Executor 接口来操作数据库，它将根据 SqlSession 传递的参数动态地生成需要执行的 SQL 语句，同时负责查询缓存的维护。

**6、** MappedStatement 对象：在 Executor 接口的执行方法中有一个 MappedStatement 类型的参数，该参数是对映射信息的封装，用于存储要映射的 SQL 语句的 id、参数等信息。

**7、** 输入参数映射：输入参数类型可以是 Map、List 等集合类型，也可以是基本数据类型和 POJO 类型。输入参数映射过程类似于 JDBC 对 preparedStatement 对象设置参数的过程。

**8、** 输出结果映射：输出结果类型可以是 Map、 List 等集合类型，也可以是基本数据类型和 POJO 类型。输出结果映射过程类似于 JDBC 对结果集的解析过程。



### MyBatis的功能架构是怎样的

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330012053.png)

我们把Mybatis的功能架构分为三层：

- API接口层：提供给外部使用的接口API，开发人员通过这些本地API来操纵数据库。接口层一接收到调用请求就会调用数据处理层来完成具体的数据处理。
- 数据处理层：负责具体的SQL查找、SQL解析、SQL执行和执行结果映射处理等。它主要的目的是根据调用的请求完成一次数据库操作。
- 基础支撑层：负责最基础的功能支撑，包括连接管理、事务管理、配置加载和缓存处理，这些都是共用的东西，将他们抽取出来作为最基础的组件。为上层的数据处理层提供最基础的支撑。



### MyBatis的框架架构设计是怎么样的

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210330012119.png)

这张图从上往下看。MyBatis的初始化，会从mybatis-config.xml配置文件，解析构造成Configuration这个类，就是图中的红框。

**1、加载配置：**配置来源于两个地方，一处是配置文件，一处是Java代码的注解，将SQL的配置信息加载成为一个个MappedStatement对象（包括了传入参数映射配置、执行的SQL语句、结果映射配置），存储在内存中。

**2、SQL解析：**当API接口层接收到调用请求时，会接收到传入SQL的ID和传入对象（可以是Map、JavaBean或者基本数据类型），Mybatis会根据SQL的ID找到对应的MappedStatement，然后根据传入参数对象对MappedStatement进行解析，解析后可以得到最终要执行的SQL语句和参数。

**3、SQL执行：**将最终得到的SQL和参数拿到数据库进行执行，得到操作数据库的结果。

**4、结果映射：**将操作数据库的结果按照映射的配置进行转换，可以转换成HashMap、JavaBean或者基本数据类型，并将最终结果返回。



### 什么是DBMS

数据库管理系统(database management system)是一种操纵和管理数据库的大型软件，用于建立、使用和维护数zd据库，简称dbms。它对数据库进行统一的管理和控制，以保证数据库的安全性和完整性。用户通过dbms访问数据库中的数据，数据库管理员也通过dbms进行数据库的维护工作。它可使多个应用程序和用户用不同的方法在同时版或不同时刻去建立，修改和询问数据库。DBMS提供数据定义语言DDL（Data Definition Language）与数据操作语言DML（Data Manipulation Language），供用户定义数据库的模式结构与权限约束，实现对数据的追加权、删除等操作。



### 为什么需要预编译

**定义：**

- SQL 预编译指的是数据库驱动在发送 SQL 语句和参数给 DBMS 之前对 SQL 语句进行编译，这样 DBMS 执行 SQL 时，就不需要重新编译。

**为什么需要预编译**

- JDBC 中使用对象 PreparedStatement 来抽象预编译语句，使用预编译。预编译阶段可以优化 SQL 的执行。预编译之后的 SQL 多数情况下可以直接执行，DBMS 不需要再次编译，越复杂的SQL，编译的复杂度将越大，预编译阶段可以合并多次操作为一个操作。同时预编译语句对象可以重复利用。把一个 SQL 预编译后产生的 PreparedStatement 对象缓存下来，下次对于同一个SQL，可以直接使用这个缓存的 PreparedState 对象。Mybatis默认情况下，将对所有的 SQL 进行预编译。
- 还有一个重要的原因，复制SQL注入



### #{}和${}的区别是什么？

- `#{}`是预编译处理

- `${}`是字符串替换。

Mybatis在处理#{}时，会将sql中的#{}替换为?号，调用PreparedStatement的set方法来赋值；

Mybatis在处理${}时，就是把${}替换成变量的值。

使用#{}可以有效的防止SQL注入，提高系统安全性。



### 当实体类中的属性名和表中的字段名不一样 ，怎么办 ？

**第1种：** 通过在查询的sql语句中定义字段名的别名，让字段名的别名和实体类的属性名一致。

```
<select id=”selectorder” parametertype=”int” resultetype=”me.gacl.domain.order”>       
	select order_id id, order_no orderno ,order_price price form orders where order_id=#{id};
</select>
```



**第2种：** 通过 `<resultMap>`来映射字段名和实体类属性名的一一对应的关系。

```
<select id="getOrder" parameterType="int" resultMap="orderresultmap">select * from orders where order_id=#{id}</select>
<resultMap type=”me.gacl.domain.order” id=”orderresultmap”>    <!–用id属性来映射主键字段–>    <id property=”id” column=”order_id”>
    <!–用result属性来映射非主键字段，property为实体类属性名，column为数据表中的属性–>    <result property = “orderno” column =”order_no”/>    <result property=”price” column=”order_price” /></reslutMap>
```



### 模糊查询like语句该怎么写?

**第1种：** 在Java代码中添加sql通配符。

```xml
string wildcardname = “%smi%”;
list<name> names = mapper.selectlike(wildcardname);

<select id=”selectlike”>
select * from foo where bar like #{value}
</select>
```



**第2种：** 在sql语句中拼接通配符，会引起sql注入

```xml
string wildcardname = “smi”;
list<name> names = mapper.selectlike(wildcardname);

<select id=”selectlike”>
	select * from foo where bar like "%"#{value}"%"
</select>
```



### Mybatis都有哪些Executor执行器？它们之间的区别是什么？

- Mybatis有三种基本的Executor执行器，SimpleExecutor、ReuseExecutor、BatchExecutor。
- **SimpleExecutor** ：每执行一次update或select，就开启一个Statement对象，用完立刻关闭Statement对象。
- **ReuseExecutor** ：执行update或select，以sql作为key查找Statement对象，存在就使用，不存在就创建，用完后，不关闭Statement对象，而是放置于Map<String, Statement>内，供下一次使用。简言之，就是重复使用Statement对象。
- **BatchExecutor** ：执行update（没有select，JDBC批处理不支持select），将所有sql都添加到批处理中（addBatch()），等待统一执行（executeBatch()），它缓存了多个Statement对象，每个Statement对象都是addBatch()完毕后，等待逐一执行executeBatch()批处理。与JDBC批处理相同。

```
作用范围：Executor的这些特点，都严格限制在SqlSession生命周期范围内。
```



### Mybatis中如何指定使用哪一种Executor执行器？

- 在Mybatis配置文件中，在设置（settings）可以指定默认的ExecutorType执行器类型，也可以手动给DefaultSqlSessionFactory的创建SqlSession的方法传递ExecutorType类型参数，如SqlSession openSession(ExecutorType execType)。
- 配置默认的执行器。SIMPLE 就是普通的执行器；REUSE 执行器会重用预处理语句（prepared statements）； BATCH 执行器将重用语句并执行批量更新。







### 通常一个Xml映射文件，都会写一个Dao接口与之对应，请问，这个Dao接口的工作原理是什么？Dao接口里的方法，参数不同时，方法能重载吗？

Dao 接口，就是人们常说的 `Mapper`接口，接口的全限名，就是映射文件中的 namespace 的值，接口的方法名，就是映射文件中`MappedStatement`的 id 值，接口方法内的参数，就是传递给 sql 的参数。`Mapper`接口是没有实现类的，当调用接口方法时，接口全限名+方法名拼接字符串作为 key 值，可唯一定位一个`MappedStatement`，举例：`com.mybatis3.mappers.StudentDao.findStudentById`，可以唯一找到 namespace 为`com.mybatis3.mappers.StudentDao`下面`id = findStudentById`的`MappedStatement`。在 MyBatis 中，每一个`<select>`、`<insert>`、`<update>`、`<delete>`标签，都会被解析为一个`MappedStatement`对象。

Dao 接口里的方法可以重载，但是Mybatis的XML里面的ID不允许重复。

Mybatis版本3.3.0，亲测如下：

```java
/**
 * Mapper接口里面方法重载
 */
public interface StuMapper {

    List<Student> getAllStu();
    
    List<Student> getAllStu(@Param("id") Integer id);
}
```

然后在 `StuMapper.xml` 中利用Mybatis的动态sql就可以实现。

```java
<select id="getAllStu" resultType="com.pojo.Student">
         select * from student
        <where>
            <if test="id != null">
                id = #{id}
            </if>
        </where>
     </select>
```

能正常运行，并能得到相应的结果，这样就实现了在Dao接口中写重载方法。

**Mybatis 的 Dao 接口可以有多个重载方法，但是多个接口对应的映射必须只有一个，否则启动会报错。**



### Mybatis是如何进行分页的？分页插件的原理是什么？

**1、** Mybatis 使用 RowBounds 对象进行分页，也可以直接编写 sql 实现分页，也可以使用

Mybatis 的分页插件。

**2、** 分页插件的原理：实现 Mybatis 提供的接口，实现自定义插件，在插件的拦截方法内拦

截待执行的 sql，然后重写 sql。

举例：

```sql
select * from student，拦截 sql 后重写为：select t.* from （select * from student）t

limit 0，10
```





### Mybatis是如何将sql执行结果封装为目标对象并返回的？都有哪些映射形式？

**第一种** 是使用 `<resultMap>`标签，逐一定义数据库列名和对象属性名之间的映射关系。



**第二种** 是使用sql列的别名功能，将列的别名书写为对象属性名。

有了列名与属性名的映射关系后，Mybatis通过反射创建对象，同时使用反射给对象的属性逐一赋值并返回，那些找不到映射关系的属性，是无法完成赋值的。



### 如何获取自动生成的(主)键值?

insert 方法总是返回一个int值 ，这个值代表的是插入的行数。

如果采用自增长策略，自动生成的键值在 insert 方法执行完后可以被设置到传入的参数对象中。

示例：

```
<insert id=”insertname” usegeneratedkeys=”true” keyproperty=”id”>
     insert into names (name) values (#{name})
</insert>
```

```java
    name name = new name();
    name.setname(“fred”);
 
    int rows = mapper.insertname(name);
    // 完成后,id已经被设置到对象中
    system.out.println(“rows inserted = ” + rows);
    system.out.println(“generated key value = ” + name.getid());
```





### 在mapper中如何传递多个参数?

**方法1：顺序传参法**

```
public User selectUser(String name, int deptId);

<select id="selectUser" resultMap="UserResultMap">
    select * from user
    where user_name = #{0} and dept_id = #{1}
</select>

```

- \#{}里面的数字代表传入参数的顺序。
- 这种方法不建议使用，sql层表达不直观，且一旦顺序调整容易出错。



**方法2：@Param注解传参法**

```
public User selectUser(@Param("userName") String name, int @Param("deptId") deptId);

<select id="selectUser" resultMap="UserResultMap">
    select * from user
    where user_name = #{userName} and dept_id = #{deptId}
</select>

```

- \#{}里面的名称对应的是注解@Param括号里面修饰的名称。
- 这种方法在参数不多的情况还是比较直观的，（推荐使用）。



**方法3：Map传参法**

```
public User selectUser(Map<String, Object> params);

<select id="selectUser" parameterType="java.util.Map" resultMap="UserResultMap">
    select * from user
    where user_name = #{userName} and dept_id = #{deptId}
</select>

```

- \#{}里面的名称对应的是Map里面的key名称。
- 这种方法适合传递多个参数，且参数易变能灵活传递的情况。（推荐使用）。



**方法4：Java Bean传参法**

```
public User selectUser(User user);

<select id="selectUser" parameterType="com.jourwon.pojo.User" resultMap="UserResultMap">
    select * from user
    where user_name = #{userName} and dept_id = #{deptId}
</select>

```

- \#{}里面的名称对应的是User类里面的成员属性。
- 这种方法直观，需要建一个实体类，扩展不容易，需要加属性，但代码可读性强，业务逻辑处理方便，推荐使用。（推荐使用）。



### Mybatis是否支持延迟加载？如果支持，它的实现原理是什么？

- Mybatis仅支持association关联对象和collection关联集合对象的延迟加载，association指的就是一对一，collection指的就是一对多查询。在Mybatis配置文件中，可以配置是否启用延迟加载lazyLoadingEnabled=true|false。
- 它的原理是，使用CGLIB创建目标对象的代理对象，当调用目标方法时，进入拦截器方法，比如调用a.getB().getName()，拦截器invoke()方法发现a.getB()是null值，那么就会单独发送事先保存好的查询关联B对象的sql，把B查询上来，然后调用a.setB(b)，于是a的对象b属性就有值了，接着完成a.getB().getName()方法的调用。这就是延迟加载的基本原理。
- 当然了，不光是Mybatis，几乎所有的包括Hibernate，支持延迟加载的原理都是一样的。



### Mybatis动态sql有什么用？执行原理？有哪些动态sql？

Mybatis动态sql可以在Xml映射文件内，以标签的形式编写动态sql，执行原理是根据表达式的值 完成逻辑判断并动态拼接sql的功能。

Mybatis提供了9种动态sql标签： `trim|where|set|foreach|if|choose|when|otherwise|bind`。

其执行原理为，使用 OGNL 从 sql 参数对象中计算表达式的值，根据表达式的值动态拼接 sql，以此来完成动态 sql 的功能。



### Xml映射文件中，除了常见的select|insert|updae|delete标签之外，还有哪些标签？

还有很多其他的标签，<resultMap>、<parameterMap>、<sql>、<include>、<selectKey>，加上动态 sql 的 9 个标签，

trim|where|set|foreach|if|choose|when|otherwise|bind 等，其中<sql>为 sql 片段标签，通过<include>标签引入 sql 片段，<selectKey>为不支持自增的主键生成策略标签。



### Mybatis的Xml映射文件中，不同的Xml映射文件，id是否可以重复？

不同的Xml映射文件，如果配置了namespace，那么id可以重复；如果没有配置namespace，那么id不能重复；

原因就是namespace+id是作为Map `<String,MapperStatement>`的key使用的，如果没有namespace，就剩下id，那么，id重复会导致数据互相覆盖。有了namespace，自然id就可以重复，namespace不同，namespace+id自然也就不同。



### 为什么说Mybatis是半自动ORM映射工具？它与全自动的区别在哪里？

Hibernate属于全自动ORM映射工具，使用Hibernate查询关联对象或者关联集合对象时，可以根据对象关系模型直接获取，所以它是全自动的。而Mybatis在查询关联对象或关联集合对象时，需要手动编写sql来完成，所以，称之为半自动ORM映射工具。



### 一对一、一对多的关联查询 ？

```
<mapper namespace="com.lcb.mapping.userMapper">  
    <!--association  一对一关联查询 -->  
    <select id="getClass" parameterType="int" resultMap="ClassesResultMap">  
        select * from class c,teacher t where c.teacher_id=t.t_id and c.c_id=#{id}  
    </select>  
 
    <resultMap type="com.lcb.user.Classes" id="ClassesResultMap">  
        <!-- 实体类的字段名和数据表的字段名映射 -->  
        <id property="id" column="c_id"/>  
        <result property="name" column="c_name"/>  
        <association property="teacher" javaType="com.lcb.user.Teacher">  
            <id property="id" column="t_id"/>  
            <result property="name" column="t_name"/>  
        </association>  
    </resultMap>  
 
 
    <!--collection  一对多关联查询 -->  
    <select id="getClass2" parameterType="int" resultMap="ClassesResultMap2">  
        select * from class c,teacher t,student s where c.teacher_id=t.t_id and c.c_id=s.class_id and c.c_id=#{id}  
    </select>  
 
    <resultMap type="com.lcb.user.Classes" id="ClassesResultMap2">  
        <id property="id" column="c_id"/>  
        <result property="name" column="c_name"/>  
        <association property="teacher" javaType="com.lcb.user.Teacher">  
            <id property="id" column="t_id"/>  
            <result property="name" column="t_name"/>  
        </association>  
 
        <collection property="student" ofType="com.lcb.user.Student">  
            <id property="id" column="s_id"/>  
            <result property="name" column="s_name"/>  
        </collection>  
    </resultMap>  
</mapper> 
```



### MyBatis 里面的动态 Sql 是怎么设定的?用什么语法?

MyBatis 里面的动态 Sql 一般是通过 if 节点来实现,通过 OGNL 语法来实现,但是如果要写的完整,必须配合 where,trim 节点,where 节点是判断包含节点有内容就插入 where,否则不插入,trim 节点是用来判断如果动态语句是以 and 或 or 开始,那么会自动把这个 and 或者 or取掉。



### Mybatis 能执行一对一、一对多的关联查询吗？都有哪些实现方式，以及它们之间的区别？

能，Mybatis 不仅可以执行一对一、一对多的关联查询，还可以执行多对一，多对多的关联查询，多对一查询，其实就是一对一查询，只需要把 selectOne()修改为 selectList()即可；

多对多查询，其实就是一对多查询，只需要把 selectOne()修改为 selectList()即可。关联对象查询，有两种实现方式，一种是单独发送一个 sql 去查询关联对象，赋给主对象，然后返回主对象。另一种是使用嵌套查询，嵌套查询的含义为使用 join 查询，一部分列是 A 对象的属性值，另外一部分列是关联对象 B 的属性值，好处是只发一个 sql 查询，就可以把主对象和其关联对象查出来。



### MyBatis实现一对一有几种方式?具体怎么操作的？

有联合查询和嵌套查询,联合查询是几个表联合查询,只查询一次, 通过在resultMap里面配置association节点配置一对一的类就可以完成；

嵌套查询是先查一个表，根据这个表里面的结果的 外键id，去再另外一个表里面查询数据,也是通过association配置，但另外一个表的查询通过select属性配置。



### MyBatis实现一对多有几种方式,怎么操作的？

有联合查询和嵌套查询。联合查询是几个表联合查询,只查询一次,通过在resultMap里面的collection节点配置一对多的类就可以完成；嵌套查询是先查一个表,根据这个表里面的 结果的外键id,去再另外一个表里面查询数据,也是通过配置collection,但另外一个表的查询通过select节点配置。



### Mybatis是否支持延迟加载？如果支持，它的实现原理是什么？

Mybatis仅支持association关联对象和collection关联集合对象的延迟加载，association指的就是一对一，collection指的就是一对多查询。在Mybatis配置文件中，可以配置是否启用延迟加载lazyLoadingEnabled=true|false。

它的原理是，使用CGLIB创建目标对象的代理对象，当调用目标方法时，进入拦截器方法，比如调用a.getB().getName()，拦截器invoke()方法发现a.getB()是null值，那么就会单独发送事先保存好的查询关联B对象的sql，把B查询上来，然后调用a.setB(b)，于是a的对象b属性就有值了，接着完成a.getB().getName()方法的调用。这就是延迟加载的基本原理。

当然了，不光是Mybatis，几乎所有的包括Hibernate，支持延迟加载的原理都是一样的。



### Mybatis的一级、二级缓存:

1）一级缓存: 基于 PerpetualCache 的 HashMap 本地缓存，其存储作用域为 Session，当 Session flush 或 close 之后，该 Session 中的所有 Cache 就将清空，默认打开一级缓存。

2）二级缓存与一级缓存其机制相同，默认也是采用 PerpetualCache，HashMap 存储，不同在于其存储作用域为 Mapper(Namespace)，并且可自定义存储源，如 Ehcache。默认不打开二级缓存，要开启二级缓存，使用二级缓存属性类需要实现Serializable序列化接口(可用来保存对象的状态),可在它的映射文件中配置 `<cache/>` ；

3）对于缓存数据更新机制，当某一个作用域(一级缓存 Session/二级缓存Namespaces)的进行了C/U/D 操作后，默认该作用域下所有 select 中的缓存将被 clear。



### 什么是MyBatis的接口绑定？有哪些实现方式？

接口绑定，就是在MyBatis中任意定义接口,然后把接口里面的方法和SQL语句绑定, 我们直接调用接口方法就可以,这样比起原来了SqlSession提供的方法我们可以有更加灵活的选择和设置。

接口绑定有两种实现方式,一种是通过注解绑定，就是在接口的方法上面加上 @Select、@Update等注解，里面包含Sql语句来绑定；另外一种就是通过xml里面写SQL来绑定, 在这种情况下,要指定xml映射文件里面的namespace必须为接口的全路径名。当Sql语句比较简单时候,用注解绑定, 当SQL语句比较复杂时候,用xml绑定,一般用xml绑定的比较多。



### 接口绑定有几种实现方式,分别是怎么实现的?

接口绑定有两种实现方式,一种是通过注解绑定,就是在接口的方法上面加上@Select@Update 等注解里面包含 Sql 语句来绑定,另外一种就是通过 xml 里面写 SQL 来绑定,在这种情况下,要指定 xml 映射文件里面的 namespace 必须为接口的全路径名.



### 什么情况下用注解绑定,什么情况下用 xml 绑定？

当 Sql 语句比较简单时候,用注解绑定；当 SQL 语句比较复杂时候,用 xml 绑定,一般用

xml 绑定的比较多



### 使用MyBatis的mapper接口调用时有哪些要求？

**1、** Mapper接口方法名和mapper.xml中定义的每个sql的id相同； 

**2、 **Mapper接口方法的输入参数类型和mapper.xml中定义的每个sql 的parameterType的类型相同； 

**3、** Mapper接口方法的输出参数类型和mapper.xml中定义的每个sql的resultType的类型相同； 

**4、** Mapper.xml文件中的namespace即是mapper接口的类路径。



### Mybais 常用注解 ？

**@Insert ：** 插入sql , 和xml insert sql语法完全一样

**@Select ：** 查询sql, 和xml select sql语法完全一样

**@Update ：** 更新sql, 和xml update sql语法完全一样

**@Delete ：** 删除sql, 和xml delete sql语法完全一样

**@Param：** 入参

**@Results：**结果集合

**@Result：** 结果



### Mapper编写有哪几种方式？

**第一种：接口实现类继承SqlSessionDaoSupport：使用此种方法需要编写mapper接口，mapper接口实现类、mapper.xml文件。**

```
（1）在sqlMapConfig.xml中配置mapper.xml的位置
<mappers>
    <mapper resource="mapper.xml文件的地址" />
    <mapper resource="mapper.xml文件的地址" />
</mappers>
（2）定义mapper接口
（3）实现类集成SqlSessionDaoSupport
mapper方法中可以this.getSqlSession()进行数据增删改查。
（4）spring 配置
<bean id=" " class="mapper接口的实现">
    <property name="sqlSessionFactory" ref="sqlSessionFactory"></property>
</bean> 

```



 **第二种：使用org.mybatis.spring.mapper.MapperFactoryBean：**

```
（1）在sqlMapConfig.xml中配置mapper.xml的位置，如果mapper.xml和mappre接口的名称相同且在同一个目录，这里可以不用配置
<mappers>
    <mapper resource="mapper.xml文件的地址" />
    <mapper resource="mapper.xml文件的地址" />
</mappers>
（2）定义mapper接口：
①mapper.xml中的namespace为mapper接口的地址
②mapper接口中的方法名和mapper.xml中的定义的statement的id保持一致
③Spring中定义
<bean id="" class="org.mybatis.spring.mapper.MapperFactoryBean">
    <property name="mapperInterface"   value="mapper接口地址" /> 
    <property name="sqlSessionFactory" ref="sqlSessionFactory" /> 
</bean>

```



**第三种：使用mapper扫描器：**

```
（1）mapper.xml文件编写：
mapper.xml中的namespace为mapper接口的地址；
mapper接口中的方法名和mapper.xml中的定义的statement的id保持一致；
如果将mapper.xml和mapper接口的名称保持一致则不用在sqlMapConfig.xml中进行配置。 
（2）定义mapper接口：
注意mapper.xml的文件名和mapper的接口名称保持一致，且放在同一个目录
（3）配置mapper扫描器：
<bean class="org.mybatis.spring.mapper.MapperScannerConfigurer">
    <property name="basePackage" value="mapper接口包地址"></property>
    <property name="sqlSessionFactoryBeanName" value="sqlSessionFactory"/> 
</bean>
（4）使用扫描器后从spring容器中获取mapper的实现对象。

```



### Mybatis 映射文件中，如果 A 标签通过 include 引用了 B 标签的内容，请问，B 标签能****否定义在 A 标签的后面，还是说必须定义在 A 标签的前面？

虽然 Mybatis 解析 Xml 映射文件是按照顺序解析的，但是，被引用的 B 标签依然可以定义在任何地方，Mybatis 都可以正确识别。原理是，Mybatis 解析 A 标签，发现 A 标签引用了 B 标签，但是 B 标签尚未解析到，尚不存在，此时，Mybatis 会将 A 标签标记为未解析状态，然后继续解析余下的标签，包含 B 标签，待所有标签解析完毕，Mybatis 会重新解析那些被标记为未解析的标签，此时再解析 A 标签时，B 标签已经存在，A 标签也就可以正常解析完成了。




### 简述Mybatis的插件运行原理，以及如何编写一个插件。

**1、**Mybatis 仅可以编写针对 ParameterHandler、ResultSetHandler、StatementHandler、

Executor 这 4 种接口的插件，Mybatis 通过动态代理，为需要拦截的接口生成代理对象以实

现接口方法拦截功能，每当执行这 4 种接口对象的方法时，就会进入拦截方法，具体就是

InvocationHandler 的 invoke()方法，当然，只会拦截那些你指定需要拦截的方法。

**2、**实现 Mybatis 的 Interceptor 接口并复写 intercept()方法，然后在给插件编写注解，指定

要拦截哪一个接口的哪些方法即可，记住，别忘了在配置文件中配置你编写的插件。



### Mybatis 动态 sql 是做什么的？都有哪些动态 sql？能简述一下动态 sql 的执行原理不？

**1、**Mybatis 动态 sql 可以让我们在 Xml 映射文件内，以标签的形式编写动态 sql，完成逻辑

判断和动态拼接 sql 的功能。

**2、**Mybatis 提供了 9 种动态 sql 标签：

trim|where|set|foreach|if|choose|when|otherwise|bind。

**3、**其执行原理为，使用 OGNL 从 sql 参数对象中计算表达式的值，根据表达式的值动态拼

接 sql，以此来完成动态 sql 的功能。



### 简述 Mybatis 的 Xml 映射文件和 Mybatis 内部数据结构之间的映射关系？

Mybatis 将所有 Xml 配置信息都封装到 All-In-One 重量级对象 Configuration 内部。在

Xml 映射文件中，<parameterMap> 标签会被解析为 ParameterMap 对象，其每个子元素会

被解析为 ParameterMapping 对象。<resultMap> 标签会被解析为 ResultMap 对象，其每个子

元素会被解析为 ResultMapping 对象。每一个<select>、<insert>、<update>、<delete>标签

均会被解析为 MappedStatement 对象，标签内的 sql 会被解析为 BoundSql 对象。


