**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

 - [什么是springboot ？](#什么是springboot-)
 - [Springboot 有哪些优点？](#springboot-有哪些优点)
 - [Spring Boot 的目录结构是怎样的？](#spring-boot-的目录结构是怎样的)
 - [Spring Boot 的核心注解是哪个？它主要由哪几个注解组成的？](#spring-boot-的核心注解是哪个它主要由哪几个注解组成的)
 - [怎么理解 Spring Boot 中 “约定优于配置“](#怎么理解-spring-boot-中-约定优于配置)
 - [如何在自定义端口上运行 Spring Boot应用程序?](#如何在自定义端口上运行-spring-boot应用程序)
 - [Spring Boot、Spring MVC 和 Spring 有什么区别？](#spring-bootspring-mvc-和-spring-有什么区别)
 - [Spring Boot初始化环境变量流程?](#spring-boot初始化环境变量流程)
 - [Spring Boot扫描流程?](#spring-boot扫描流程)
 - [Spring Boot 配置加载顺序详解](#spring-boot-配置加载顺序详解)
 - [Spring Boot 如何定义多套不同环境配置？](#spring-boot-如何定义多套不同环境配置)
 - [Spring Boot 有哪几种读取配置的方式？](#spring-boot-有哪几种读取配置的方式)
 - [SpringBoot 实现热部署有哪几种方式？](#springboot-实现热部署有哪几种方式)
 - [什么是 JavaConfig？](#什么是-javaconfig)
 - [Spring Boot 支持哪些日志框架？推荐和默认的日志框架是哪个](#spring-boot-支持哪些日志框架推荐和默认的日志框架是哪个)
 - [如何重新加载Spring Boot上的更改，而无需重新启动服务器？](#如何重新加载spring-boot上的更改而无需重新启动服务器)
 - [SpringBoot的原理](#springboot的原理)
 - [Spring Boot 自动配置原理是什么？](#spring-boot-自动配置原理是什么)
 - [你如何理解 Spring Boot 中的 Starters？](#你如何理解-spring-boot-中的-starters)
 - [spring-boot-starter-parent 有什么用 ?](#spring-boot-starter-parent-有什么用-)
 - [什么是 Spring Boot Stater ？](#什么是-spring-boot-stater-)
 - [SpringBoot常用的starter有哪些?](#springboot常用的starter有哪些)
 - [Spring Boot 的核心配置文件有哪几个？它们的区别是什么？](#spring-boot-的核心配置文件有哪几个它们的区别是什么)
 - [Spring Boot 的核心注解是哪个？它主要由哪几个注解组成的？](#spring-boot-的核心注解是哪个它主要由哪几个注解组成的)
 - [创建一个 Spring Boot Project 的最简单的方法是什么？](#创建一个-spring-boot-project-的最简单的方法是什么)
 - [Spring Initializr 是创建 Spring Boot Projects 的唯一方法吗？](#spring-initializr-是创建-spring-boot-projects-的唯一方法吗)
 - [如何集成 Spring Boot 和 ActiveMQ？](#如何集成-spring-boot-和-activemq)
 - [什么是 Swagger？你用 Spring Boot 实现了它吗？](#什么是-swagger你用-spring-boot-实现了它吗)
 - [运行 Spring Boot 有哪几种方式？](#运行-spring-boot-有哪几种方式)
 - [Spring Boot 打成的 jar 和普通的 jar 有什么区别 ?](#spring-boot-打成的-jar-和普通的-jar-有什么区别-)
 - [如何使用 Spring Boot 实现分页和排序？](#如何使用-spring-boot-实现分页和排序)
 - [Spring Boot 中如何实现定时任务 ?](#spring-boot-中如何实现定时任务-)
 - [Spring Boot 中的 starter 到底是什么](#spring-boot-中的-starter-到底是什么)
 - [spring-boot-starter-parent 有什么用](#spring-boot-starter-parent-有什么用)
 - [Spring Boot 打成的 jar 和普通的 jar 有什么区别](#spring-boot-打成的-jar-和普通的-jar-有什么区别)
 - [Spring Boot 还提供了其它的哪些 Starter Project Options？](#spring-boot-还提供了其它的哪些-starter-project-options)
 - [为什么我们需要 spring-boot-maven-plugin?](#为什么我们需要-spring-boot-maven-plugin)
 - [Springboot集成mybatis的过程](#springboot集成mybatis的过程)
 - [**什么是YAML？**](#什么是yaml)
 - [YAML 配置的优势在哪里 ?](#yaml-配置的优势在哪里-)
 - [Spring Boot 是否可以使用 XML 配置 ?](#spring-boot-是否可以使用-xml-配置-)
 - [spring boot 核心配置文件是什么？bootstrap.properties 和 application.properties 有何区别 ?](#spring-boot-核心配置文件是什么bootstrapproperties-和-applicationproperties-有何区别-)
 - [什么是 Spring Profiles？](#什么是-spring-profiles)
 - [什么是JavaConfig？](#什么是javaconfig)
 - [Spring Boot、Spring MVC 和 Spring 有什么区别？](#spring-bootspring-mvc-和-spring-有什么区别)
 - [springboot自动配置的原理](#springboot自动配置的原理)
 - [如何禁用一个特定自动配置类？](#如何禁用一个特定自动配置类)
 - [Spring Boot中的监视器是什么？](#spring-boot中的监视器是什么)
 - [什么是 Spring Batch?](#什么是-spring-batch)
 - [Spring Boot 中如何解决跨域问题 ?](#spring-boot-中如何解决跨域问题-)
 - [微服务中如何实现 session 共享](#微服务中如何实现-session-共享)
 - [什么是 CSRF 攻击？](#什么是-csrf-攻击)
 - [我们如何监视所有 Spring Boot 微服务？](#我们如何监视所有-spring-boot-微服务)
 - [什么是嵌入式服务器？我们为什么要使用嵌入式服务器呢?](#什么是嵌入式服务器我们为什么要使用嵌入式服务器呢)
 - [当 Spring Boot 应用程序作为 Java 应用程序运行时，后台会发生什么？](#当-spring-boot-应用程序作为-java-应用程序运行时后台会发生什么)
 - [RequestMapping 和 GetMapping 的不同之处在哪里？](#requestmapping-和-getmapping-的不同之处在哪里)
 - [什么是 Spring Data？](#什么是-spring-data)
 - [什么是 Spring Data REST?](#什么是-spring-data-rest)
 - [为什么我们不建议在实际的应用程序中使用 Spring Data Rest?](#为什么我们不建议在实际的应用程序中使用-spring-data-rest)
 - [比较一下 Spring Security 和 Shiro 各自的优缺点 ?](#比较一下-spring-security-和-shiro-各自的优缺点-)

<!-- /TOC -->

### 什么是springboot ？

用来简化spring应用的初始搭建以及开发过程 使用特定的方式来进行配置（properties或yml文件）

创建独立的spring引用程序 main方法运行 

嵌入的Tomcat 无需部署war文件 

简化maven配置 

自动配置spring添加对应功能starter自动化配置 

> spring boot来简化spring应用开发，约定大于配置，去繁从简，just run就能创建一个独立的，产品级别的应用



### Springboot 有哪些优点？

- 减少开发，测试时间和努力。
- 使用JavaConfig有助于避免使用XML。
- 避免大量的Maven导入和各种版本冲突。
- 提供意见发展方法。
- 通过提供默认值快速开始开发。
- 没有单独的Web服务器需要。这意味着你不再需要启动Tomcat，Glassfish或其他任何东西。
- 需要更少的配置 因为没有web.xml文件。只需添加用@ Configuration注释的类，然后添加用@Bean注释的方法，Spring将自动加载对象并像以前一样对其进行管理。您甚至可以将@Autowired添加到bean方法中，以使Spring自动装入需要的依赖关系中。
- 基于环境的配置 使用这些属性，您可以将您正在使用的环境传递到应用程序：-Dspring.profiles.active = {enviornment}。在加载主应用程序属性文件后，Spring将在（application{environment} .properties）中加载后续的应用程序属性文件。



### Spring Boot 的目录结构是怎样的？

```java

 +- javastack
     +- MyApplication.java
     |
     +- customer
     |   +- Customer.java
     |   +- CustomerController.java
     |   +- CustomerService.java
     |   +- CustomerRepository.java
     |
     +- order
         +- Order.java
         +- OrderController.java
         +- OrderService.java
         +- OrderRepository.java
```

这个目录结构是主流及推荐的做法，而在主入口类上加上 `@SpringBootApplication` 注解来开启 Spring Boot 的各项能力，如自动配置、组件扫描等。

```java
package cn.javastack.MyApplication;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class MyApplication {

    public static void main(String[] args) {
        SpringApplication.run(MyApplication.class, args);
    }

}
```

如果你不想这么做，你也可以充分利用 `@EnableAutoConfiguration` 和`@ComponentScan` 注解自定义你的行为，不过这不是推荐的做法。



### Spring Boot 的核心注解是哪个？它主要由哪几个注解组成的？

启动类上面的注解是@SpringBootApplication，它也是 Spring Boot 的核心注解，主要组合包含了以下 3 个注解：

**@SpringBootConfiguration：** 组合了 @Configuration 注解，实现配置文件的功能。

**@EnableAutoConfiguration：** 打开自动配置的功能，也可以关闭某个自动配置的选项，如关闭数据源自动配置功能：@SpringBootApplication(exclude = { DataSourceAutoConfiguration.class })。

**@ComponentScan： **Spring组件扫描。



### 怎么理解 Spring Boot 中 “约定优于配置“

Spring Boot Starter、Spring Boot Jpa 都是“约定优于配置“的一种体现。都是通过“约定优于配置“的设计思路来设计的，Spring Boot Starter 在启动的过程中会根据约定的信息对资源进行初始化；Spring Boot Jpa 通过约定的方式来自动生成 Sql ，避免大量无效代码编写。



### 如何在自定义端口上运行 Spring Boot应用程序?

在 `application.properties`中指定端口`serverport=8090`。



### Spring Boot、Spring MVC 和 Spring 有什么区别？

**1、Spring**

Spring最重要的特征是依赖注入。所有 SpringModules 不是依赖注入就是 IOC 控制反转。

当我们恰当的使用 DI 或者是 IOC 的时候，我们可以开发松耦合应用。松耦合应用的单元测试可以很容易的进行。

**2、Spring MVC**

Spring MVC 提供了一种分离式的方法来开发 Web 应用。通过运用像 DispatcherServelet，MoudlAndView 和 ViewResolver 等一些简单的概念，开发 Web 应用将会变的非常简单。

**3、SpringBoot**

Spring 和 SpringMVC 的问题在于需要配置大量的参数。

Spring Boot 通过一个自动配置和启动的项来目解决这个问题。为了更快的构建产品就绪应用程序，Spring Boot 提供了一些非功能性特征。



### Spring Boot初始化环境变量流程?

**1、** 调用`prepareEnvironment`方法去设置环境变量 

**2、** 接下来有三个方法`getOrCreateEnvironment`，`configureEnvironment`，`environmentPrepared` 

**3、** `getOrCreateEnvironment`去初始化系统环境变量 

**4、** `configureEnvironment`去初始化命令行参数 

**5、** `environmentPrepared`当广播到来的时候调用`onApplicationEnvironmentPreparedEvent`方法去使用`postProcessEnvironment`方法`load yml`和`properties变量`



### Spring Boot扫描流程?

**1、** 调用run方法中的`refreshContext`方法 

**2、** 用AbstractApplicationContext中的`refresh`方法 

**3、** 委托给`invokeBeanFactoryPostProcessors`去处理调用链 

**4、** 其中一个方法`postProcessBeanDefinitionRegistry会`去调用`processConfigBeanDefinitions`解析`beandefinitions` 

**5、** 在`processConfigBeanDefinitions`中有一个`parse`方法，其中有`componentScanParser.parse`的方法，这个方法会扫描当前路径下所有`Component`组件





### Spring Boot 配置加载顺序详解

使用 Spring Boot 会涉及到各种各样的配置，如开发、测试、线上就至少 3 套配置信息了。Spring Boot 可以轻松的帮助我们使用相同的代码就能使开发、测试、线上环境使用不同的配置。

**在 Spring Boot 里面，可以使用以下几种方式来加载配置。本章内容基于 Spring Boot 2.0 进行详解。**

1、properties文件；

2、YAML文件；

3、系统环境变量；

4、命令行参数；

等等……

**配置属性加载的顺序如下：**

```java
1、开发者工具 `Devtools` 全局配置参数；

2、单元测试上的 `@TestPropertySource` 注解指定的参数；

3、单元测试上的 `@SpringBootTest` 注解指定的参数；

4、命令行指定的参数，如 `java -jar springboot.jar --name="Java技术栈"`；

5、命令行中的 `SPRING_APPLICATION_JSONJSON` 指定参数, 如 `java -Dspring.application.json='{"name":"Java技术栈"}' -jar springboot.jar`

6、`ServletConfig` 初始化参数；

7、`ServletContext` 初始化参数；

8、JNDI参数（如 `java:comp/env/spring.application.json`）；

9、Java系统参数（来源：`System.getProperties()`）；

10、操作系统环境变量参数；

11、`RandomValuePropertySource` 随机数，仅匹配：`ramdom.*`；

12、JAR包外面的配置文件参数（`application-{profile}.properties（YAML）`）

13、JAR包里面的配置文件参数（`application-{profile}.properties（YAML）`）

14、JAR包外面的配置文件参数（`application.properties（YAML）`）

15、JAR包里面的配置文件参数（`application.properties（YAML）`）

16、`@Configuration`配置文件上 `@PropertySource` 注解加载的参数；

17、默认参数（通过 `SpringApplication.setDefaultProperties` 指定）；
```

**数字小的优先级越高，即数字小的会覆盖数字大的参数值**



### Spring Boot 如何定义多套不同环境配置？

提供多套配置文件，如：

```xml
applcation.properties

application-dev.properties

application-test.properties

application-prod.properties
```

然后在applcation.properties文件中指定当前的环境spring.profiles.active=test,这时候读取的就是application-test.properties文件。



### Spring Boot 有哪几种读取配置的方式？

Spring Boot 可以通过 

- @PropertySource
- @Value
- @Environment,
- @ConfigurationProperties 

来绑定变量



### SpringBoot 实现热部署有哪几种方式？

这可以使用 DEV 工具来实现。

通过这种依赖关系，您可以节省任何更改，嵌入式tomcat 将重新启动。

Spring Boot 有一个开发工具（DevTools）模块，它有助于提高开发人员的生产力。

Java 开发人员面临的一个主要挑战是将文件更改自动部署到服务器并自动重启服务器。开发人员可以重新加载 Spring Boot 上的更改，而无需重新启动服务器。这将消除每次手动部署更改的需要。Spring Boot 在发布它的第一个版本时没有这个功能。

这是开发人员最需要的功能。DevTools 模块完全满足开发人员的需求。该模块将在生产环境中被禁用。它还提供 H2 数据库控制台以更好地测试应用程序。



### 什么是 JavaConfig？

Spring JavaConfig 是 Spring 社区的产品，它提供了配置 Spring IoC 容器的纯Java 方法。因此它有助于避免使用 XML 配置。使用 JavaConfig 的优点在于：

**（1）面向对象的配置。** 由于配置被定义为 JavaConfig 中的类，因此用户可以充分利用 Java 中的面向对象功能。一个配置类可以继承另一个，重写它的@Bean 方法等。

**（2）减少或消除 XML 配置。** 基于依赖注入原则的外化配置的好处已被证明。但是，许多开发人员不希望在 XML 和 Java 之间来回切换。JavaConfig 为开发人员提供了一种纯 Java 方法来配置与 XML 配置概念相似的 Spring 容器。从技术角度来讲，只使用 JavaConfig 配置类来配置容器是可行的，但实际上很多人认为将JavaConfig 与 XML 混合匹配是理想的。

**（3）类型安全和重构友好。** JavaConfig 提供了一种类型安全的方法来配置 Spring容器。由于 Java 5.0 对泛型的支持，现在可以按类型而不是按名称检索 bean，不需要任何强制转换或基于字符串的查找。



### Spring Boot 支持哪些日志框架？推荐和默认的日志框架是哪个

Spring Boot 支持 Java Util Logging, Log4j2, Lockback 作为日志框架，如果你使用 Starters 启动器，Spring Boot 将使用 Logback 作为默认日志框架



### 如何重新加载Spring Boot上的更改，而无需重新启动服务器？

这可以使用DEV工具来实现。通过这种依赖关系，您可以节省任何更改，嵌入式tomcat将重新启动。 

Spring Boot有一个开发工具（DevTools）模块，它有助于提高开发人员的生产力。Java开发人员面临的一个主要挑战是将文件更改自动部署到服务器并自动重启服务器。 

开发人员可以重新加载Spring Boot上的更改，而无需重新启动服务器。这将消除每次手动部署更改的需要。Spring Boot在发布它的第一个版本时没有这个功能。 

这是开发人员最需要的功能。DevTools模块完全满足开发人员的需求。该模块将在生产环境中被禁用。它还提供H2数据库控制台以更好地测试应用程序。 

org.springframework.boot 

spring-boot-devtools 

true 



### SpringBoot的原理

**1、Spring Boot 自动配置的原理**

1. 注解 @EnableAutoConfiguration, @Configuration, @ConditionalOnClass 就是自动配置的核心，

2. @EnableAutoConfiguration 给容器导入META-INF/spring.factories 里定义的自动配置类。

3. 筛选有效的自动配置类。

4. 每一个自动配置类结合对应的 xxxProperties.java 读取配置文件进行自动配置功能

5. Spring Boot 需要独立的容器运行吗？

6. 1. 可以不需要，内置了 Tomcat/ Jetty 等容器。

**2、Spring Boot 配置加载顺序，几种方式来加载配置**

1. properties文件；

2. YAML文件；

3. 1. YAML 是一种人类可读的数据序列化语言。它通常用于配置文件。与属性文件相比，如果我们想要在配置文件中添加复杂的属性，YAML 文件就更加结构化，而且更少混淆。可以看出 YAML 具有分层配置数据。

   2. YAML 现在可以算是非常流行的一种配置文件格式了，无论是前端还是后端，都可以见到 YAML 配置。那么 YAML 配置和传统的 properties 配置相比到底有哪些优势呢？

   3. 1. 配置有序，在一些特殊的场景下，配置有序很关键
      2. 支持数组，数组中的元素可以是基本数据类型也可以是对象
      3. 简洁
      4. 缺点：相比 properties 配置文件，YAML 还有一个缺点，就是不支持 @PropertySource 注解导入自定义的 YAML 配置。

**3、系统环境变量**

**4、命令行参数**

**5、可以使用XML配置**

1. Spring Boot 推荐使用 Java 配置而非 XML 配置，但是 Spring Boot 中也可以使用 XML 配置，通过 @ImportResource 注解可以引入一个 XML 配置。



### Spring Boot 自动配置原理是什么？

注解 @EnableAutoConfiguration, @Configuration, @ConditionalOnClass 就是自动配置的核心，

@EnableAutoConfiguration 给容器导入META-INF/spring.factories 里定义的自动配置类。

筛选有效的自动配置类。

每一个自动配置类结合对应的 xxxProperties.java 读取配置文件进行自动配置功能







### 你如何理解 Spring Boot 中的 Starters？

Starters可以理解为启动器，它包含了一系列可以集成到应用里面的依赖包，你可以一站式集成 Spring 及其他技术，而不需要到处找示例代码和依赖包。如你想使用 Spring JPA 访问数据库，只要加入 spring-boot-starter-data-jpa 启动器依赖就能使用了。

Starters包含了许多项目中需要用到的依赖，它们能快速持续的运行，都是一系列得到支持的管理传递性依赖。



### spring-boot-starter-parent 有什么用 ?

我们都知道，新创建一个 Spring Boot 项目，默认都是有 parent 的，这个 parent 就是 spring-boot-starter-parent ，spring-boot-starter-parent 主要有如下作用：

定义了 Java 编译版本为 1.8 。
使用 UTF-8 格式编码。
继承自 spring-boot-dependencies，这个里边定义了依赖的版本，也正是因为继承了这个依赖，所以我们在写依赖时才不需要写版本号。
执行打包操作的配置。
自动化的资源过滤。
自动化的插件配置。
针对 application.properties 和 application.yml 的资源过滤，包括通过 profile 定义的不同环境的配置文件，例如 application-dev.properties 和 application-dev.yml。



### 什么是 Spring Boot Stater ？

启动器是一套方便的依赖没描述符，它可以放在自己的程序中。你可以一站式的获取你所需要的 Spring 和相关技术，而不需要依赖描述符的通过示例代码搜索和复制黏贴的负载。

例如，如果你想使用 Sping 和 JPA 访问数据库，只需要你的项目包含 spring-boot-starter-data-jpa 依赖项，你就可以完美进行。



### SpringBoot常用的starter有哪些?

**1、** `spring-boot-starter-web` (嵌入tomcat和web开发需要servlet与jsp支持) 

**2、** `spring-boot-starter-data-jpa` (数据库支持) 

**3、** `spring-boot-starter-data-redis` (redis数据库支持) 

**4、** `spring-boot-starter-data-solr` (solr搜索应用框架支持) 

**5、** `mybatis-spring-boot-starter` (第三方的mybatis集成starter)






### Spring Boot 的核心配置文件有哪几个？它们的区别是什么？

Spring Boot 的核心配置文件是 application 和 bootstrap 配置文件。

application 配置文件这个容易理解，主要用于 Spring Boot 项目的自动化配置。

bootstrap 配置文件有以下几个应用场景。

- 使用 Spring Cloud Config 配置中心时，这时需要在 bootstrap 配置文件中添加连接到配置中心的配置属性来加载外部配置中心的配置信息；
- 一些固定的不能被覆盖的属性；
- 一些加密/解密的场景；



### Spring Boot 的核心注解是哪个？它主要由哪几个注解组成的？

启动类上面的注解是@SpringBootApplication，它也是 Spring Boot 的核心注解，主要组合包含了以下 3 个注解：

**@SpringBootConfiguration：**组合了 @Configuration 注解，实现配置文件的功能。

**@EnableAutoConfiguration：**打开自动配置的功能，也可以关闭某个自动配置的选项，如关闭数据源自动配置功能： @SpringBootApplication(exclude = { DataSourceAutoConfiguration.class })。

**@ComponentScan：**Spring组件扫描。



### 创建一个 Spring Boot Project 的最简单的方法是什么？

Spring Initializr是启动 Spring Boot Projects 的一个很好的工具。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210329102421.png)

就像上图中所展示的一样，我们需要做一下几步：

**1、**登录 Spring Initializr，按照以下方式进行选择：

**2、**选择 com.in28minutes.springboot 为组

**3、**选择 studet-services 为组件

**4、**选择下面的依赖项

​    Web

​    Actuator

​    DevTools

**5、**点击生 GenerateProject

**6、**将项目导入 Eclipse。文件 - 导入 - 现有的 Maven 项目



###  Spring Initializr 是创建 Spring Boot Projects 的唯一方法吗？

不是的。

Spring Initiatlizr 让创建 Spring Boot 项目变的很容易，但是，你也可以通过设置一个 maven 项目并添加正确的依赖项来开始一个项目。

在我们的 Spring 课程中，我们使用两种方法来创建项目。

第一种方法是 start.spring.io 。

另外一种方法是在项目的标题为“Basic Web Application”处进行手动设置。

手动设置一个 maven 项目

这里有几个重要的步骤：

**1、**在 Eclipse 中，使用文件 - 新建 Maven 项目来创建一个新项目

**2、**添加依赖项。

**3、**添加 maven 插件。

**4、**添加 Spring Boot 应用程序类。

到这里，准备工作已经做好！



### 如何集成 Spring Boot 和 ActiveMQ？

对于集成 Spring Boot 和 ActiveMQ，我们使用依赖关系。 它只需要很少的配置，并且不需要样板代码。



### 什么是 Swagger？你用 Spring Boot 实现了它吗？

Swagger 广泛用于可视化 API，使用 Swagger UI 为前端开发人员提供在线沙箱。Swagger 是用于生成 RESTful Web 服务的可视化表示的工具，规范和完整框架实现。它使文档能够以与服务器相同的速度更新。当通过 Swagger 正确定义时，消费者可以使用最少量的实现逻辑来理解远程服务并与其进行交互。因此，Swagger消除了调用服务时的猜测。



### 运行 Spring Boot 有哪几种方式？

**1、**打包用命令或者放到容器中运行

**2、**用 Maven/ Gradle 插件运行

**3、**直接执行 main 方法运行



### Spring Boot 打成的 jar 和普通的 jar 有什么区别 ?

Spring Boot 项目最终打包成的 jar 是可执行 jar ，这种 jar 可以直接通过 java -jar xxx.jar 命令来运行，这种 jar 不可以作为普通的 jar 被其他项目依赖，即使依赖了也无法使用其中的类。

Spring Boot 的 jar 无法被其他项目依赖，主要还是他和普通 jar 的结构不同。普通的 jar 包，解压后直接就是包名，包里就是我们的代码，而 Spring Boot 打包成的可执行 jar 解压后，在 \BOOT-INF\classes 目录下才是我们的代码，因此无法被直接引用。如果非要引用，可以在 pom.xml 文件中增加配置，将 Spring Boot 项目打包成两个 jar ，一个可执行，一个可引用。



### 如何使用 Spring Boot 实现分页和排序？

使用 Spring Boot 实现分页非常简单。使用 Spring Data-JPA 可以实现将可分页的传递给存储库方法。



### Spring Boot 中如何实现定时任务 ?

定时任务也是一个常见的需求，Spring Boot 中对于定时任务的支持主要还是来自 Spring 框架。

在 Spring Boot 中使用定时任务主要有两种不同的方式，一个就是使用 Spring 中的 @Scheduled 注解，另一个则是使用第三方框架 Quartz。

使用 Spring 中的 @Scheduled 的方式主要通过 @Scheduled 注解来实现。

使用 Quartz ，则按照 Quartz 的方式，定义 Job 和 Trigger 即可。



### Spring Boot 中的 starter 到底是什么 

首先，这个 Starter 并非什么新的技术点，基本上还是基于 Spring 已有功能来实现的。

首先它提供了一个自动化配置类，一般命名为 XXXAutoConfiguration ，在这个配置类中通过条件注解来决定一个配置是否生效（条件注解就是 Spring 中原本就有的），然后它还会提供一系列的默认配置，也允许开发者根据实际情况自定义相关配置，然后通过类型安全的属性注入将这些配置属性注入进来，新注入的属性会代替掉默认属性。正因为如此，很多第三方框架，我们只需要引入依赖就可以直接使用了。当然，开发者也可以自定义 Starter



### spring-boot-starter-parent 有什么用

新创建一个 Spring Boot 项目，默认都是有 parent 的，这个 parent 就是 spring-boot-starter-parent ，spring-boot-starter-parent 主要有如下作用

**1、** 定义了 Java 编译版本为 1.8 。
**2、** 使用 UTF-8 格式编码。
**3、** 继承自 spring-boot-dependencies，这个里边定义了依赖的版本，也正是因为继承了这个依赖，所以我们在写依赖时才不需要写版本号。
**4、** 执行打包操作的配置。
**5、** 自动化的资源过滤。
**6、** 自动化的插件配置。
**7、** 针对 application.properties 和 application.yml 的资源过滤，包括通过 profile 定义的不同环境的配置文件，例如 application-dev.properties 和 application-dev.yml



### Spring Boot 打成的 jar 和普通的 jar 有什么区别

**1、** Spring Boot 项目最终打包成的 jar 是可执行 jar ，这种 jar 可以直接通过 java -jar xxx.jar 命令来运行，这种 jar 不可以作为普通的 jar 被其他项目依赖，即使依赖了也无法使用其中的类。
**2、** Spring Boot 的 jar 无法被其他项目依赖，主要还是他和普通 jar 的结构不同。普通的 jar 包，解压后直接就是包名，包里就是我们的代码，而 Spring Boot 打包成的可执行 jar 解压后，在 \BOOT-INF\classes 目录下才是我们的代码，因此无法被直接引用。如果非要引用，可以在 pom.xml 文件中增加配置，将 Spring Boot 项目打包成两个 jar ，一个可执行，一个可引用。

1. 1. 



### Spring Boot 还提供了其它的哪些 Starter Project Options？

Spring Boot 也提供了其它的启动器项目包括，包括用于开发特定类型应用程序的典型依赖项。

- spring-boot-starter-web-services - SOAP Web Services
- spring-boot-starter-web - Web 和 RESTful 应用程序
- spring-boot-starter-test - 单元测试和集成测试
- spring-boot-starter-jdbc - 传统的 JDBC
- spring-boot-starter-hateoas - 为服务添加 HATEOAS 功能
- spring-boot-starter-security - 使用 SpringSecurity 进行身份验证和授权
- spring-boot-starter-data-jpa - 带有 Hibeernate 的 Spring Data JPA
- spring-boot-starter-data-rest - 使用 Spring Data REST 公布简单的 REST 服务



### 为什么我们需要 spring-boot-maven-plugin?

spring-boot-maven-plugin 提供了一些像 jar 一样打包或者运行应用程序的命令。

**1、**spring-boot:run 运行你的 SpringBooty 应用程序。

**2、**spring-boot：repackage 重新打包你的 jar 包或者是 war 包使其可执行

**3、**spring-boot：start 和 spring-boot：stop 管理 Spring Boot 应用程序的生命周期（也可以说是为了集成测试）。

**4、**spring-boot:build-info 生成执行器可以使用的构造信息。



### Springboot集成mybatis的过程

添加mybatis的starter maven依赖 

```XML
<dependency>
    <groupId>org.mybatis.spring.boot</groupId>
    <artifactId>mybatis-spring-boot-starter</artifactId>
    <version>1.3.2</version>
</dependency>
```

在mybatis的接口中 添加@Mapper注解 

在application.yml配置数据源信息



### **什么是YAML？**

YAML是一种人类可读的数据序列化语言。它通常用于配置文件。 与属性文件相比，如果我们想要在配置文件中添加复杂的属性，YAML文件就更加结构化，而且更少混淆。可以看出YAML具有分层配置数据。



### YAML 配置的优势在哪里 ?

YAML 现在可以算是非常流行的一种配置文件格式了，无论是前端还是后端，都可以见到 YAML 配置。那么 YAML 配置和传统的 properties 配置相比到底有哪些优势呢？

1. 配置有序，在一些特殊的场景下，配置有序很关键
2. 支持数组，数组中的元素可以是基本数据类型也可以是对象
3. 简洁

相比 properties 配置文件，YAML 还有一个缺点，就是不支持 @PropertySource 注解导入自定义的 YAML 配置。



### Spring Boot 是否可以使用 XML 配置 ?

Spring Boot 推荐使用 Java 配置而非 XML 配置，但是 Spring Boot 中也可以使用 XML 配置，通过 @ImportResource 注解可以引入一个 XML 配置。



### spring boot 核心配置文件是什么？bootstrap.properties 和 application.properties 有何区别 ?

单纯做 Spring Boot 开发，可能不太容易遇到 bootstrap.properties 配置文件，但是在结合 Spring Cloud 时，这个配置就会经常遇到了，特别是在需要加载一些远程配置文件的时侯。

**spring boot 核心的两个配置文件：**

- **bootstrap (. yml 或者 . properties)：** boostrap 由父 ApplicationContext 加载的，比 applicaton 优先加载，配置在应用程序上下文的引导阶段生效。一般来说我们在 Spring Cloud Config 或者 Nacos 中会用到它。且 boostrap 里面的属性不能被覆盖；
- **application (. yml 或者 . properties)：** 由ApplicatonContext 加载，用于 spring boot 项目的自动化配置。



### 什么是 Spring Profiles？

Spring Profiles 允许用户根据配置文件（dev，test，prod 等）来注册 bean。因此，当应用程序在开发中运行时，只有某些 bean 可以加载，而在 PRODUCTION中，某些其他 bean 可以加载。假设我们的要求是 Swagger 文档仅适用于 QA 环境，并且禁用所有其他文档。这可以使用配置文件来完成。Spring Boot 使得使用配置文件非常简单。



### 什么是JavaConfig？

Spring JavaConfig是Spring社区的产品，它提供了配置Spring IoC容器的纯Java方法。因此它有助于避免使用XML配置。使用JavaConfig的优点在于：

面向对象的配置。由于配置被定义为JavaConfig中的类，因此用户可以充分利用Java中的面向对象功能。一个配置类可以继承另一个，重写它的@Bean方法等。

减少或消除XML配置。基于依赖注入原则的外化配置的好处已被证明。但是，许多开发人员不希望在XML和Java之间来回切换。

JavaConfig为开发人员提供了一种纯Java方法来配置与XML配置概念相似的Spring容器。

从技术角度来讲，只使用JavaConfig配置类来配置容器是可行的，但实际上很多人认为将JavaConfig与XML混合匹配是理想的。

类型安全和重构友好。JavaConfig提供了一种类型安全的方法来配置Spring容器。由于Java 5.0对泛型的支持，现在可以按类型而不是按名称检索bean，不需要任何强制转换或基于字符串的查找。Spring JavaConfig是Spring社区的产品，它提供了配置Spring IoC容器的纯Java方法。因此它有助于避免使用XML配置。使用JavaConfig的优点在于：

面向对象的配置。由于配置被定义为JavaConfig中的类，因此用户可以充分利用Java中的面向对象功能。一个配置类可以继承另一个，重写它的@Bean方法等。

减少或消除XML配置。基于依赖注入原则的外化配置的好处已被证明。但是，许多开发人员不希望在XML和Java之间来回切换。

JavaConfig为开发人员提供了一种纯Java方法来配置与XML配置概念相似的Spring容器。

从技术角度来讲，只使用JavaConfig配置类来配置容器是可行的，但实际上很多人认为将JavaConfig与XML混合匹配是理想的。

类型安全和重构友好。JavaConfig提供了一种类型安全的方法来配置Spring容器。由于Java 5.0对泛型的支持，现在可以按类型而不是按名称检索bean，不需要任何强制转换或基于字符串的查找。



### Spring Boot、Spring MVC 和 Spring 有什么区别？

**1、Spring**

Spring最重要的特征是依赖注入。所有 SpringModules 不是依赖注入就是 IOC 控制反转。

当我们恰当的使用 DI 或者是 IOC 的时候，我们可以开发松耦合应用。松耦合应用的单元测试可以很容易的进行。

**2、Spring MVC**

Spring MVC 提供了一种分离式的方法来开发 Web 应用。通过运用像 DispatcherServelet，MoudlAndView 和 ViewResolver 等一些简单的概念，开发 Web 应用将会变的非常简单。

**3、SpringBoot**

Spring 和 SpringMVC 的问题在于需要配置大量的参数。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210329101122.png)

Spring Boot 通过一个自动配置和启动的项来目解决这个问题。为了更快的构建产品就绪应用程序，Spring Boot 提供了一些非功能性特征。



### springboot自动配置的原理

只要使用了`@EnableAutoConfiguration`注解就能实现自动配置。

```java
@Target(ElementType.TYPE)
@Retention(RetentionPolicy.RUNTIME)
@Documented
@Inherited
@AutoConfigurationPackage
@Import(AutoConfigurationImportSelector.class)
public @interface EnableAutoConfiguration  

```

`@Import(AutoConfigurationImportSelector.class)`这个是自动配置的关键，它完成了自动配置的主要逻辑。 下面是代码的主要片段

```java
@Override
public String[] selectImports(AnnotationMetadata annotationMetadata) {
	if (!isEnabled(annotationMetadata)) {
		return NO_IMPORTS;
	}
   // 获取配置的元数据
   AutoConfigurationMetadata autoConfigurationMetadata = AutoConfigurationMetadataLoader
			.loadMetadata(this.beanClassLoader);
   // 这个方法包含了加载的主要逻辑，它能找到所有自动注入的类
   AutoConfigurationEntry autoConfigurationEntry = getAutoConfigurationEntry(
			autoConfigurationMetadata, annotationMetadata);
   return StringUtils.toStringArray(autoConfigurationEntry.getConfigurations());
}

```

下面来看`getAutoConfigurationEntry`的主要逻辑

```java
protected AutoConfigurationEntry getAutoConfigurationEntry(
		AutoConfigurationMetadata autoConfigurationMetadata,
		AnnotationMetadata annotationMetadata) {
	// ....
	// 获取候选配置类
	List<String> configurations = getCandidateConfigurations(annotationMetadata, attributes);
	// ... 过滤、去重、排除一些配置类
	return new AutoConfigurationEntry(configurations, exclusions);
}

```

> `SpringFactoriesLoader`是spring提供的一个扩展机制，它能加载模块下的`META-INF/sring.factories`文件，这个Properties格式的文件中的key是接口、注解、或抽象类的全名，value是以逗号“,"分隔的实现类。SpringFactoriesLoader能将相应的实现类注入Spirng容器中。

查看一下spring-boot-autoconfigure模块下的`META-INF/spring.factories`文件

```java
...
# Auto Configure
org.springframework.boot.autoconfigure.EnableAutoConfiguration=\
org.springframework.boot.autoconfigure.admin.SpringApplicationAdminJmxAutoConfiguration,\
org.springframework.boot.autoconfigure.aop.AopAutoConfiguration,\
...

```

就可以看出来它加载哪些自动配置类；通过这个机制我们可以自己写自动配置类并且在模块下的`META-INF/spring.factories`文件中写入

```java
org.springframework.boot.autoconfigure.EnableAutoConfiguration=\
org.yuan.interview.springboot.XXXAutoConfiguration
```

这样直接引入我们的模块就会加载`org.yuan.interview.springboot.XXXAutoConfiguration`配置类了。



### 如何禁用一个特定自动配置类？

**1、**使用`@EnableAutoConfiguration`的`exclude`属性。

```java
@EnableAutoConfiguration(exclude={DataSourceAutoConfiguration.class})
```



**2、**如果类不在类路径上，可以使用`@EnableAutoConfiguration`的`excludeName`属性

```java
@EnableAutoConfiguration(excludeName={Foo.class})
```



**3、**可以使用配置spring.autoconfigure.exclude属性来控制要排除的自动配置类列表。 在application.properties配置文件中配置属性，并且可以使用逗号分隔添加多个类。







### Spring Boot中的监视器是什么？

Spring boot actuator是spring启动框架中的重要功能之一。Spring boot监视器可帮助您访问生产环境中正在运行的应用程序的当前状态。

有几个指标必须在生产环境中进行检查和监控。即使一些外部应用程序可能正在使用这些服务来向相关人员触发警报消息。监视器模块公开了一组可直接作为HTTP URL访问的REST端点来检查状态。



### 什么是 Spring Batch?

`Spring Boot Batch`提供可重用的函数，这些函数在处理大量记录时非常重要；包括日志/跟踪，事务管理，作业处理统计信息，作业重新启动，跳过和资源管理。它还提供了更先进的技术服务和功能，通过优化和分区技术，可以实现极高批量和高性能批处理作业。简单以及复杂的大批量批处理作业可以高度可扩展的方式利用框架处理重要大量的信息。



### Spring Boot 中如何解决跨域问题 ?

跨域可以在前端通过 JSONP 来解决，但是 JSONP 只可以发送 GET 请求，无法发送其他类型的请求，在 RESTful 风格的应用中，就显得非常鸡肋，因此我们推荐在后端通过 （CORS，Cross-origin resource sharing） 来解决跨域问题。这种解决方案并非 Spring Boot 特有的，在传统的 SSM 框架中，就可以通过 CORS 来解决跨域问题，只不过之前我们是在 XML 文件中配置 CORS ，现在可以通过实现WebMvcConfigurer接口然后重写addCorsMappings方法解决跨域问题。

```java
@Configuration
public class CorsConfig implements WebMvcConfigurer {

    @Override
    public void addCorsMappings(CorsRegistry registry) {
        registry.addMapping("/**")
                .allowedOrigins("*")
                .allowCredentials(true)
                .allowedMethods("GET", "POST", "PUT", "DELETE", "OPTIONS")
                .maxAge(3600);
    }

}

```

项目中前后端分离部署，所以需要解决跨域的问题。
我们使用cookie存放用户登录的信息，在spring拦截器进行权限控制，当权限不符合时，直接返回给用户固定的json结果。
当用户登录以后，正常使用；当用户退出登录状态时或者token过期时，由于拦截器和跨域的顺序有问题，出现了跨域的现象。
我们知道一个http请求，先走filter，到达servlet后才进行拦截器的处理，如果我们把cors放在filter里，就可以优先于权限拦截器执行。

```java
@Configuration
public class CorsConfig {

    @Bean
    public CorsFilter corsFilter() {
        CorsConfiguration corsConfiguration = new CorsConfiguration();
        corsConfiguration.addAllowedOrigin("*");
        corsConfiguration.addAllowedHeader("*");
        corsConfiguration.addAllowedMethod("*");
        corsConfiguration.setAllowCredentials(true);
        UrlBasedCorsConfigurationSource urlBasedCorsConfigurationSource = new UrlBasedCorsConfigurationSource();
        urlBasedCorsConfigurationSource.registerCorsConfiguration("/**", corsConfiguration);
        return new CorsFilter(urlBasedCorsConfigurationSource);
    }

}

```



### 微服务中如何实现 session 共享 

在微服务中，一个完整的项目被拆分成多个不相同的独立的服务，各个服务独立部署在不同的服务器上，各自的 session 被从物理空间上隔离开了，但是经常，我们需要在不同微服务之间共享 session ，常见的方案就是 Spring Session + Redis 来实现 session 共享。将所有微服务的 session 统一保存在 Redis 上，当各个微服务对 session 有相关的读写操作时，都去操作 Redis 上的 session 。这样就实现了 session 共享，Spring Session 基于 Spring 中的代理过滤器实现，使得 session 的同步操作对开发人员而言是透明的，非常简便。



### 什么是 CSRF 攻击？

CSRF 代表跨站请求伪造。这是一种攻击，迫使最终用户在当前通过身份验证的Web 应用程序上执行不需要的操作。CSRF 攻击专门针对状态改变请求，而不是数据窃取，因为攻击者无法查看对伪造请求的响应。



### 我们如何监视所有 Spring Boot 微服务？

Spring Boot 提供监视器端点以监控各个微服务的度量。这些端点对于获取有关应用程序的信息（如它们是否已启动）以及它们的组件（如数据库等）是否正常运行很有帮助。但是，使用监视器的一个主要缺点或困难是，我们必须单独打开应用程序的知识点以了解其状态或健康状况。想象一下涉及 50 个应用程序的微服务，管理员将不得不击中所有 50 个应用程序的执行终端。为了帮助我们处理这种情况，我们将使用位于的开源项目。 它建立在 Spring Boot Actuator 之上，它提供了一个 Web UI，使我们能够可视化多个应用程序的度量。




### 什么是嵌入式服务器？我们为什么要使用嵌入式服务器呢?

思考一下在你的虚拟机上部署应用程序需要些什么。

**1、**安装 Java

**2、**安装 Web 或者是应用程序的服务器（Tomat/Wbesphere/Weblogic 等等）

**3、**部署应用程序 war 包

如果我们想简化这些步骤，应该如何做呢？

让我们来思考如何使服务器成为应用程序的一部分？

你只需要一个安装了 Java 的虚拟机，就可以直接在上面部署应用程序了，

这个想法是嵌入式服务器的起源。

当我们创建一个可以部署的应用程序的时候，我们将会把服务器（例如，tomcat）嵌入到可部署的服务器中。

例如，对于一个 Spring Boot 应用程序来说，你可以生成一个包含 Embedded Tomcat 的应用程序 jar。你就可以想运行正常 Java 应用程序一样来运行 web 应用程序了。

嵌入式服务器就是我们的可执行单元包含服务器的二进制文件（例如，tomcat.jar）。



### 当 Spring Boot 应用程序作为 Java 应用程序运行时，后台会发生什么？

如果你使用 Eclipse IDE，Eclipse maven 插件确保依赖项或者类文件的改变一经添加，就会被编译并在目标文件中准备好！在这之后，就和其它的 Java 应用程序一样了。

当你启动 java 应用程序的时候，spring boot 自动配置文件就会魔法般的启用了。

当 Spring Boot 应用程序检测到你正在开发一个 web 应用程序的时候，它就会启动 tomcat。



### RequestMapping 和 GetMapping 的不同之处在哪里？

RequestMapping 具有类属性的，可以进行 GET,POST,PUT 或者其它的注释中具有的请求方法。GetMapping 是 GET 请求方法中的一个特例。它只是 ResquestMapping 的一个延伸，目的是为了提高清晰度。



### 什么是 Spring Data？

Spring Data 的使命是在保证底层数据存储特殊性的前提下，为数据访问提供一个熟悉的，一致性的，基于 Spring 的编程模型。这使得使用数据访问技术，关系数据库和非关系数据库，map-reduce 框架以及基于云的数据服务变得很容易。

为了让它更简单一些，Spring Data 提供了不受底层数据源限制的 Abstractions 接口。

下面来举一个例子:

![图片](https://mmbiz.qpic.cn/mmbiz_png/KLTiaLuJImELSYlz43K7eJXnVZcbNPt3hLHwyT4Fq4J0QDyEib2HKs8RXLibTphzu4LQfUvId9fHwgEOLuccv6eew/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

你可以定义一简单的库，用来插入，更新，删除和检索代办事项，而不需要编写大量的代码。



### 什么是 Spring Data REST?

Spring Data TEST 可以用来发布关于 Spring 数据库的 HATEOAS RESTful 资源。

下面是一个使用 JPA 的例子:

![图片](https://mmbiz.qpic.cn/mmbiz_png/KLTiaLuJImELSYlz43K7eJXnVZcbNPt3hkicW88KlcduuBRPcmicEUrw3icd8Xt6zbbK7CcsP5V9oj3ib992iaiakEJCA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

不需要写太多代码，我们可以发布关于 Spring 数据库的 RESTful API。

下面展示的是一些关于 TEST 服务器的例子

```
POST:
URL:http：//localhost：8080/todos
Use Header:Content-Type:Type:application/json
Request Content
```



代码如下：

![图片](https://mmbiz.qpic.cn/mmbiz_png/KLTiaLuJImELSYlz43K7eJXnVZcbNPt3hTST5jZiaZrRUffjOVm693ptDSJnoPeHuRr07nHyE9VewExrO2uvzppA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

响应内容：

![图片](https://mmbiz.qpic.cn/mmbiz_png/KLTiaLuJImELSYlz43K7eJXnVZcbNPt3hhph3vaFppIXed4B9QChMtYOuNn0QH8cicD7zaicW9AfK1l7VljxuK3Sg/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

响应包含新创建资源的 href。



### 为什么我们不建议在实际的应用程序中使用 Spring Data Rest?

我们认为 Spring Data Rest 很适合快速原型制造！在大型应用程序中使用需要谨慎。

通过 Spring Data REST 你可以把你的数据实体作为 RESTful 服务直接发布。

当你设计 RESTful 服务器的时候，最佳实践表明，你的接口应该考虑到两件重要的事情：

你的模型范围。

你的客户。

通过 With Spring Data REST，你不需要再考虑这两个方面，只需要作为 TEST 服务发布实体。

这就是为什么我们建议使用 Spring Data Rest 在快速原型构造上面，或者作为项目的初始解决方法。对于完整演变项目来说，这并不是一个好的注意。



### 比较一下 Spring Security 和 Shiro 各自的优缺点 ?

由于 Spring Boot 官方提供了大量的非常方便的开箱即用的 Starter ，包括 Spring Security 的 Starter ，使得在 Spring Boot 中使用 Spring Security 变得更加容易，甚至只需要添加一个依赖就可以保护所有的接口，所以，如果是 Spring Boot 项目，一般选择 Spring Security 。当然这只是一个建议的组合，单纯从技术上来说，无论怎么组合，都是没有问题的。Shiro 和 Spring Security 相比，主要有如下一些特点：

**1、** Spring Security 是一个重量级的安全管理框架；Shiro 则是一个轻量级的安全管理框架

**2、** Spring Security 概念复杂，配置繁琐；Shiro 概念简单、配置简单

**3、** Spring Security 功能强大；Shiro 功能简单

