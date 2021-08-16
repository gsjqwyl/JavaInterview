**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**


<!-- TOC -->

- [什么是spring?](#什么是spring)
- [说说你对Spring的理解](#说说你对spring的理解)
- [使用Spring框架的好处是什么？](#使用spring框架的好处是什么)
- [Spring由哪些模块组成?](#spring由哪些模块组成)
- [Spring核心模块有哪些 ?](#spring核心模块有哪些-)
- [Spring框架使用了哪些设计模式](#spring框架使用了哪些设计模式)
- [Spring支持的ORM](#spring支持的orm)
- [Spring Framework 有哪些不同的功能？](#spring-framework-有哪些不同的功能)
- [什么是Spring的MVC框架？](#什么是spring的mvc框架)
- [什么是控制反转(IOC)？什么是依赖注入？](#什么是控制反转ioc什么是依赖注入)
- [什么是 Spring IOC 容器？](#什么是-spring-ioc-容器)
- [什么是依赖注入？](#什么是依赖注入)
- [可以通过多少种方式完成依赖注入？](#可以通过多少种方式完成依赖注入)
- [spring 中有多少种 IOC 容器？](#spring-中有多少种-ioc-容器)
- [区分 BeanFactory 和 ApplicationContext](#区分-beanfactory-和-applicationcontext)
- [Spring IoC 的实现机制](#spring-ioc-的实现机制)
- [列举 IoC 的一些好处。](#列举-ioc-的一些好处)
- [列举 Spring Framework 的优点。](#列举-spring-framework-的优点)
- [Spring Framework 有哪些不同的功能？](#spring-framework-有哪些不同的功能)
- [Spring Framework 中有多少个模块，它们分别是什么？](#spring-framework-中有多少个模块它们分别是什么)
- [什么是 spring bean？](#什么是-spring-bean)
- [Spring 提供了哪些配置方式？](#spring-提供了哪些配置方式)
- [springmvc常用到的注解，作用是什么，原理。](#springmvc常用到的注解作用是什么原理)
- [在 Spring 中，有几种配置 Bean 的方式？](#在-spring-中有几种配置-bean-的方式)
- [Spring 应用程序有哪些不同组件？](#spring-应用程序有哪些不同组件)
- [请解释一下 Spring Bean 的生命周期？](#请解释一下-spring-bean-的生命周期)
- [BeanFactory和ApplicationContext有什么区别？](#beanfactory和applicationcontext有什么区别)
- [Spring框架中的单例bean是线程安全的吗?](#spring框架中的单例bean是线程安全的吗)
- [Spring如何处理线程并发问题？](#spring如何处理线程并发问题)
- [什么是Spring的内部bean？](#什么是spring的内部bean)
- [Spring Bean 有哪些作用域，它们之间有什么区别？](#spring-bean-有哪些作用域它们之间有什么区别)
- [自动装配有哪些方式？](#自动装配有哪些方式)
- [自动装配有什么局限？](#自动装配有什么局限)
- [你用过哪些重要的 Spring 注解？](#你用过哪些重要的-spring-注解)
- [如何在 spring 中启动注解装配？](#如何在-spring-中启动注解装配)
- [@Component, @Controller, @Repository, @Service 有何区别？](#component-controller-repository-service-有何区别)
- [@Required 注解有什么用？](#required-注解有什么用)
- [@Autowired 注解有什么用？](#autowired-注解有什么用)
- [@Qualifier 注解有什么用？](#qualifier-注解有什么用)
- [@RequestMapping 注解有什么用？](#requestmapping-注解有什么用)
- [Springmvc controller方法中为什么不能定义局部变量？](#springmvc-controller方法中为什么不能定义局部变量)
- [spring DAO 有什么用？](#spring-dao-有什么用)
- [列举 Spring DAO 抛出的异常。](#列举-spring-dao-抛出的异常)
- [Spring JDBC API 中存在哪些类？](#spring-jdbc-api-中存在哪些类)
- [Spring 支持哪些 ORM 框架](#spring-支持哪些-orm-框架)
- [什么是 AOP？](#什么是-aop)
- [AOP实现的关键是什么 ?](#aop实现的关键是什么-)
- [AOP动态代理有几种方式 ?](#aop动态代理有几种方式-)
- [AOP 中的 Aspect、Advice、Pointcut、JointPoint 和 Advice 参数分别是什么？](#aop-中的-aspectadvicepointcutjointpoint-和-advice-参数分别是什么)
- [什么是通知（Advice）？](#什么是通知advice)
- [有哪些类型的通知（Advice）？](#有哪些类型的通知advice)
- [指出在 spring aop 中 concern 和 cross-cutting concern 的不同之处。](#指出在-spring-aop-中-concern-和-cross-cutting-concern-的不同之处)
- [AOP 有哪些实现方式？](#aop-有哪些实现方式)
- [Spring AOP and AspectJ AOP 有什么区别？](#spring-aop-and-aspectj-aop-有什么区别)
- [如何理解 Spring 中的代理？](#如何理解-spring-中的代理)
- [在 Spring中如何注入一个java集合？](#在-spring中如何注入一个java集合)
- [Spring MVC 框架有什么用？](#spring-mvc-框架有什么用)
- [什么是Spring MVC框架的控制器？](#什么是spring-mvc框架的控制器)
- [描述一下 DispatcherServlet 的工作流程](#描述一下-dispatcherservlet-的工作流程)
- [介绍一下 WebApplicationContext](#介绍一下-webapplicationcontext)
- [Spring DAO 有什么用？](#spring-dao-有什么用)
- [Spring JDBC API 中存在哪些类？](#spring-jdbc-api-中存在哪些类)
- [Spring框架中有哪些不同类型的事件？](#spring框架中有哪些不同类型的事件)
- [请解释一下，Spring 框架有哪些自动装配模式，它们之间有何区别？](#请解释一下spring-框架有哪些自动装配模式它们之间有何区别)
- [Springmvc 中DispatcherServlet初始化过程。](#springmvc-中dispatcherservlet初始化过程)
- [SpringMVC执行流程和原理  SpringMVC流程：](#springmvc执行流程和原理--springmvc流程)
- [WebApplicationContext](#webapplicationcontext)
- [你用过哪些重要的 Spring 注解？](#你用过哪些重要的-spring-注解)
- [DispatcherServlet](#dispatcherservlet)
- [@Component, @Controller, @Repository, @Service 有何区别？](#component-controller-repository-service-有何区别)
- [@Autowired 注解解释](#autowired-注解解释)
- [@Qualifier 注解解释](#qualifier-注解解释)
- [@Resource 注解解释](#resource-注解解释)
- [@Controller 注解](#controller-注解)
- [@RequestMapping 注解](#requestmapping-注解)
- [@Required 注解有什么用？](#required-注解有什么用)
- [@Autowire和@Resource区别](#autowire和resource区别)
- [SpringMVC中的拦截器和Servlet中的filter有什么区别？](#springmvc中的拦截器和servlet中的filter有什么区别)
- [讲讲Spring加载流程。](#讲讲spring加载流程)
- [Spring的IOC理解：](#spring的ioc理解)
- [列举 IoC 的一些好处](#列举-ioc-的一些好处)
- [Spring 中的 IoC 的实现原理就是工厂模式加反射机制。](#spring-中的-ioc-的实现原理就是工厂模式加反射机制)
- [Spring通知有哪些类型？](#spring通知有哪些类型)
- [解释一下Spring AOP里面的几个名词：](#解释一下spring-aop里面的几个名词)
- [**Spring AOP的实现原理。**](#spring-aop的实现原理)
- [在Spring AOP 中，关注点和横切关注的区别是什么？](#在spring-aop-中关注点和横切关注的区别是什么)
- [Spring中AOP的底层是怎么实现的？](#spring中aop的底层是怎么实现的)
- [Spring事务的实现方式和实现原理：](#spring事务的实现方式和实现原理)
- [讲讲Spring事务的传播属性。](#讲讲spring事务的传播属性)
- [Spring如何管理事务的](#spring如何管理事务的)
- [Spring框架的事务管理有哪些优点？](#spring框架的事务管理有哪些优点)
- [怎样用注解的方式配置Spring？](#怎样用注解的方式配置spring)
- [Spring怎么配置事务（具体说出一些关键的xml 元素）。](#spring怎么配置事务具体说出一些关键的xml-元素)
- [Springbean的生命周期](#springbean的生命周期)
- [Spring容器的bean什么时候被实例化？](#spring容器的bean什么时候被实例化)
- [说说 BeanFactory 和 ApplicationContext 的区别？ 什么是延迟实例化，它的优缺点是什么？](#说说-beanfactory-和-applicationcontext-的区别-什么是延迟实例化它的优缺点是什么)
- [BeanFactory – BeanFactory 实现举例](#beanfactory--beanfactory-实现举例)
- [XMLBeanFactory](#xmlbeanfactory)
- [Spring中Bean的作用域有哪些？](#spring中bean的作用域有哪些)

<!-- /TOC -->

### 什么是spring?

spring 首先它是一个框架，在我们的开发工作的环境中，所有的其他的框架基本都依赖Spring，spring起着一个容器的作用，用来承载我们整体的bean对象。它帮我们整理了整个bean的从创建到销毁的管理。



### 说说你对Spring的理解

**1、** Spring是一个开源框架，主要是为简化企业级应用开发而生。可以实现EJB可以实现的功能，Spring是一个IOC和AOP容器框架。 ♧ 控制反转（IOC）：Spring容器使用了工厂模式为我们创建了所需要的对象，我们使用时不需要自己去创建，直接调用Spring为我们提供的对象即可，这就是控制反转的思想。 ♧ 依赖注入（DI）：Spring使用Java Bean对象的Set方法或者带参数的构造方法为我们在创建所需对象时将其属性自动设置所需要的值的过程就是依赖注入的基本思想。 ♧ 面向切面编程（AOP）：在面向对象编程(OOP)思想中，我们将事物纵向抽象成一个个的对象。而在面向切面编程中，我们将一个个对象某些类似的方面横向抽象成一个切面，对这个切面进行一些如权限验证，事物管理，记录日志等公用操作处理的过程就是面向切面编程的思想。 

**2、** 在Spring中，所有管理的都是JavaBean对象，而BeanFactory和ApplicationContext就是Spring框架的那个IOC容器，现在一般使用ApplicationContext，其不但包括了BeanFactory的作用，同时还进行了更多的扩展。



###  使用Spring框架的好处是什么？

**1、轻量：** Spring 是轻量的，基本的版本大约2MB。

**2、控制反转：** Spring通过控制反转实现了松散耦合，对象们给出它们的依赖，而不是创建或查找依赖的对象们。

**3、面向切面的编程(AOP)：** Spring支持面向切面的编程，并且把应用业务逻辑和系统服务分开。

**4、容器：** Spring 包含并管理应用中对象的生命周期和配置。

**5、MVC框架** ：Spring的WEB框架是个精心设计的框架，是Web框架的一个很好的替代品。

**6、事务管理：** Spring 提供一个持续的事务管理接口，可以扩展到上至本地事务下至全局事务（JTA）。

**7、异常处理：** Spring 提供方便的API把具体技术相关的异常（比如由JDBC，Hibernate or JDO抛出的）转化为一致的unchecked 异常。



| 序号 | 好处              | 说明                                                         |
| ---- | ----------------- | ------------------------------------------------------------ |
| 1    | 轻量              | Spring 是轻量的，基本的版本大约2MB。                         |
| 2    | 控制反转          | Spring通过控制反转实现了松散耦合，对象们给出它们的依赖，而不是创建或查找依赖的对象们。 |
| 3    | 面向切面编程(AOP) | Spring支持面向切面的编程，并且把应用业务逻辑和系统服务分开。 |
| 4    | 容器              | Spring 包含并管理应用中对象的生命周期和配置。                |
| 5    | MVC框架           | Spring的WEB框架是个精心设计的框架，是Web框架的一个很好的替代品。 |
| 6    | 事务管理          | Spring 提供一个持续的事务管理接口，可以扩展到上至本地事务下至全局事务（JTA）。 |
| 7    | 异常处理          | Spring 提供方便的API把具体技术相关的异常(比如由JDBC，Hibernate or JDO抛出的)转化为一致的unchecked 异常。 |
| 8    | 最重要的          | 用的人多！！！                                               |





### Spring由哪些模块组成?

截止到目前Spring 框架已集成了 20 多个模块 。 这些模块主要被分如下图所示的核心容器 、 数据访问 / 集成 、Web、AOP （面向切面编程） 、 工具 、 消息和测试模块 。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210327015925.png)

以下是Spring 框架的基本模块：

- Core module
- Bean module
- Context module
- Expression Language module
- JDBC module
- ORM module
- OXM module
- Java Messaging Service(JMS) module
- Transaction module
- Web module
- Web-Servlet module
- Web-Struts module
- Web-Portlet module

| 核心模块       | 说明                                                         |
| -------------- | ------------------------------------------------------------ |
| Spring Core    | **核心容器**:核心容器提供Spring框架的基本功能。Spring以bean的方式组织和管理Java应用中的各个组件及其关系。Spring使用BeanFactory来产生和管理Bean，它是工厂模式的实现。BeanFactory使用控制反转(IoC)模式将应用的配置和依赖性规范与实际的应用程序代码分开 |
| Spring Context | **应用上下文**: 是一个配置文件，向Spring框架提供上下文信息。Spring上下文包括企业服务，如JNDI、EJB、电子邮件、国际化、校验和调度功能 |
| Spring AOP     | **面向切面编程**: 是面向对象编程的有效补充和完善，Spring的AOP是基于动态代理实现的，实现的方式有两种分别是Schema和AspectJ这两种方式 |
| Spring Dao     | **JDBC和Dao模块:** JDBC、DAO的抽象层提供了有意义的异常层次结构，可用该结构来管理异常处理，和不同数据库供应商所抛出的错误信息。异常层次结构简化了错误处理，并且极大的降低了需要编写的代码数量，比如打开和关闭链接 |
| Spring ORM     | **对象实体映射:** Spring框架插入了若干个ORM框架，从而提供了ORM对象的关系工具，其中包括了Hibernate、JDO和 IBatis SQL Map等，所有这些都遵从Spring的通用事物和DAO异常层次结构。 |
| Spring Web     | **Web模块:** Web上下文模块建立在应用程序上下文模块之上，为基于web的应用程序提供了上下文。所以Spring框架支持与Struts集成，web模块还简化了处理多部分请求以及将请求参数绑定到域对象的工作 |
| Spring Web MVC | **MVC模块:**MVC框架是一个全功能的构建Web应用程序的MVC实现。通过策略接口，MVC框架变成为高度可配置的。MVC容纳了大量视图技术，其中包括JSP、POI等，模型由JavaBean构成，存放于m当中，而视图是一个接口，负责实现模型，控制器表示逻辑代码，由c的事情。Spring框架的功能可以用在任何J2EE服务器当中，大多数功能也适用于不受管理的环境。Spring的核心要点就是支持不绑定到特定J2EE服务的可重用业务和数据的访问的对象，毫无疑问这样的对象可以在不同的J2EE环境，独立应用程序和测试环境之间重用。 |



### Spring核心模块有哪些 ?

**Spring Core：** 核心类库，提供IOC服务
**Spring AOP： **AOP服务
**Spring MVC：** 提供面向Web应用的Model-View-Controller实现
**Spring Web： ** 提供了基本的面向Web的综合特性，例如多方文件上传
**Spring Context：** 提供框架式的Bean访问方式，以及企业级功能（JNDI、定时任务等）
**Spring DAO：** 对JDBC的抽象，简化了数据访问异常的处理
**Spring ORM：** 对现有的ORM框架的支持



### Spring框架使用了哪些设计模式

**1、** 单例模式

**2、** 原型模式

**3、** 工厂模式

**4、** 适配器模式

**5、** 包装模式

**6、** 代理模式

**7、** 观察者模式

**8、** 策略模式

**9、** 模板模式



### Spring支持的ORM

Spring支持以下ORM：

Hibernate

iBatis

JPA (Java Persistence API)

TopLink

JDO (Java Data Objects)

OJB



### Spring Framework 有哪些不同的功能？

轻量级 - Spring 在代码量和透明度方面都很轻便。
IOC - 控制反转
AOP - 面向切面编程可以将应用业务逻辑和系统服务分离，以实现高内聚。
容器 - Spring 负责创建和管理对象（Bean）的生命周期和配置。
MVC - 对 web 应用提供了高度可配置性，其他框架的集成也十分方便。
事务管理 - 提供了用于事务管理的通用抽象层。Spring 的事务支持也可用于容器较少的环境。
JDBC 异常 - Spring 的 JDBC 抽象层提供了一个异常层次结构，简化了错误处理策略。



### 什么是Spring的MVC框架？

Spring 配备构建Web 应用的全功能MVC框架。Spring可以很便捷地和其他MVC框架集成，如Struts，Spring 的MVC框架用控制反转把业务对象和控制逻辑清晰地隔离。它也允许以声明的方式把请求参数和业务对象绑定。



### 什么是控制反转(IOC)？什么是依赖注入？

控制反转是应用于软件工程领域中的，在运行时被装配器对象来绑定耦合对象的一种编程技巧，对象之间耦合关系在编译时通常是未知的。在传统的编程方式中，业 务逻辑的流程是由应用程序中的早已被设定好关联关系的对象来决定的。在使用控制反转的情况下，业务逻辑的流程是由对象关系图来决定的，该对象关系图由装配 器负责实例化，这种实现方式还可以将对象之间的关联关系的定义抽象化。而绑定的过程是通过“依赖注入”实现的。控制反转是一种以给予应用程序中目标组件更多控制为目的设计范式，并在我们的实际工作中起到了有效的作用。依赖注入是在编译阶段尚未知所需的功能是来自哪个的类的情况下，将其他对象所依赖的功能对象实例化的模式。这就需要一种机制用来激活相应的组件以提供特定的功能，所以依赖注入是控制反转的基础。否则如果在组件不受框架控制的情况下，框架又怎么知道要创建哪个组件？在 Java 中依然注入有以下三种实现方式：

**1、** 构造器注入

**2、** Setter 方法注入

**3、** 接口注入



### 什么是 Spring IOC 容器？

Spring 框架的核心是 Spring 容器。容器创建对象，将它们装配在一起，配置它们并管理它们的完整生命周期。Spring 容器使用依赖注入来管理组成应用程序的组件。

容器通过读取提供的配置元数据来接收对象进行实例化，配置和组装的指令。该元数据可以通过 XML，Java 注解或 Java 代码提供。

![图片](https://mmbiz.qpic.cn/mmbiz_png/JfTPiahTHJhrA7s3UqnlzWAX3Uia8UO9icdAvicKiaXwEjyANro0iaHtKdCC5jgysmoapg6PyU8gT8JR682YHSdx8VAQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### 什么是依赖注入？

在依赖注入中，您不必创建对象，但必须描述如何创建它们。您不是直接在代码中将组件和服务连接在一起，而是描述配置文件中哪些组件需要哪些服务。由 IoC 容器将它们装配在一起。



### 可以通过多少种方式完成依赖注入？

通常，依赖注入可以通过三种方式完成，即：

- 构造函数注入
- setter 注入
- 接口注入

在 Spring Framework 中，仅使用构造函数和 setter 注入。



### spring 中有多少种 IOC 容器？

- BeanFactory - BeanFactory 就像一个包含 bean 集合的工厂类。它会在客户端要求时实例化 bean。
- ApplicationContext - ApplicationContext 接口扩展了 BeanFactory 接口。它在 BeanFactory 基础上提供了一些额外的功能。



### 区分 BeanFactory 和 ApplicationContext

![图片](https://mmbiz.qpic.cn/mmbiz_png/oTKHc6F8tshSRrp13FoDDfVNKUgujElkialapGTjSwWplWnMcsEQibBqxict661ULW3AcALxAbRdlqhBNK3ic9PFMQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### Spring IoC 的实现机制

Spring 中的 IoC 的实现原理就是工厂模式加反射机制。

示例：

```
interface Fruit {
     public abstract void eat();
}
class Apple implements Fruit {
    public void eat(){
        System.out.println("Apple");
    }
}
class Orange implements Fruit {
    public void eat(){
        System.out.println("Orange");
    }
}
class Factory {
    public static Fruit getInstance(String ClassName) {
        Fruit f=null;
        try {
            f=(Fruit)Class.forName(ClassName).newInstance();
        } catch (Exception e) {
            e.printStackTrace();
        }
        return f;
    }
}
class Client {
    public static void main(String[] a) {
        Fruit f=Factory.getInstance("io.github.dunwu.spring.Apple");
        if(f!=null){
            f.eat();
        }
    }
}
```



### 列举 IoC 的一些好处。

IoC 的一些好处是：

- 它将最小化应用程序中的代码量。
- 它将使您的应用程序易于测试，因为它不需要单元测试用例中的任何单例或 JNDI 查找机制。
- 它以最小的影响和最少的侵入机制促进松耦合。
- 它支持即时的实例化和延迟加载服务。



### 列举 Spring Framework 的优点。

由于 Spring Frameworks 的分层架构，用户可以自由选择自己需要的组件。

Spring Framework 支持 POJO(Plain Old Java Object) 编程，从而具备持续集成和可测试性。

由于依赖注入和控制反转，JDBC 得以简化。

它是开源免费的。



### Spring Framework 有哪些不同的功能？

轻量级 - Spring 在代码量和透明度方面都很轻便。

IOC - 控制反转

AOP - 面向切面编程可以将应用业务逻辑和系统服务分离，以实现高内聚。

容器 - Spring 负责创建和管理对象（Bean）的生命周期和配置。

MVC - 对 web 应用提供了高度可配置性，其他框架的集成也十分方便。

事务管理 - 提供了用于事务管理的通用抽象层。Spring 的事务支持也可用于容器较少的环境。

JDBC 异常 - Spring 的 JDBC 抽象层提供了一个异常层次结构，简化了错误处理策略。



### Spring Framework 中有多少个模块，它们分别是什么？

![图片](https://mmbiz.qpic.cn/mmbiz/xq9PqibkVAzoNMw1tg6TQ9cs2PUXG80NRibkA6DehRbQ6r7HAzAgEfibMvShjSNtYCzXwDQwpQ5ib6Ognz7uf2xcNw/640?wx_fmt=other&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**Spring 核心容器 – 该层基本上是 Spring Framework 的核心。它包含以下模块：**

- Spring Core
- Spring Bean
- SpEL (Spring Expression Language)
- Spring Context

**数据访问/集成 – 该层提供与数据库交互的支持。它包含以下模块：**

- JDBC (Java DataBase Connectivity)
- ORM (Object Relational Mapping)
- OXM (Object XML Mappers)
- JMS (Java Messaging Service)
- Transaction

**Web – 该层提供了创建 Web 应用程序的支持。它包含以下模块：**

- Web
- Web – Servlet
- Web – Socket
- Web – Portlet

**AOP** – 该层支持面向切面编程

**Instrumentation** – 该层为类检测和类加载器实现提供支持。

**Test** – 该层为使用 JUnit 和 TestNG 进行测试提供支持。

几个杂项模块:

- Messaging – 该模块为 STOMP 提供支持。它还支持注解编程模型，该模型用于从 WebSocket 客户端路由和处理 STOMP 消息
- Aspects – 该模块为与 AspectJ 的集成提供支持。





### 什么是 spring bean？

- 它们是构成用户应用程序主干的对象。
- Bean 由 Spring IoC 容器管理。
- 它们由 Spring IoC 容器实例化，配置，装配和管理。
- Bean 是基于用户提供给容器的配置元数据创建。



### Spring 提供了哪些配置方式？

- **基于 xml 配置**

bean 所需的依赖项和服务在 XML 格式的配置文件中指定。这些配置文件通常包含许多 bean 定义和特定于应用程序的配置选项。它们通常以 bean 标签开头。例如：

```xml
<bean id="studentbean" class="org.edureka.firstSpring.StudentBean">
 <property name="name" value="Edureka"></property>
</bean>
```

- **基于注解配置**

您可以通过在相关的类，方法或字段声明上使用注解，将 bean 配置为组件类本身，而不是使用 XML 来描述 bean 装配。默认情况下，Spring 容器中未打开注解装配。因此，您需要在使用它之前在 Spring 配置文件中启用它。例如：

```xml
<beans>
<context:annotation-config/>
<!-- bean definitions go here -->
</beans>
```

- **基于 Java API 配置**

Spring 的 Java 配置是通过使用 @Bean 和 @Configuration 来实现。

1. @Bean 注解扮演与 <bean /> 元素相同的角色。
2. @Configuration 类允许通过简单地调用同一个类中的其他 @Bean 方法来定义 bean 间依赖关系。

例如：

```java
@Configuration
public class StudentConfig {
    @Bean
    public StudentBean myStudent() {
        return new StudentBean();
    }
}
```



### springmvc常用到的注解，作用是什么，原理。

**@Controller注解** 

是在Spring的org.springframework.stereotype包下，org.springframework.stereotype.Controller注解类型用于指示Spring类的实例是一个控制器

使用@Controller注解的类不需要继承特定的父类或者实现特定的接口，相对之前的版本实现Controller接口变的更加简单。

而Controller接口的实现类只能处理一个单一的请求动作，而@Controller注解注解的控制器可以同时支持处理多个请求动作，使程序开发变的更加灵活。 @Controller用户标记一个类，使用它标记的类就是一个Spring MVC Controller对象，即：一个控制器类。Spring使用扫描机制查找应用程序中所有基于注解的控制器类，分发处理器会扫描使用了该注解的方法，并检测该方法是否使用了@RequestMapping注解，而使用@RequestMapping注解的方法才是真正处理请求的处理器。为了保证Spring能找到控制器，我们需要完成两件事：



**@RequestParam注解**

下面来说org.springframework.web.bind.annotation包下的第三个注解，即：@RequestParam注解，该注解类型用于将指定的请求参数赋值给方法中的形参。那么@RequestParam注解有什么属性呢？它有4种属性，下面将逐一介绍这四种属性：

**1、**name属性该属性的类型是String类型，它可以指定请求头绑定的名称； 

**2、**value属性该属性的类型是String类型，它可以设置是name属性的别名； 

**3、**required属性该属性的类型是boolean类型，它可以设置指定参数是否必须绑定； 

**4、**defalutValue属性该属性的类型是String类型，它可以设置如果没有传递参数可以使用默认值。



**@PathVaribale注解** 

下面来说org.springframework.web.bind.annotation包下的第四个注解，即：@PathVaribale注解，该注解类型可以非常方便的获得请求url中的动态参数。@PathVaribale注解只支持一个属性value，类型String，表示绑定的名称，如果省略则默认绑定同名参数。



### 在 Spring 中，有几种配置 Bean 的方式？

- 基于XML的配置
- 基于注解的配置
- 基于Java的配置



### Spring 应用程序有哪些不同组件？

Spring 应用一般有以下组件：

**接口** - 定义功能。

**Bean 类** - 它包含属性，setter 和 getter 方法，函数等。

**Spring 面向切面编程（AOP）**  - 提供面向切面编程的功能。

**Bean 配置文件**  - 包含类的信息以及如何配置它们。

**用户程序** - 它使用接口。



### 请解释一下 Spring Bean 的生命周期？

- 首先说一下Servlet的生命周期：实例化，初始init，接收请求service，销毁destroy；

   Spring上下文中的Bean生命周期也类似，如下：

  **1、实例化Bean：**

  对于BeanFactory容器，当客户向容器请求一个尚未初始化的bean时，或初始化bean的时候需要注入另一个尚未初始化的依赖时，容器就会调用createBean进行实例化。对于ApplicationContext容器，当容器启动结束后，通过获取BeanDefinition对象中的信息，实例化所有的bean。

  

  **2、设置对象属性（依赖注入）：**

  实例化后的对象被封装在BeanWrapper对象中，紧接着，Spring根据BeanDefinition中的信息 以及 通过BeanWrapper提供的设置属性的接口完成依赖注入。

  

  **3、处理Aware接口：**

  接着，Spring会检测该对象是否实现了xxxAware接口，并将相关的xxxAware实例注入给Bean：

  - 如果这个Bean已经实现了BeanNameAware接口，会调用它实现的setBeanName(String beanId)方法，此处传递的就是Spring配置文件中Bean的id值；
  - 如果这个Bean已经实现了BeanFactoryAware接口，会调用它实现的setBeanFactory()方法，传递的是Spring工厂自身。
  - 如果这个Bean已经实现了ApplicationContextAware接口，会调用setApplicationContext(ApplicationContext)方法，传入Spring上下文；

  

  **4、BeanPostProcessor：**

  如果想对Bean进行一些自定义的处理，那么可以让Bean实现了BeanPostProcessor接口，那将会调用postProcessBeforeInitialization(Object obj, String s)方法。由于这个方法是在Bean初始化结束时调用的，所以可以被应用于内存或缓存技术；

  

  **5、InitializingBean 与 init-method：**

  如果Bean在Spring配置文件中配置了 init-method 属性，则会自动调用其配置的初始化方法。

  

  **6、**如果这个Bean实现了BeanPostProcessor接口，将会调用postProcessAfterInitialization(Object obj, String s)方法；

  以上几个步骤完成后，Bean就已经被正确创建了，之后就可以使用这个Bean了。

  

  **7、DisposableBean：**

  当Bean不再需要时，会经过清理阶段，如果Bean实现了DisposableBean这个接口，会调用其实现的destroy()方法；

  

  **8、destroy-method：**

  最后，如果这个Bean的Spring配置中配置了destroy-method属性，会自动调用其配置的销毁方法。



### BeanFactory和ApplicationContext有什么区别？

在类图关系上BeanFactory是ApplicationContext接口的父接口

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210328194156.png)



![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210328194205.png)

**BeanFactory**

是spring中比较原始的Factory。如XMLBeanFactory就是一种典型的BeanFactory。原始的BeanFactory无法支持spring的许多插件，如AOP功能、Web应用等。

**ApplicationContext**

ApplicationContext接口是由BeanFactory接口派生而来，因而具有BeanFactory所有的功能。ApplicationContext以一种更向面向框架的方式工作以及对上下文进行分层和实现继承，ApplicationContext包还提供了以下的功能

1. MessageSource, 提供国际化的消息访问
2. 资源访问，如URL和文件
3. 事件传播
4. 载入多个（有继承关系）上下文 ，使得每一个上下文都专注于一个特定的层次，比如应用的web层,其实通过上面的类图大家应该也能看的出来BeanFactory和ApplicationContext的区别的。



### Spring框架中的单例bean是线程安全的吗?

肯定不是线程安全的，当多用户同时请求一个服务时，容器会给每一个请求分配一个线程，这是多个线程会并发执行该请求多对应的业务逻辑（成员方法），此时就要注意了，如果该处理逻辑中有对该单列状态的修改（体现为该单列的成员属性），则必须考虑线程同步问题.

Spring框架并没有对单例bean进行任何多线程的封装处理。关于单例bean的线程安全和并发问题需要开发者自行去搞定。但实际上，大部分的Spring bean并没有可变的状态(比如Serview类和DAO类)，所以在某种程度上说Spring的单例bean是线程安全的。如果你的bean有多种状态的话（比如 View Model 对象），就需要自行保证线程安全。最浅显的解决办法就是将多态bean的作用域由“singleton”变更为“prototype”。



### Spring如何处理线程并发问题？

在一般情况下，只有无状态的Bean才可以在多线程环境下共享，在Spring中，绝大部分Bean都可以声明为singleton作用域，因为Spring对一些Bean中非线程安全状态采用ThreadLocal进行处理，解决线程安全问题。

ThreadLocal和线程同步机制都是为了解决多线程中相同变量的访问冲突问题。同步机制采用了“时间换空间”的方式，仅提供一份变量，不同的线程在访问前需要获取锁，没获得锁的线程则需要排队。而ThreadLocal采用了“空间换时间”的方式。

ThreadLocal会为每一个线程提供一个独立的变量副本，从而隔离了多个线程对数据的访问冲突。因为每一个线程都拥有自己的变量副本，从而也就没有必要对该变量进行同步了。ThreadLocal提供了线程安全的共享对象，在编写多线程代码时，可以把不安全的变量封装进ThreadLocal。



### 什么是Spring的内部bean？

当一个bean仅被用作另一个bean的属性时，它能被声明为一个内部bean，为了定义inner bean，在Spring 的 基于XML的 配置元数据中，可以在 或\ 元素内使用 元素，内部bean通常是匿名的，它们的Scope一般是prototype。

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">
 
	<bean id="CustomerBean" class="com.dpb.common.Customer">
		<property name="person" ref="PersonBean"/>
	</bean>
	
	<bean id="PersonBean" class="com.dpb.common.Person">
		<property name="name" value="波波烤鸭"/>
		<property name="address" value="深圳"/>
		<property name="age" value="17"/>
	</bean>
</beans>

```

**改为内部bean的方式**

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">
 
	<bean id="CustomerBean" class="com.dpb.common.Customer">
		<property name="person">
			<bean class="com.dpb.common.Person">
				<property name="name" value="波波烤鸭"/>
				<property name="address" value="湖南"/>
				<property name="age" value="17"/>
			</bean>		
		</property>
	</bean>
</beans>

```

**内部 bean 也支持构造器注入**

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">
 
	<bean id="CustomerBean" class="com.dpb.common.Customer">
		<constructor-arg >
			<bean class="com.dpb.common.Person">
				<property name="name" value="波波烤鸭"/>
				<property name="address" value="湖南"/>
				<property name="age" value="17"/>
			</bean>		
		</constructor-arg>
	</bean>
</beans>

```

id 或 name 值在bean类是没有必要以一个内部 bean 呈现



### Spring Bean 有哪些作用域，它们之间有什么区别？

**singleton ：** 这种 bean 范围是**默认**的，这种范围确保不管接受到多少个请求，每个容器中只有一个 bean 的实例，单例的模式由 bean factory 自身来维护 。

**prototype ：** 原形范围与单例范围相反，为每一个 bean 请求提供一个实例 。

**request ：** 在请求 bean 范围内会每一个来自客户端的网络请求创建一个实例，在请求完成以后， bean 会失效并被垃圾回收器回收 。

**Session ：** 与请求范围类似，确保每个 session 中有一个 bean 的实例，在 session 过期后， bean 会随之失效 。

**global-session ：** global-session 和 Portlet 应用相关 。 当你的应用部署在 Portlet 容器中工作时，它包含很多 portlet。 如果你想要声明让所有的 portlet 共用全局的存储变量的话，那么这全局变量需要存储在 global-session 中 。



### 自动装配有哪些方式？

Spring 容器能够自动装配 bean。也就是说，可以通过检查 BeanFactory 的内容让 Spring 自动解析 bean 的协作者。

自动装配的不同模式：

- no - 这是默认设置，表示没有自动装配。应使用显式 bean 引用进行装配。
- byName - 它根据 bean 的名称注入对象依赖项。它匹配并装配其属性与 XML 文件中由相同名称定义的 bean。
- byType - 它根据类型注入对象依赖项。如果属性的类型与 XML 文件中的一个 bean 名称匹配，则匹配并装配属性。
- 构造函数 - 它通过调用类的构造函数来注入依赖项。它有大量的参数。
- autodetect - 首先容器尝试通过构造函数使用 autowire 装配，如果不能，则尝试通过 byType 自动装配。



### 自动装配有什么局限？

- 覆盖的可能性 - 您始终可以使用<constructor-arg> 和 <property>设置指定依赖项，这将覆盖自动装配。
- 基本元数据类型 - 简单属性（如原数据类型，字符串和类）无法自动装配。
- 令人困惑的性质 - 总是喜欢使用明确的装配，因为自动装配不太精确。



### 你用过哪些重要的 Spring 注解？

- @Controller - 用于 Spring MVC 项目中的控制器类。
- @Service - 用于服务类。
- @RequestMapping - 用于在控制器处理程序方法中配置 URI 映射。
- @ResponseBody - 用于发送 Object 作为响应，通常用于发送 XML 或 JSON 数据作为响应。
- @PathVariable - 用于将动态值从 URI 映射到处理程序方法参数。
- @Autowired - 用于在 spring bean 中自动装配依赖项。
- @Qualifier - 使用 @Autowired 注解，以避免在存在多个 bean 类型实例时出现混淆。
- @Scope - 用于配置 spring bean 的范围。
- @Configuration，@ComponentScan 和 @Bean - 用于基于 java 的配置。
- @Aspect，@Before，@After，@Around，@Pointcut - 用于切面编程（AOP）。



### 如何在 spring 中启动注解装配？

默认情况下，Spring 容器中未打开注解装配。因此，要使用基于注解装配，我们必须通过配置<context：annotation-config /> 元素在 Spring 配置文件中启用它。



### @Component, @Controller, @Repository, @Service 有何区别？

- @Component：这将 java 类标记为 bean。它是任何 Spring 管理组件的通用构造型。spring 的组件扫描机制现在可以将其拾取并将其拉入应用程序环境中。
- @Controller：这将一个类标记为 Spring Web MVC 控制器。标有它的 Bean 会自动导入到 IoC 容器中。
- @Service：此注解是组件注解的特化。它不会对 @Component 注解提供任何其他行为。您可以在服务层类中使用 @Service 而不是 @Component，因为它以更好的方式指定了意图。
- @Repository：这个注解是具有类似用途和功能的 @Component 注解的特化。它为 DAO 提供了额外的好处。它将 DAO 导入 IoC 容器，并使未经检查的异常有资格转换为 Spring DataAccessException。



### @Required 注解有什么用？

@Required 应用于 bean 属性 setter 方法。此注解仅指示必须在配置时使用 bean 定义中的显式属性值或使用自动装配填充受影响的 bean 属性。如果尚未填充受影响的 bean 属性，则容器将抛出 BeanInitializationException。

示例：

```java
public class Employee {
    private String name;
    @Required
    public void setName(String name){
        this.name=name;
    }
    public string getName(){
        return name;
    }
}
```



### @Autowired 注解有什么用？

@Autowired 可以更准确地控制应该在何处以及如何进行自动装配。此注解用于在 setter 方法，构造函数，具有任意名称或多个参数的属性或方法上自动装配 bean。默认情况下，它是类型驱动的注入。

```java
public class Employee {
    private String name;
    @Autowired
    public void setName(String name) {
        this.name=name;
    }
    public string getName(){
        return name;
    }
}
```



### @Qualifier 注解有什么用？

当您创建多个相同类型的 bean 并希望仅使用属性装配其中一个 bean 时，您可以使用@Qualifier 注解和 @Autowired 通过指定应该装配哪个确切的 bean 来消除歧义。

例如，这里我们分别有两个类，Employee 和 EmpAccount。在 EmpAccount 中，使用@Qualifier 指定了必须装配 id 为 emp1 的 bean。

```java
public class Employee {
    private String name;
    @Autowired
    public void setName(String name) {
        this.name=name;
    }
    public string getName() {
        return name;
    }
}
```

EmpAccount.java

```java
public class EmpAccount {
    private Employee emp;
    @Autowired
    @Qualifier(emp1)
    public void showName() {
        System.out.println(“Employee name : ”+emp.getName);
    }
}
```



### @RequestMapping 注解有什么用？

@RequestMapping 注解用于将特定 HTTP 请求方法映射到将处理相应请求的控制器中的特定类/方法。此注解可应用于两个级别：

- 类级别：映射请求的 URL
- 方法级别：映射 URL 以及 HTTP 请求方法



### Springmvc controller方法中为什么不能定义局部变量？

因为controller是默认单例模式，高并发下全局变量会出现线程安全问题

现这种问题如何解决呢？

**1、** 既然是全局变量惹的祸，那就将全局变量都编程局部变量，通过方法参数来传递。

**2、** jdk提供了java.lang.ThreadLocal,它为多线程并发提供了新思路。

**3、** 使用@Scope("session")，会话级别

```java
    @Controller  
    //把这个bean 的范围设置成session，表示这bean是会话级别的，  
    @Scope("session")  
    public class XxxController{  
        private List<String> list ;  
 
      //@PostConstruct当bean加载完之后，就会执行init方法，并且将list实例化；  
        @PostConstruct  
        public void init(){  
            list = new ArrayList<String>();  
        }  
    } 
```

**4、** 将控制器的作用域从单例改为原型，即在spring配置文件Controller中声明 scope="prototype"，每次都创建新的controller



### spring DAO 有什么用？

Spring DAO 使得 JDBC，Hibernate 或 JDO 这样的数据访问技术更容易以一种统一的方式工作。这使得用户容易在持久性技术之间切换。它还允许您在编写代码时，无需考虑捕获每种技术不同的异常。



### 列举 Spring DAO 抛出的异常。

![图片](https://mmbiz.qpic.cn/mmbiz_png/JfTPiahTHJhrA7s3UqnlzWAX3Uia8UO9icdJHa6RwkusOYA9LniacOPQibmrXN5QNCSpNn4ZBTHpicJAbW6juY51ga3Q/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### Spring JDBC API 中存在哪些类？

- JdbcTemplate
- SimpleJdbcTemplate
- NamedParameterJdbcTemplate
- SimpleJdbcInsert
- SimpleJdbcCall



### Spring 支持哪些 ORM 框架

- Hibernate
- iBatis
- JPA
- JDO
- OJB



### 什么是 AOP？

AOP(Aspect-Oriented Programming), 即 面向切面编程, 它与 OOP( Object-Oriented Programming, 面向对象编程) 相辅相成, 提供了与 OOP 不同的抽象软件结构的视角.

在 OOP 中, 我们以类(class)作为我们的基本单元, 而 AOP 中的基本单元是 Aspect(切面)



### AOP实现的关键是什么 ?

**关键：**
关键在于代理模式
AOP代理主要分为静态代理和动态代理。

**静态代理：**
代表：AspectJ
解析：就是AOP框架会在编译阶段生成AOP代理类，因此也称为编译时增强，
他会在编译阶段将AspectJ(切面)织入到Java字节码中

**动态代理：**
代表：Spring AOP
解析：就是说AOP框架不会去修改字节码，而是每次运行时在内存中临时为
方法生成一个AOP对象，这个AOP对象包含了目标对象的全部方法

**两种代理区别：**
区别：生成AOP代理对象的时机不同，相对来说AspectJ性能更好，
但是AspectJ需要特定的编译器进行处理，而Spring AOP则无需特定的编译器处理



### AOP动态代理有几种方式 ?

2种
JDK动态代理和CGLIB动态代理

**JDK动态代理：**
**核心：** InvocationHandler接口和Proxy类
**解析：** JDK动态代理只提供接口的代理，不支持类的代理。
InvocationHandler 通过invoke()方法反射来调用目标类中的代码

**CGLIB动态代理：**
**核心：** CGLIB（Code Generation Library），是一个代码生成的类库
**解析：** CGLIB是通过继承的方式做的动态代理，因此如果某个类被标记为final，
那么它是无法使用CGLIB做动态代理的



### AOP 中的 Aspect、Advice、Pointcut、JointPoint 和 Advice 参数分别是什么？

![图片](https://mmbiz.qpic.cn/mmbiz_png/JfTPiahTHJhrA7s3UqnlzWAX3Uia8UO9icdMhI2Z8eT5JwVm9Z4O6ZChPLN7s7fckjMdHPg18ZW4O3DU9Cd4b2Wmg/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**1、Aspect - Aspect** 是一个实现交叉问题的类，例如事务管理。方面可以是配置的普通类，然后在 Spring Bean 配置文件中配置，或者我们可以使用 Spring AspectJ 支持使用 @Aspect 注解将类声明为 Aspect。

**2、Advice - Advice** 是针对特定 JoinPoint 采取的操作。在编程方面，它们是在应用程序中达到具有匹配切入点的特定 JoinPoint 时执行的方法。您可以将 Advice 视为 Spring 拦截器（Interceptor）或 Servlet 过滤器（filter）。

**3、Advice Arguments** - 我们可以在 advice 方法中传递参数。我们可以在切入点中使用 args() 表达式来应用于与参数模式匹配的任何方法。如果我们使用它，那么我们需要在确定参数类型的 advice 方法中使用相同的名称。

**4、Pointcut - Pointcut** 是与 JoinPoint 匹配的正则表达式，用于确定是否需要执行 Advice。Pointcut 使用与 JoinPoint 匹配的不同类型的表达式。Spring 框架使用 AspectJ Pointcut 表达式语言来确定将应用通知方法的 JoinPoint。

**5、JoinPoint - JoinPoint** 是应用程序中的特定点，例如方法执行，异常处理，更改对象变量值等。在 Spring AOP 中，JoinPoint 始终是方法的执行器。



### 什么是通知（Advice）？

特定 JoinPoint 处的 Aspect 所采取的动作称为 Advice。Spring AOP 使用一个 Advice 作为拦截器，在 JoinPoint “周围”维护一系列的拦截器。



### 有哪些类型的通知（Advice）？

- Before - 这些类型的 Advice 在 joinpoint 方法之前执行，并使用 @Before 注解标记进行配置。
- After Returning - 这些类型的 Advice 在连接点方法正常执行后执行，并使用@AfterReturning 注解标记进行配置。
- After Throwing - 这些类型的 Advice 仅在 joinpoint 方法通过抛出异常退出并使用 @AfterThrowing 注解标记配置时执行。
- After (finally) - 这些类型的 Advice 在连接点方法之后执行，无论方法退出是正常还是异常返回，并使用 @After 注解标记进行配置。
- Around - 这些类型的 Advice 在连接点之前和之后执行，并使用 @Around 注解标记进行配置。



### 指出在 spring aop 中 concern 和 cross-cutting concern 的不同之处。

concern 是我们想要在应用程序的特定模块中定义的行为。它可以定义为我们想要实现的功能。

cross-cutting concern 是一个适用于整个应用的行为，这会影响整个应用程序。例如，日志记录，安全性和数据传输是应用程序几乎每个模块都需要关注的问题，因此它们是跨领域的问题。



### AOP 有哪些实现方式？

实现 AOP 的技术，主要分为两大类：

- 静态代理 - 指使用 AOP 框架提供的命令进行编译，从而在编译阶段就可生成 AOP 代理类，因此也称为编译时增强；
- 编译时编织（特殊编译器实现）
- 类加载时编织（特殊的类加载器实现）。
- 动态代理 - 在运行时在内存中“临时”生成 AOP 动态代理类，因此也被称为运行时增强。
- JDK 动态代理
- CGLIB



###  Spring AOP and AspectJ AOP 有什么区别？

Spring AOP 基于动态代理方式实现；AspectJ 基于静态代理方式实现。

Spring AOP 仅支持方法级别的 PointCut；提供了完全的 AOP 支持，它还支持属性级别的 PointCut。



### 如何理解 Spring 中的代理？

将 Advice 应用于目标对象后创建的对象称为代理。在客户端对象的情况下，目标对象和代理对象是相同的。

```
Advice + Target Object = Proxy
```





### 在 Spring中如何注入一个java集合？

Spring提供以下几种集合的配置元素：

| 元素      | 说明                                               |
| --------- | -------------------------------------------------- |
| **list**  | 类型用于注入一列值，允许有相同的值。               |
| **set**   | 类型用于注入一组值，不允许有相同的值。             |
| **map**   | 类型用于注入一组键值对，键和值都可以为任意类型。   |
| **props** | 类型用于注入一组键值对，键和值都只能为String类型。 |

```xml
<!-- 配置 student对象 -->
<bean class="com.dpb.javabean.Student">
	<property name="id" value="10"/>
	<property name="name" value="波波烤鸭"/>
	<!-- 对象注入 -->
	<property name="cat" ref="catId"></property>
	<!-- List集合注入 -->
	<property name="games">
		<list>
			<value>LOL</value>
			<value>DNF</value>
			<value>CS</value>
		</list>
	</property>
<property name="score">
	<map>
		<entry key="数学" value="99"/>
		<entry key="英语" value="78"/>
		<entry key="化学" value="84"/>
	</map>
</property>
<property name="props">
	<props>
		<prop key="userName">admin</prop>
		<prop key="password">123</prop>
	</props>
</property>


```



###  Spring MVC 框架有什么用？

Spring Web MVC 框架提供 模型-视图-控制器 架构和随时可用的组件，用于开发灵活且松散耦合的 Web 应用程序。MVC 模式有助于分离应用程序的不同方面，如输入逻辑，业务逻辑和 UI 逻辑，同时在所有这些元素之间提供松散耦合。



### 什么是Spring MVC框架的控制器？

控制器提供一个访问应用程序的行为，此行为通常通过服务接口实现。控制器解析用户输入并将其转换为一个由视图呈现给用户的模型。Spring用一个非常抽象的方式实现了一个控制层，允许用户创建多种用途的控制器。



### 描述一下 DispatcherServlet 的工作流程

DispatcherServlet 的工作流程可以用一幅图来说明：

![图片](https://mmbiz.qpic.cn/mmbiz_png/JfTPiahTHJhrA7s3UqnlzWAX3Uia8UO9icdG0z2VDCwn4J76bx3co50iagSyWsrUd0WRUkerRe7Yeu5RDNkg0g6QlA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**1、** 向服务器发送 HTTP 请求，请求被前端控制器 DispatcherServlet 捕获。

**2、** DispatcherServlet 根据 -servlet.xml 中的配置对请求的 URL 进行解析，得到请求资源标识符（URI）。然后根据该 URI，调用 HandlerMapping 获得该 Handler 配置的所有相关的对象（包括 Handler 对象以及 Handler 对象对应的拦截器），最后以HandlerExecutionChain 对象的形式返回。

**3、** DispatcherServlet 根据获得的Handler，选择一个合适的 HandlerAdapter。（附注：如果成功获得HandlerAdapter后，此时将开始执行拦截器的 preHandler(…)方法）。

**4、** 提取Request中的模型数据，填充Handler入参，开始执行Handler（Controller)。在填充Handler的入参过程中，根据你的配置，Spring 将帮你做一些额外的工作：

- HttpMessageConveter：将请求消息（如 Json、xml 等数据）转换成一个对象，将对象转换为指定的响应信息。
- 数据转换：对请求消息进行数据转换。如`String`转换成`Integer`、`Double`等。
- 数据根式化：对请求消息进行数据格式化。如将字符串转换成格式化数字或格式化日期等。
- 数据验证：验证数据的有效性（长度、格式等），验证结果存储到`BindingResult`或`Error`中。

**5、** Handler(Controller)执行完成后，向 DispatcherServlet 返回一个 ModelAndView 对象；

**6、** 根据返回的ModelAndView，选择一个适合的 ViewResolver（必须是已经注册到 Spring 容器中的ViewResolver)返回给DispatcherServlet。

**7、** ViewResolver 结合Model和View，来渲染视图。

**8、** 视图负责将渲染结果返回给客户端。



### 介绍一下 WebApplicationContext

WebApplicationContext 是 ApplicationContext 的扩展。它具有 Web 应用程序所需的一些额外功能。它与普通的 ApplicationContext 在解析主题和决定与哪个 servlet 关联的能力方面有所不同。



### Spring DAO 有什么用？

Spring DAO 使得 JDBC，Hibernate 或 JDO 这样的数据访问技术更容易以一种统一的方式工作。这使得用户容易在持久性技术之间切换。它还允许您在编写代码时，无需考虑捕获每种技术不同的异常。



### Spring JDBC API 中存在哪些类？

- JdbcTemplate
- SimpleJdbcTemplate
- NamedParameterJdbcTemplate
- SimpleJdbcInsert
- SimpleJdbcCall



### Spring框架中有哪些不同类型的事件？

Spring 提供了以下5种标准的事件：

**1、上下文更新事件（ContextRefreshedEvent）：** 在调用ConfigurableApplicationContext 接口中的refresh()方法时被触发。

**2、上下文开始事件（ContextStartedEvent）：** 当容器调用ConfigurableApplicationContext的Start()方法开始/重新开始容器时触发该事件。

**3、上下文停止事件（ContextStoppedEvent）：** 当容器调用ConfigurableApplicationContext的Stop()方法停止容器时触发该事件。

**4、上下文关闭事件（ContextClosedEvent）：** 当ApplicationContext被关闭时触发该事件。容器被关闭时，其管理的所有单例Bean都被销毁。

**5、请求处理事件（RequestHandledEvent）：** 在Web应用中，当一个http请求（request）结束触发该事件。



如果一个bean实现了ApplicationListener接口，当一个ApplicationEvent 被发布以后，bean会自动被通知。



### 请解释一下，Spring 框架有哪些自动装配模式，它们之间有何区别？

**no ：** 这是 Spring 框架的**默认**设置，在该设置下自动装配是关闭的，开发者需要自行在 bean 定义中用标签明确的设置依赖关系 。

**byName ：** 该选项可以根据 **bean 名称**设置依赖关系 。 当向一个 bean 中自动装配一个属性时，容器将根据 bean 的名称自动在在配置文件中查询一个匹配的 bean。 如果找到的话，就装配这个属性，如果没找到的话就报错 。

**byType ：** 该选项可以根据 bean 类型设置依赖关系 。 当向一个 bean 中自动装配一个属性时，容器将根据 bean 的类型自动在在配置文件中查询一个匹配的 bean。 如果找到的话，就装配这个属性，如果没找到的话就报错 。

**constructor ：** 构造器的自动装配和 byType 模式类似，但是仅仅适用于与有构造器相同参数的 bean ，如果在容器中没有找到与构造器参数类型一致的 bean ，那么将会抛出异常 。

**autodetect ：** 该模式自动探测使用构造器自动装配或者 byType 自动装配 。 首先，首先会尝试找合适的带参数的构造器，如果找到的话就是用构造器自动装配，如果在 bean 内部没有找到相应的构造器或者是无参构造器，容器就会自动选择 byTpe 的自动装配方式 。



### Springmvc 中DispatcherServlet初始化过程。

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210328183208.png)





### SpringMVC执行流程和原理  SpringMVC流程：

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210328185541.png)

**1、** 用户发送出请求到前端控制器DispatcherServlet。

**2、** DispatcherServlet收到请求调用HandlerMapping（处理器映射器）。

**3、** HandlerMapping找到具体的处理器(可查找xml配置或注解配置)，生成处理器对象及处理器拦截器(如果有)，再一起返回给DispatcherServlet。

**4、** DispatcherServlet调用HandlerAdapter（处理器适配器）。

**5、** HandlerAdapter经过适配调用具体的处理器（Handler/Controller）。

**6、** Controller执行完成返回ModelAndView对象。

**7、 **HandlerAdapter将Controller执行结果ModelAndView返回给DispatcherServlet。

**8、** DispatcherServlet将ModelAndView传给ViewReslover（视图解析器）。

**9、** ViewReslover解析后返回具体View（视图）。

**10、** DispatcherServlet根据View进行渲染视图（即将模型数据填充至视图中）。

**11、** DispatcherServlet响应用户。



### WebApplicationContext

WebApplicationContext 继承了ApplicationContext 并增加了一些WEB应用必备的特有功能，它不同于一般的ApplicationContext ，因为它能处理主题，并找到被关联的servlet。



### 你用过哪些重要的 Spring 注解？

@Controller - 用于 Spring MVC 项目中的控制器类。
@Service - 用于服务类。
@RequestMapping - 用于在控制器处理程序方法中配置 URI 映射。
@ResponseBody - 用于发送 Object 作为响应，通常用于发送 XML 或 JSON 数据作为响应。
@PathVariable - 用于将动态值从 URI 映射到处理程序方法参数。
@Autowired - 用于在 spring bean 中自动装配依赖项。
@Qualifier - 使用 @Autowired 注解，以避免在存在多个 bean 类型实例时出现混淆。
@Scope - 用于配置 spring bean 的范围。
@Configuration，@ComponentScan 和 @Bean - 用于基于 java 的配置。
@Aspect，@Before，@After，@Around，@Pointcut - 用于切面编程（AOP）



### DispatcherServlet

Spring的MVC框架是围绕DispatcherServlet来设计的，它用来处理所有的HTTP请求和响应。



### @Component, @Controller, @Repository, @Service 有何区别？

**@Component：** 这将 java 类标记为 bean。它是任何 Spring 管理组件的通用构造型。spring 的组件扫描机制现在可以将其拾取并将其拉入应用程序环境中。
**@Controller：** 这将一个类标记为 Spring Web MVC 控制器。标有它的 Bean 会自动导入到 IoC 容器中。
**@Service： **此注解是组件注解的特化。它不会对 @Component 注解提供任何其他行为。您可以在服务层类中使用 @Service 而不是 @Component，因为它以更好的方式指定了意图。
**@Repository：** 这个注解是具有类似用途和功能的 @Component 注解的特化。它为 DAO 提供了额外的好处。它将 DAO 导入 IoC 容器，并使未经检查的异常有资格转换为 Spring DataAccessException。



### @Autowired 注解解释

通过类型来实现自动注入bean。和@Qualifier注解配合使用可以实现根据name注入bean。



### @Qualifier 注解解释

和@Autowired一块使用，在同一类型的bean有多个的情况下可以实现根据name注入的需求



### @Resource 注解解释

默认是根据name注入bean的，可以通过设置类型来实现通过类型来注入



### @Controller 注解

该注解表明该类扮演控制器的角色，Spring不需要你继承任何其他控制器基类或引用Servlet API。



### @RequestMapping 注解

@RequestMapping 注解用于将特定 HTTP 请求方法映射到将处理相应请求的控制器中的特定类/方法。此注解可应用于两个级别：
类级别：映射请求的 URL
方法级别：映射 URL 以及 HTTP 请求方法



###  @Required 注解有什么用？

@Required 应用于 bean 属性 setter 方法。此注解仅指示必须在配置时使用 bean 定义中的显式属性值或使用自动装配填充受影响的 bean 属性。如果尚未填充受影响的 bean 属性，则容器将抛出 BeanInitializationException。



### @Autowire和@Resource区别

| 对比项   | @Autowire                | @Resource                          |
| -------- | ------------------------ | ---------------------------------- |
| 注解来源 | Spring注解               | JDK注解(JSR-250标准注解，属于J2EE) |
| 装配方式 | 优先按类型               | 优先按名称                         |
| 属性     | required                 | name、type                         |
| 作用范围 | 字段、setter方法、构造器 | 字段、setter方法                   |



### SpringMVC中的拦截器和Servlet中的filter有什么区别？

首先最核心的一点他们的拦截侧重点是不同的，SpringMVC中的拦截器是依赖JDK的反射实现的，SpringMVC的拦截器主要是进行拦截请求，通过对Handler进行处理的时候进行拦截，先声明的拦截器中的preHandle方法会先执行，然而它的postHandle方法（他是介于处理完业务之后和返回结果之前）和afterCompletion方法却会后执行。并且Spring的拦截器是按照配置的先后顺序进行拦截的。

而Servlet的filter是基于函数回调实现的过滤器，Filter主要是针对URL地址做一个编码的事情、过滤掉没用的参数、安全校验（比较泛的，比如登录不登录之类）



### 讲讲Spring加载流程。

初始化环境—>加载配置文件—>实例化Bean—>调用Bean显示信息

首先从大的几个核心步骤来去说明，因为Spring中的具体加载过程和用到的类实在是太多了。

**1、** 首先是先从AbstractBeanFactory中去调用doGetBean（name, requiredType, final Object[] args, boolean typeCheckOnly【这个是判断进行创建bean还是仅仅用来做类型检查】）方法，然后第一步要做的就是先去对传入的参数name进行做转换，因为有可能传进来的name=“&XXX”之类，需要去除&符号

**2、** 然后接着是去调用getSingleton（）方法，其实在上一个面试题中已经提到了这个方法，这个方法就是利用“三级缓存” 来去避免循环依赖问题的出现的。【这里补充一下，只有在是单例的情况下才会去解决循环依赖问题】

**3、** 对从缓存中拿到的bean其实是最原始的bean，还未长大，所以这里还需要调用getObjectForBeanInstance（Object beanInstance, String name, String beanName, RootBeanDefinition mbd）方法去进行实例化。

**4、** 然后会解决单例情况下尝试去解决循环依赖，如果isPrototypeCurrentlyInCreation（beanName）返回为true的话，会继续下一步，否则throw new BeanCurrentlyInCreationException(beanName);

**5、** 因为第三步中缓存中如果没有数据的话，就直接去parentBeanFactory中去获取bean，然后判断containsBeanDefinition（beanName）中去检查已加载的XML文件中是否包含有这样的bean存在，不存在的话递归去getBean（）获取，如果没有继续下一步

**6、** 这一步是吧存储在XML配置文件中的GernericBeanDifinition转换为RootBeanDifinition对象。这里主要进行一个转换，如果父类的bean不为空的话，会一并合并父类的属性

**7、** 这一步核心就是需要跟这个Bean有关的所有依赖的bean都要被加载进来，通过刚刚的那个RootBeanDifinition对象去拿到所有的beanName,然后通过registerDependentBean（dependsOnBean, beanName）注册bean的依赖

**8、** 然后这一步就是会根据我们在定义bean的作用域的时候定义的作用域是什么，然后进行判断在进行不同的策略进行创建（比如isSingleton、isPrototype）

**9、** 这个是最后一步的类型装换，会去检查根据需要的类型是否符合bean的实际类型去做一个类型转换。Spring中提供了许多的类型转换器



### Spring的IOC理解：

**1、** IOC就是控制反转，是指创建对象的控制权的转移，以前创建对象的主动权和时机是由自己把控的，而现在这种权力转移到Spring容器中，并由容器根据配置文件去创建实例和管理各个实例之间的依赖关系，对象与对象之间松散耦合，也利于功能的复用。DI依赖注入，和控制反转是同一个概念的不同角度的描述，即 应用程序在运行时依赖IoC容器来动态注入对象需要的外部资源。



**2、** 最直观的表达就是，IOC让对象的创建不用去new了，可以由spring自动生产，使用java的反射机制，根据配置文件在运行时动态的去创建对象以及管理对象，并调用对象的方法的。



**3、** Spring的IOC有三种注入方式 ：构造器注入、setter方法注入、根据注解注入。



IoC让相互协作的组件保持松散的耦合，而AOP编程允许你把遍布于应用各层的功能分离出来形成可重用的功能组件。



### 列举 IoC 的一些好处

它将最小化应用程序中的代码量。
它将使您的应用程序易于测试，因为它不需要单元测试用例中的任何单例或 JNDI 查找机制。
它以最小的影响和最少的侵入机制促进松耦合。
它支持即时的实例化和延迟加载服务。



### Spring 中的 IoC 的实现原理就是工厂模式加反射机制。

![图片](https://mmbiz.qpic.cn/mmbiz_png/QrAhoguKjhRTWM6ibibILa5gia7nCtDDymicPFtR8WRicyBrlhqRYNYl4SGcjDBkHLmbfQPiaWosmIM0W0sJapLayiccw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### Spring通知有哪些类型？

**1、前置通知（Before advice）：** 在某连接点（join point）之前执行的通知，但这个通知不能阻止连接点前的执行（除非它抛出一个异常）。

**2、返回后通知（After returning advice）：** 在某连接点（join point）正常完成后执行的通知：例如，一个方法没有抛出任何异常，正常返回。 

**3、抛出异常后通知（After throwing advice）：** 在方法抛出异常退出时执行的通知。 

**4、后通知（After (finally) advice）：** 当某连接点退出的时候执行的通知（不论是正常返回还是异常退出）。 

**5、环绕通知（Around Advice）：** 包围一个连接点（join point）的通知，如方法调用。这是最强大的一种通知类型。 环绕通知可以在方法调用前后完成自定义的行为。它也会选择是否继续执行连接点或直接返回它们自己的返回值或抛出异常来结束执行。 环绕通知是最常用的一种通知类型。大部分基于拦截的AOP框架，例如Nanning和JBoss4，都只提供环绕通知。 



同一个aspect，不同advice的执行顺序：

**①没有异常情况下的执行顺序：**

around before advice

before advice

target method 执行

around after advice

after advice

afterReturning



**②有异常情况下的执行顺序：**

around before advice

before advice

target method 执行

around after advice

after advice

afterThrowing:异常发生

java.lang.RuntimeException: 异常发生



### 解释一下Spring AOP里面的几个名词：

**1、切面（Aspect）：** 被抽取的公共模块，可能会横切多个对象。 在Spring AOP中，切面可以使用通用类（基于模式的风格） 或者在普通类中以 @AspectJ 注解来实现。

**2、连接点（Join point）：** 指方法，在Spring AOP中，一个连接点 总是 代表一个方法的执行。 

**3、通知（Advice）：** 在切面的某个特定的连接点（Join point）上执行的动作。通知有各种类型，其中包括“around”、“before”和“after”等通知。许多AOP框架，包括Spring，都是以拦截器做通知模型， 并维护一个以连接点为中心的拦截器链。

**4、切入点（Pointcut）：** 切入点是指 我们要对哪些Join point进行拦截的定义。通过切入点表达式，指定拦截的方法，比如指定拦截add*、search*。

**5、引入（Introduction）：**（也被称为内部类型声明（inter-type declaration））。声明额外的方法或者某个类型的字段。Spring允许引入新的接口（以及一个对应的实现）到任何被代理的对象。例如，你可以使用一个引入来使bean实现 IsModified 接口，以便简化缓存机制。

**6、目标对象（Target Object）：** 被一个或者多个切面（aspect）所通知（advise）的对象。也有人把它叫做 被通知（adviced） 对象。 既然Spring AOP是通过运行时代理实现的，这个对象永远是一个 被代理（proxied） 对象。

**7、织入（Weaving）：** 指把增强应用到目标对象来创建新的代理对象的过程。Spring是在运行时完成织入。



切入点（pointcut）和连接点（join point）匹配的概念是AOP的关键，这使得AOP不同于其它仅仅提供拦截功能的旧技术。 切入点使得定位通知（advice）可独立于OO层次。 例如，一个提供声明式事务管理的around通知可以被应用到一组横跨多个对象中的方法上（例如服务层的所有业务操作）。



### **Spring AOP的实现原理。**

AOP（Aspect-OrientedProgramming，面向方面编程）：是OOP的补充和完善。OOP引入了封装、继承、多态性等建立一种对象层次结构（从上到下的关系）。当需要为分散的对象引入公共行为的时候（从左到右的关系），OOP就显得无能为力。例如：日志功能。日志代码往往水平的散步所有对象层次中，与对象的核心功能毫无关系。这种代码被称为横切（cross-cutting）代码还有像安全性、异常处理、透明的持续性等都称为横切代码。在OOP设计中，它们导致了大量代码的重复，不利于模块的重用。

AOP与OOP相反，利用“横切”技术将影响多个类的公共行为封装到一个可重用模块，称为Aspect。简单点，就是将那些与业务无关，却被业务模块所共同调用的逻辑封装起来，便于减少系统的重复代码，降低模块间的耦合度，并有利于未来的可操作性和可维护性。AOP的核心思想就是“将应用程序中的商业逻辑同对其提供支持的通用服务进行分离。”  Spring提供了两种方式生成代理对象：JDKProxy和Cglib具体使用哪种方式生成由AopProxyFactory根据AdvisedSupport对象的配置来决定。默认的策略是如果目标类是接口，则使用JDK动态代理技术，否则使用Cglib来生成代理。



### 在Spring AOP 中，关注点和横切关注的区别是什么？

关注点是应用中一个模块的行为，一个关注点可能会被定义成一个我们想实现的一个功能。

横切关注点是一个关注点，此关注点是整个应用都会使用的功能，并影响整个应用，比如日志，安全和数据传输，几乎应用的每个模块都需要的功能。因此这些都属于横切关注点。



### Spring中AOP的底层是怎么实现的？

**Spring中AOP底层的实现其实是基于JDK的动态代理和cglib动态创建类进行动态代理来实现的:**

1、第一种基于JDK的动态代理的原理是：

需要用到的几个关键成员 InvocationHandler （你想要通过动态代理生成的对象都必须实现这个接口） 真实的需要代理的对象（帮你代理的对象） Proxy对象（是JDK中java.lang.reflect包下的）

下面是具体如何动态利用这三个组件生成代理对象

- 首先你的真是要代理的对象必须要实现InvocationHandler 这个接口，并且覆盖这个接口的invoke(Object proxyObject, Method method, Object[] args)方法，这个Invoker中方法的参数的proxyObject就是你要代理的真实目标对象，方法调用会被转发到该类的invoke()方法， method是真实对象中调用方法的Method类，Object[] args是真实对象中调用方法的参数

- 然后通过Proxy类去调用newProxyInstance(classLoader, interfaces, handler)方法，classLoader是指真实代理对象的类加载器,interfaces是指真实代理对象需要实现的接口，还可以同时指定多个接口，handler方法调用的实际处理者（其实就是帮你代理的那个对象），代理对象的方法调用都会转发到这里，然后直接就能生成你想要的对象类了。



### Spring事务的实现方式和实现原理：

Spring事务的本质其实就是数据库对事务的支持，没有数据库的事务支持，spring是无法提供事务功能的。真正的数据库层的事务提交和回滚是通过binlog或者redo log实现的。



**1、Spring事务的种类：**

spring支持编程式事务管理和声明式事务管理两种方式：

①编程式事务管理使用TransactionTemplate。

②声明式事务管理建立在AOP之上的。其本质是通过AOP功能，对方法前后进行拦截，将事务处理的功能编织到拦截的方法中，也就是在目标方法开始之前加入一个事务，在执行完目标方法之后根据执行情况提交或者回滚事务。

声明式事务最大的优点就是不需要在业务逻辑代码中掺杂事务管理的代码，只需在配置文件中做相关的事务规则声明或通过@Transactional注解的方式，便可以将事务规则应用到业务逻辑中。

声明式事务管理要优于编程式事务管理，这正是spring倡导的非侵入式的开发方式，使业务代码不受污染，只要加上注解就可以获得完全的事务支持。唯一不足地方是，最细粒度只能作用到方法级别，无法做到像编程式事务那样可以作用到代码块级别。



**2、spring的事务传播行为：**

spring事务的传播行为说的是，当多个事务同时存在的时候，spring如何处理这些事务的行为。

① PROPAGATION_REQUIRED：如果当前没有事务，就创建一个新事务，如果当前存在事务，就加入该事务，该设置是最常用的设置。

② PROPAGATION_SUPPORTS：支持当前事务，如果当前存在事务，就加入该事务，如果当前不存在事务，就以非事务执行。‘

③ PROPAGATION_MANDATORY：支持当前事务，如果当前存在事务，就加入该事务，如果当前不存在事务，就抛出异常。

④ PROPAGATION_REQUIRES_NEW：创建新事务，无论当前存不存在事务，都创建新事务。

⑤ PROPAGATION_NOT_SUPPORTED：以非事务方式执行操作，如果当前存在事务，就把当前事务挂起。

⑥ PROPAGATION_NEVER：以非事务方式执行，如果当前存在事务，则抛出异常。

⑦ PROPAGATION_NESTED：如果当前存在事务，则在嵌套事务内执行。如果当前没有事务，则按REQUIRED属性执行。



**3、Spring中的隔离级别：**

① ISOLATION_DEFAULT：这是个 PlatfromTransactionManager 默认的隔离级别，使用数据库默认的事务隔离级别。

② ISOLATION_READ_UNCOMMITTED：读未提交，允许另外一个事务可以看到这个事务未提交的数据。

③ ISOLATION_READ_COMMITTED：读已提交，保证一个事务修改的数据提交后才能被另一事务读取，而且能看到该事务对已有记录的更新。

④ ISOLATION_REPEATABLE_READ：可重复读，保证一个事务修改的数据提交后才能被另一事务读取，但是不能看到该事务对已有记录的更新。

⑤ ISOLATION_SERIALIZABLE：一个事务在执行的过程中完全看不到其他事务对数据库所做的更新。





### 讲讲Spring事务的传播属性。

**1、 **PROPAGATION_REQUIRED,那么由于执行ServiceA.methodA的时候，ServiceA.methodA已经起了事务，这时调用ServiceB.methodB，ServiceB.methodB看到自己已经运行在ServiceA.methodA的事务内部，就不再起新的事务。而假如ServiceA.methodA运行的时候发现自己没有在事务中，他就会为自己分配一个事务。这样，在ServiceA.methodA或者在ServiceB.methodB内的任何地方出现异常，事务都会被回滚。即使ServiceB.methodB的事务已经被提交，但是ServiceA.methodA在接下来fail要回滚，ServiceB.methodB也要回滚。  

**2、** PROPAGATION_SUPPORTS —— 支持当前事务，如果当前没有事务，就以非事务方式执行。  

**3、 **PROPAGATION_MANDATORY ——支持当前事务，如果当前没有事务，就抛出异常。  

**4、 **PROPAGATION_REQUIRES_NEW ——支持当前事务，如果当前没有事务，就将当前事务挂起。如ServiceA.methodA的事务级别为PROPAGATION_REQUIRED，ServiceB.methodB的事务级别为PROPAGATION_REQUIRES_NEW，那么当执行到ServiceB.methodB的时候，ServiceA.methodA所在的事务就会挂起，ServiceB.methodB会起一个新的事务，等待ServiceB.methodB的事务完成以后，A才继续执行。他与PROPAGATION_REQUIRED的事务区别在于事务的回滚程度了。因为ServiceB.methodB是新起一个事务，那么就是存在两个不同的事务。如果ServiceB.methodB已经提交，那么ServiceA.methodA失败回滚，ServiceB.methodB是不会回滚的。如果ServiceB.methodB失败回滚，如果他抛出的异常被ServiceA.methodA捕获，ServiceA.methodA事务仍然可能提交。  

**5、 **PROPAGATION_NOT_SUPPORTED —— 以非事务方式执行当前操作，如果当前存在事务，就把事务挂起来。 /

**6、** PROPAGATION_NEVER —— 以非事务方式执行，如果当前存在事务，则抛异常。  

**7、 ** PROPAGATION_NESTED—— 如果当前存在事务，则在嵌套事务内执行，关键是savepoint。如果当前没有事务，则进行与PROPAGATION_REQUIRED类似的操作。与PROPAGATION_REQUIRES_NEW的区别是NESTED的事务和他的父事务是相依的，它的提交是要等父事务一块提交。也就是说，如果父事务最后回滚，它也要回滚。



### Spring如何管理事务的

Spring事务管理主要包括3个接口，Spring事务主要由以下三个共同完成的：  

**1、PlatformTransactionManager：** 事务管理器，主要用于平台相关事务的管理。主要包括三个方法：①、commit：事务提交。②、rollback：事务回滚。③、getTransaction：获取事务状态。

**2、TransacitonDefinition：** 事务定义信息，用来定义事务相关属性，给事务管理器PlatformTransactionManager使用这个接口有下面四个主要方法：①、getIsolationLevel：获取隔离级别。②、getPropagationBehavior：获取传播行为。③、getTimeout获取超时时间。④、isReadOnly：是否只读（保存、更新、删除时属性变为false--可读写，查询时为true--只读）事务管理器能够根据这个返回值进行优化，这些事务的配置信息，都可以通过配置文件进行配置。

**3、TransationStatus： ** 事务具体运行状态，事务管理过程中，每个时间点事务的状态信息。例如：①、hasSavepoint()：返回这个事务内部是否包含一个保存点。②、isCompleted()：返回该事务是否已完成，也就是说，是否已经提交或回滚。③、isNewTransaction()：判断当前事务是否是一个新事务。



### Spring框架的事务管理有哪些优点？

它为不同的事务API 如 JTA，JDBC，Hibernate，JPA 和JDO，提供一个不变的编程模式。 它为编程式事务管理提供了一套简单的API而不是一些复杂的事务API如它为编程式事务管理提供了一套简单的API而不是一些复杂的事务API如 它支持声明式事务管理。它支持声明式事务管理。 它和Spring各种数据访问抽象层很好得集成。它和Spring各种数据访问抽象层很好得集成。



### 怎样用注解的方式配置Spring？

1.**配置文件中开启扫描**

```xml
<beans xmlns="http://www.springframework.org/schema/beans"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:p="http://www.springframework.org/schema/p"
	xmlns:context="http://www.springframework.org/schema/context"
	xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd
		http://www.springframework.org/schema/context http://www.springframework.org/schema/context/spring-context-4.3.xsd">
	<!-- 开启注解 配置扫描路径 -->
	<context:component-scan base-package="com.dpb.javabean"/>
	<!-- 如果有多个路径 ,号隔开 
		<context:component-scan base-package="com.dpb.javabean,com.dpb.factory"/>
	-->
</beans>

```

**2.加载容器**

如果是web项目的话，在web.xml文件添加如下配置:

```xml
 <context-param>
     <param-name>contextConfigLocation</param-name>
     <param-value>classpath:applicationContext.xml</param-value>
 </context-param>

 <listener>
     <listener-class>org.springframework.web.context.ContextLoaderListener</listener-class>
 </listener>

```

如果是java项目可以通过BeanFactory或ApplicationContext来直接加载Spring容器

```xml
BeanFactory bf = 
	new XmlBeanFactory(new ClassPathResource("applicationContext.xml"));
// 或者
ApplicationContext = 
	new ClassPathXmlApplicationContext("applicationContext.xml");
```



### Spring怎么配置事务（具体说出一些关键的xml 元素）。

配置事务的方法有两种：

**1、基于XML的事务配置。**

```java
<?xml version="1.0" encoding="UTF-8"?>
<!-- from the file 'context.xml' -->  
<beans xmlns="http://www.springframework.org/schema/beans"  
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"  
     xmlns:aop="http://www.springframework.org/schema/aop"  
     xmlns:tx="http://www.springframework.org/schema/tx"  
     xsi:schemaLocation="  
     http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans-2.5.xsd  
     http://www.springframework.org/schema/tx http://www.springframework.org/schema/tx/spring-tx-2.5.xsd  
     http://www.springframework.org/schema/aop http://www.springframework.org/schema/aop/spring-aop-2.5.xsd">  
      
  <!-- 数据元信息 -->  
  <bean id="dataSource" class="org.apache.commons.dbcp.BasicDataSource" destroy-method="close">  
  	<property name="driverClassName" value="oracle.jdbc.driver.OracleDriver"/>  
  	<property name="url" value="jdbc:oracle:thin:@rj-t42:1521:elvis"/>  
  	<property name="username" value="root"/>  
  	<property name="password" value="root"/>  
  </bean>  
  
  <!-- 管理事务的类,指定我们用谁来管理我们的事务-->  
  <bean id="txManager" class="org.springframework.jdbc.datasource.DataSourceTransactionManager">  
  	<property name="dataSource" ref="dataSource"/>  
  </bean>   
  
  <!-- 首先我们要把服务对象声明成一个bean  例如HelloService -->  
  <bean id="helloService" class="com.yintong.service.HelloService"/>  
  
  <!-- 然后是声明一个事物建议tx:advice,spring为我们提供了事物的封装，这个就是封装在了<tx:advice/>中 -->
  <!-- <tx:advice/>有一个transaction-manager属性，我们可以用它来指定我们的事物由谁来管理。
      默认：事务传播设置是 REQUIRED，隔离级别是DEFAULT -->
  <tx:advice id="txAdvice" transaction-manager="txManager">  
	  <!-- 配置这个事务建议的属性 -->  
	  <tx:attributes>  
	    <!-- 指定所有get开头的方法执行在只读事务上下文中 -->  
	    <tx:method name="get*" read-only="true"/>  
	    <!-- 其余方法执行在默认的读写上下文中 -->  
	    <tx:method name="*"/>  
	  </tx:attributes>  
  </tx:advice>  
    
  <!-- 我们定义一个切面，它匹配FooService接口定义的所有操作 -->  
  <aop:config>  
	 <!-- <aop:pointcut/>元素定义AspectJ的切面表示法，这里是表示com.yintong.service.helloService包下的任意方法。 -->
 	 <aop:pointcut id="helloServiceOperation" expression="execution(* com.yintong.service.helloService.*(..))"/>  
	 <!-- 然后我们用一个通知器：<aop:advisor/>把这个切面和tx:advice绑定在一起，表示当这个切面：fooServiceOperation执行时tx:advice定义的通知逻辑将被执行 -->
  	 <aop:advisor advice-ref="txAdvice" pointcut-ref="helloServiceOperation"/>  
  </aop:config>  
 
</beans>  

```

**2、基于注解方式的事务配置。**

@Transactional：直接在Java源代码中声明事务的做法让事务声明和将受其影响的代码距离更近了，而且一般来说不会有不恰当的耦合的风险，因为，使用事务性的代码几乎总是被部署在事务环境中。

```java
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"  
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"  
     xmlns:aop="http://www.springframework.org/schema/aop"  
     xmlns:tx="http://www.springframework.org/schema/tx"  
     xsi:schemaLocation="  
     http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans-2.5.xsd  
     http://www.springframework.org/schema/tx http://www.springframework.org/schema/tx/spring-tx-2.5.xsd  
     http://www.springframework.org/schema/aop http://www.springframework.org/schema/aop/spring-aop-2.5.xsd">  
    
  <bean id="helloService" class="com.yintong.service.HelloService"/>  
  <bean id="txManager" class="org.springframework.jdbc.datasource.DataSourceTransactionManager">  
     <property name="dataSource" ref="dataSource"/>  
  </bean>
  <!-- 配置注解事务 -->  
  <tx:annotation-driven transaction-manager="txManager"/>  
</beans>

```

主要在类中定义事务注解@Transactional，如下：

```java
//@Transactional 注解可以声明在类上，也可以声明在方法上。在大多数情况下，方法上的事务会首先执行
@Transactional(readOnly = true)    
public class HelloService{  
    public Foo getFoo(String fooName) {  
    }  
    //@Transactional 注解的事务设置将优先于类级别注解的事务设置   propagation:可选的传播性设置 
    @Transactional(readOnly = false, propagation = Propagation.REQUIRES_NEW)      
    public void updateFoo(Hel hel) {
    }
}  

```





### Springbean的生命周期

![](https://gitee.com/gsjqwyl/images_repo/raw/master/2021-3-11/20210328192251.png)

通过这张图能大致看懂spring的生命周期，详解：

首先会先进行实例化bean对象 然后是进行对bean的一个属性进行设置 接着是对BeanNameAware（其实就是为了让Spring容器来获取bean的名称）、BeanFactoryAware（让bean的BeanFactory调用容器的服务）、ApplicationContextAware（让bean当前的applicationContext可以来取调用Spring容器的服务） 

然后是实现BeanPostProcessor 这个接口中的两个方法，主要是对调用接口的前置初始化postProcessBeforeInitialization 这里是主要是对xml中自己定义的初始化方法 init-method = “xxxx”进行调用 然后是继续对BeanPostProcessor 这个接口中的后置初始化方法进行一个调用postProcessAfterInitialization（） 其实到这一步，基本上这个bean的初始化基本已经完成，就处于就绪状态 然后就是当Spring容器中如果使用完毕的话，就会调用destory（）方法 最后会去执行我们自己定义的销毁方法来进行销毁，然后结束生命周期。



### Spring容器的bean什么时候被实例化？

**1、** 如果你使用BeanFactory作为Spring Bean的工厂类，则所有的bean都是在第一次使用该Bean的时候实例化 

**2、** 如果你使用ApplicationContext作为Spring Bean的工厂类，则又分为以下几种情况： 如果bean的scope是singleton的，并且lazy-init为false（默认是false，所以可以不用设置），则 ApplicationContext启动的时候就实例化该Bean，并且将实例化的Bean放在一个map结构的缓存中，下次再使 用该 Bean的时候，直接从这个缓存中取 如果bean的scope是singleton的，并且lazy-init为true，则该Bean的实例化是在第一次使用该Bean的时候进行实例化。 如果bean的scope是prototype的，则该Bean的实例化是在第一次使用该Bean的时候进行实例化。




### 说说 BeanFactory 和 ApplicationContext 的区别？ 什么是延迟实例化，它的优缺点是什么？

 BeanFactory和ApplicationContext是Spring的两大核心接口，都可以当做Spring的容器。其中ApplicationContext是BeanFactory的子接口。

1、BeanFactory：是Spring里面最底层的接口，包含了各种Bean的定义，读取bean配置文档，管理bean的加载、实例化，控制bean的生命周期，维护bean之间的依赖关系。ApplicationContext接口作为BeanFactory的派生，除了提供BeanFactory所具有的功能外，还提供了更完整的框架功能：

- 继承MessageSource，因此支持国际化。
- 统一的资源文件访问方式。
- 提供在监听器中注册bean的事件。
- 同时加载多个配置文件。
- 载入多个（有继承关系）上下文 ，使得每一个上下文都专注于一个特定的层次，比如应用的web层。



**2、**

- BeanFactroy采用的是延迟加载形式来注入Bean的，即只有在使用到某个Bean时(调用getBean())，才对该Bean进行加载实例化。这样，我们就不能发现一些存在的Spring的配置问题。如果Bean的某一个属性没有注入，BeanFacotry加载后，直至第一次使用调用getBean方法才会抛出异常。
- ApplicationContext，它是在容器启动时，一次性创建了所有的Bean。这样，在容器启动时，我们就可以发现Spring中存在的配置错误，这样有利于检查所依赖属性是否注入。 ApplicationContext启动后预载入所有的单实例Bean，通过预载入单实例bean ,确保当你需要的时候，你就不用等待，因为它们已经创建好了。
- 相对于基本的BeanFactory，ApplicationContext 唯一的不足是占用内存空间。当应用程序配置Bean较多时，程序启动较慢。
- BeanFactory通常以编程的方式被创建，ApplicationContext还能以声明的方式创建，如使用ContextLoader。
- BeanFactory和ApplicationContext都支持BeanPostProcessor、BeanFactoryPostProcessor的使用，但两者之间的区别是：BeanFactory需要手动注册，而ApplicationContext则是自动注册。








###  BeanFactory – BeanFactory 实现举例

Bean 工厂是工厂模式的一个实现，提供了控制反转功能，用来把应用的配置和依赖从正真的应用代码中分离。

最常用的BeanFactory 实现是XmlBeanFactory 类。



### XMLBeanFactory

最常用的就是org.springframework.beans.factory.xml.XmlBeanFactory ，它根据XML文件中的定义加载beans。该容器从XML 文件读取配置元数据并用它去创建一个完全配置的系统或应用。



### Spring中Bean的作用域有哪些？

**singleton作用域**

在默认情况下,spring的ApplicationContext容器在启动时,自动实例化所有singleton的Bean并缓存于容器中.虽然启动时会花费一些时间,但带来两个好处:首先对Bean提前的实例化操作会及早发现一些潜在的配置问题.其次Bean以缓存的方式保存,当运行时使用到该Bean时就无须再实例化了,加快了运行效率.如果用户不希望在容器启动时提前实例化singleton的Bean,可以通过lazy-init属性进行控制.

**prototype**

在默认情况下,spring容器在启动时不实例化prototype的Bean.此外,spring容器将prototype的Bean交给调用者后,就不再管理它的生命周期.

**request作用域**

每次HTTP请求都会创建一个新的Bean,HTTP请求处理完毕后,销毁这个Bean.该作用域仅适用于webApplicationContext环境.

**session作用域**

同一个HTTP session共享一个Bean,不同HTTP session使用不同的Bean,当HTTP Session结束后,实例才被销毁.该作用域仅适用于webApplicationContext环境

**globalSession作用域**

同一个全局session共享一个Bean,一般用于portlet应用环境,该作用域仅适用于webApplicationContext环境.





