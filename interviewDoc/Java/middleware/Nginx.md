**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

**所有问题以及答案，我都整理成了高清PDF，并且带目录：[Java面试整理高清PDF下载](https://gitee.com/tiger-a/java-interview/blob/master/interviewDoc/Java/index.md)**

<!-- TOC -->

 - [请解释一下什么是`Nginx`?](#请解释一下什么是nginx)
 - [什么是正向代理和反向代理？](#什么是正向代理和反向代理)
 - [为什么要用Nginx？](#为什么要用nginx)
 - [为什么Nginx性能这么高？](#为什么nginx性能这么高)
 - [使用“反向代理服务器的优点是什么?](#使用反向代理服务器的优点是什么)
 - [Nginx怎么处理请求的？](#nginx怎么处理请求的)
 - [请列举`Nginx`的一些特性。](#请列举nginx的一些特性)
 - [请列举Nginx和Apache 之间的不同点](#请列举nginx和apache-之间的不同点)
 - [Nginx的优缺点？](#nginx的优缺点)
 - [使用“反向代理服务器”的优点是什么?](#使用反向代理服务器的优点是什么)
 - [Nginx常用变量](#nginx常用变量)
 - [请解释 Nginx 如何处理 HTTP 请求？](#请解释-nginx-如何处理-http-请求)
 - [请列举Nginx服务器的最佳用途。](#请列举nginx服务器的最佳用途)
 - [请解释Nginx服务器上的Master和Worker进程分别是什么?](#请解释nginx服务器上的master和worker进程分别是什么)
 - [请解释代理设计中的正向代理和反向代理](#请解释代理设计中的正向代理和反向代理)
 - [请解释是否有可能将Nginx的错误替换为502错误、503?](#请解释是否有可能将nginx的错误替换为502错误503)
 - [在Nginx中，解释如何在URL中保留双斜线?](#在nginx中解释如何在url中保留双斜线)
 - [Nginx 常用命令？](#nginx-常用命令)
 - [fastcgi 与 cgi 的区别？](#fastcgi-与-cgi-的区别)
 - [请解释Nginx如何处理HTTP请求。](#请解释nginx如何处理http请求)
 - [为什么Nginx性能这么高？](#为什么nginx性能这么高)
 - [长连接和短连接区别](#长连接和短连接区别)
 - [HTTP和HTTPS的区别](#http和https的区别)
 - [Nginx负载均衡的规则有哪些](#nginx负载均衡的规则有哪些)
 - [在Nginx中，如何使用未定义的服务器名称来阻止处理请求?](#在nginx中如何使用未定义的服务器名称来阻止处理请求)
 - [Nginx应用场景？](#nginx应用场景)
 - [请解释Nginx服务器上的Master和Worker进程分别是什么?](#请解释nginx服务器上的master和worker进程分别是什么)
 - [请解释你如何通过不同于80的端口开启Nginx?](#请解释你如何通过不同于80的端口开启nginx)
 - [Nginx负载均衡的算法怎么实现的?策略有哪些?](#nginx负载均衡的算法怎么实现的策略有哪些)
 - [Nginx配置高可用性怎么配置？](#nginx配置高可用性怎么配置)
 - [Nginx怎么判断IP不可访问？](#nginx怎么判断ip不可访问)
 - [如果访问的ip地址为192.168.9.115,则返回403](#如果访问的ip地址为1921689115则返回403)
 - [如果访问的ip地址为192.168.9.115,则返回403](#如果访问的ip地址为1921689115则返回403)
  - [怎么限制浏览器访问？](#怎么限制浏览器访问)
    - [解释Nginx是否支持将请求压缩到上游?](#解释nginx是否支持将请求压缩到上游)
    - [Nginx目录结构有哪些？](#nginx目录结构有哪些)
    - [Nginx配置文件nginx.conf有哪些属性模块?](#nginx配置文件nginxconf有哪些属性模块)
    - [为什么Nginx性能这么高？](#为什么nginx性能这么高)
    - [Nginx静态资源?](#nginx静态资源)
    - [如何用Nginx解决前端跨域问题？](#如何用nginx解决前端跨域问题)
    - [Nginx怎么处理请求的？](#nginx怎么处理请求的)
    - [Nginx虚拟主机怎么配置?](#nginx虚拟主机怎么配置)
  - [location的作用是什么？](#location的作用是什么)
  - [Location正则案例](#location正则案例)
  - [Nginx常用变量](#nginx常用变量)
  - [Nginx设置重定向](#nginx设置重定向)
  - [限流怎么做的？](#限流怎么做的)
  - [为什么要做动静分离？](#为什么要做动静分离)
  - [Nginx怎么做的动静分离？](#nginx怎么做的动静分离)
  - [LVS、Nginx、HAproxy 有什么区别？](#lvsnginxhaproxy-有什么区别)
  - [Nginx条件判断](#nginx条件判断)

<!-- /TOC -->


### **请解释一下什么是`Nginx`?**

Nginx---Ngine X，是一款免费的、自由的、开源的、高性能HTTP服务器和反向代理服务器；也是一个IMAP、POP3、SMTP代理服务器；Nginx以其高性能、稳定性、丰富的功能、简单的配置和低资源消耗而闻名。

也就是说Nginx本身就可以托管网站（类似于Tomcat一样），进行Http服务处理，也可以作为反向代理服务器 、负载均衡器和HTTP缓存。

Nginx 解决了服务器的C10K（就是在一秒之内连接客户端的数目为10k即1万）问题。它的设计不像传统的服务器那样使用线程处理请求，而是一个更加高级的机制—事件驱动机制，是一种异步事件驱动结构。



### 什么是正向代理和反向代理？

- 正向代理就是一个人发送一个请求直接就到达了目标的服务器
- 反方代理就是请求统一被Nginx接收，nginx反向代理服务器接收到之后，按照一定的规则分发给了后端的业务处理服务器进行处理了



### 为什么要用Nginx？

跨平台、配置简单、方向代理、高并发连接：处理2-3万并发连接数，官方监测能支持5万并发，内存消耗小：开启10个nginx才占150M内存 ，nginx处理静态文件好，耗费内存少，

而且Nginx内置的健康检查功能：如果有一个服务器宕机，会做一个健康检查，再发送的请求就不会发送到宕机的服务器了。重新将请求提交到其他的节点上。

使用Nginx的话还能：

- 节省宽带：支持GZIP压缩，可以添加浏览器本地缓存
- 稳定性高：宕机的概率非常小
- 接收用户请求是异步的



### 为什么Nginx性能这么高？

因为他的事件处理机制：异步非阻塞事件处理机制：运用了epoll模型，提供了一个队列，排队解决



### 使用“反向代理服务器的优点是什么?

反向代理服务器可以隐藏源服务器的存在和特征。它充当互联网云和web服务器之间的中间层。这对于安全方面来说是很好的，特别是当您使用web托管服务时。



### Nginx怎么处理请求的？

nginx接收一个请求后，首先由listen和server_name指令匹配server模块，再匹配server模块里的location，location就是实际地址

```
    server {                            # 第一个Server区块开始，表示一个独立的虚拟主机站点
        listen       80；                      # 提供服务的端口，默认80
        server_name  localhost；            # 提供服务的域名主机名
        location / {                        # 第一个location区块开始
            root   html；               # 站点的根目录，相当于Nginx的安装目录
            index  index.html index.htm；        # 默认的首页文件，多个用空格分开
        }                          # 第一个location区块结果
    }           
```



### **请列举`Nginx`的一些特性。**

- 跨平台：可以在大多数Unix like 系统编译运行。而且也有Windows的移植版本。 
- 配置异常简单：非常的简单，易上手。 
- 非阻塞、高并发连接：数据复制时，磁盘I/O的第一阶段是非阻塞的。官方测试能支持5万并发连接，实际生产中能跑2~3万并发连接数（得益于Nginx采用了最新的epoll事件处理模型（消息队列）。 
- Nginx代理和后端Web服务器间无需长连接； 
- Nginx接收用户请求是异步的，即先将用户请求全部接收下来，再一次性发送到后端Web服务器，极大减轻后端Web服务器的压力。 
- 发送响应报文时，是边接收来自后端Web服务器的数据，边发送给客户端。 
- 网络依赖性低，理论上只要能够ping通就可以实施负载均衡，而且可以有效区分内网、外网流量。 
- 支持内置服务器检测。Nginx能够根据应用服务器处理页面返回的状态码、超时信息等检测服务器是否出现故障，并及时返回错误的请求重新提交到其它节点上。 
- 此外还有内存消耗小、成本低廉（比F5硬件负载均衡器廉价太多）、节省带宽、稳定性高等特点。



### 请列举Nginx和Apache 之间的不同点

![img](http://static.iocoder.cn/7bdf14ce3d607e5765e37750cc49d65f)



### Nginx的优缺点？

**优点：**

- 占内存小，可实现高并发连接，处理响应快
- 可实现http服务器、虚拟主机、方向代理、负载均衡
- Nginx配置简单
- 可以不暴露正式的服务器IP地址

**缺点：**

- 动态处理差：nginx处理静态文件好,耗费内存少，但是处理动态页面则很鸡肋，现在一般前端用nginx作为反向代理抗住压力，



### 使用“反向代理服务器”的优点是什么?

反向代理服务器可以隐藏源服务器的存在和特征。它充当互联网云和web服务器之间的中间层。这对于安全方面来说是很好的，特别是当您使用web托管服务时。



### Nginx常用变量

- $host: 请求的主机头

```
if ($host = 'bbs.gitlib.com') {
	rewrite ^/$ http://bbs.bliwan.com permanent;
}
```

- $remote_addr: 客户端IP地址
- $remote_port: 客户端端口号
- $remote_user: 已经经过Auth Basic Module验证的用户名
- $http_referer: 请求引用地址
- $http_user_agent: 客户端代理信息(UA)
- $http_x_forwarded_for: 相当于网络访问路径
- $body_bytes_sent: 页面传送的字节数
- $time_local: 服务器时间
- $request: 客户端请求
- $request_uri: 请求的URI,带参数, 不包含主机名
- $request_filename: 请求的文件路径
- $request_method: 请求的方法，如GET、POST
- $args: 客户端请求中的参数
- $query_string: 等同于$args, 客户端请求的参数
- $nginx_version: 当前nginx版本
- $status: 服务器响应状态码
- $server_addr: 服务器地址
- $server_port: 请求到达的服务器端口号
- $server_protocol: 请求的协议版本
- $content_type: HTTP请求信息里的Content-Type字段
- $content_length: HTTP请求信息里的Content-Length字段
- $uri: 请求中的当前URI(不带请求参数，参数位于$args)
- $document_root: 当前请求在root指令中指定的值
- $document_uri: 与$uri相同



### 请解释 Nginx 如何处理 HTTP 请求？

- 首先，Nginx 在启动时，会解析配置文件，得到需要监听的端口与 IP 地址，然后在 Nginx 的 Master 进程里面先初始化好这个监控的Socket(创建 S ocket，设置 addr、reuse 等选项，绑定到指定的 ip 地址端口，再 listen 监听)。
- 然后，再 fork(一个现有进程可以调用 fork 函数创建一个新进程。由 fork 创建的新进程被称为子进程 )出多个子进程出来。
- 之后，子进程会竞争 accept 新的连接。此时，客户端就可以向 nginx 发起连接了。当客户端与nginx进行三次握手，与 nginx 建立好一个连接后。此时，某一个子进程会 accept 成功，得到这个建立好的连接的 Socket ，然后创建 nginx 对连接的封装，即 ngx_connection_t 结构体。
- 接着，设置读写事件处理函数，并添加读写事件来与客户端进行数据的交换。
- 最后，Nginx 或客户端来主动关掉连接，到此，一个连接就寿终正寝了。
- 最后，Nginx 或客户端来主动关掉连接，到此，一个连接就寿终正寝了。
  



### 请列举Nginx服务器的最佳用途。

Nginx服务器的最佳用法是在网络上部署动态HTTP内容，使用SCGI、WSGI应用程序服务器、用于脚本的FastCGI处理程序。它还可以作为负载均衡器。



### 请解释Nginx服务器上的Master和Worker进程分别是什么?

- 主程序 Master process 启动后，通过一个 for 循环来 接收 和 处理外部信号 ；
- 主进程通过 fork() 函数产生 worker 子进程 ，每个子进程执行一个 for循环来实现Nginx服务器对事件的接收和处理 。

![图片](https://mmbiz.qpic.cn/mmbiz_png/UtWdDgynLdYJzfyu1L8rI8asia8NkuKt5RiajKOy5hzmpA2NxqZBqakbyVj7QtricyBia1MEgtMOkzoiaF7Z1sFc1hg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

一般推荐 worker 进程数与CPU内核数一致，这样一来不存在大量的子进程生成和管理任务，避免了进程之间竞争CPU 资源和进程切换的开销。而且 Nginx 为了更好的利用 多核特性 ，提供了 CPU 亲缘性的绑定选项，我们可以将某一个进程绑定在某一个核上，这样就不会因为进程的切换带来 Cache 的失效。

对于每个请求，有且只有一个工作进程 对其处理。首先，每个 worker 进程都是从 master进程 fork 过来。在 master 进程里面，先建立好需要 listen 的 socket（listenfd） 之后，然后再 fork 出多个 worker 进程。

所有 worker 进程的 listenfd 会在新连接到来时变得可读 ，为保证只有一个进程处理该连接，所有 worker 进程在注册 listenfd 读事件前抢占 accept_mutex ，抢到互斥锁的那个进程注册 listenfd 读事件 ，在读事件里调用 accept 接受该连接。

当一个 worker 进程在 accept 这个连接之后，就开始读取请求、解析请求、处理请求，产生数据后，再返回给客户端 ，最后才断开连接。这样一个完整的请求就是这样的了。我们可以看到，一个请求，完全由 worker 进程来处理，而且只在一个 worker 进程中处理。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/UtWdDgynLdYJzfyu1L8rI8asia8NkuKt5X9ZBNgaawiaFg1KEAwZaibXuichhPNgHTZRqXLicd2avQzMMxOTc2mBDXA/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

在 Nginx 服务器的运行过程中， 主进程和工作进程 需要进程交互。交互依赖于 Socket 实现的管道来实现。



### 请解释代理设计中的正向代理和反向代理

首先，代理服务器一般指局域网内部的机器通过代理服务器发送请求到互联网上的服务器，代理服务器一般作用在客户端。例如：GoAgent翻墙软件。我们的客户端在进行翻墙操作的时候，我们使用的正是正向代理，通过正向代理的方式，在我们的客户端运行一个软件，将我们的HTTP请求转发到其他不同的服务器端，实现请求的分发。

![图片](https://mmbiz.qpic.cn/mmbiz_png/UtWdDgynLdYJzfyu1L8rI8asia8NkuKt5vXdia1RicjhSpzVkvmOuHDVRWMcljQh60Z90cmLHFQ4Md8cJq4Kn0thg/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

反向代理服务器作用在服务器端，它在服务器端接收客户端的请求，然后将请求分发给具体的服务器进行处理，然后再将服务器的相应结果反馈给客户端。Nginx就是一个反向代理服务器软件。

![图片](https://mmbiz.qpic.cn/mmbiz_png/UtWdDgynLdYJzfyu1L8rI8asia8NkuKt5EGFQBBLqOG2wMNh27CPcndwibeMrRaQsU9q553ZkwsQaB7SNtr8aibJw/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

从上图可以看出：客户端必须设置正向代理服务器，当然前提是要知道正向代理服务器的IP地址，还有代理程序的端口。 
反向代理正好与正向代理相反，对于客户端而言代理服务器就像是原始服务器，并且客户端不需要进行任何特别的设置。客户端向反向代理的命名空间（name-space）中的内容发送普通请求，接着反向代理将判断向何处（原始服务器）转交请求，并将获得的内容返回给客户端。

![图片](https://mmbiz.qpic.cn/mmbiz_png/UtWdDgynLdYJzfyu1L8rI8asia8NkuKt5UOLvTTtAFI04Dbicmz7Cb23rjVwTia9bJicPYkhB7lSKUAO7YOzmXwE8A/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### 请解释是否有可能将Nginx的错误替换为502错误、503?

502 =错误网关

503 =服务器超载

有可能，但是您可以确保fastcgi_intercept_errors被设置为ON，并使用错误页面指令。

![图片](https://mmbiz.qpic.cn/mmbiz_png/gUFHIUJJ6iay23sEXiaRGraGvdj7G5yy6ib18waolmZ4ia4z150Baw2uBIkRickyuAXIYhQpDmuxNic4RzmccYOaJSdA/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)





### 在Nginx中，解释如何在URL中保留双斜线?

要在URL中保留双斜线，就必须使用merge_slashes_off;

语法:merge_slashes [on/off]

默认值: merge_slashes on

环境: http，server



### Nginx 常用命令？

- 启动 `nginx` 。
- 停止 `nginx -s stop` 或 `nginx -s quit` 。
- 重载配置 `./sbin/nginx -s reload`(平滑重启) 或 `service nginx reload` 。
- 重载指定配置文件 `.nginx -c /usr/local/nginx/conf/nginx.conf` 。
- 查看 nginx 版本 `nginx -v` 。
- 检查配置文件是否正确 `nginx -t` 。
- 显示帮助信息 `nginx -h` 。
  



### fastcgi 与 cgi 的区别？

**1）cgi**

web 服务器会根据请求的内容，然后会 fork 一个新进程来运行外部 c 程序（或 perl 脚本…）， 这个进程会把处理完的数据返回给 web 服务器，最后 web 服务器把内容发送给用户，刚才 fork 的进程也随之退出。

如果下次用户还请求改动态脚本，那么 web 服务器又再次 fork 一个新进程，周而复始的进行。

**2）fastcgi**

web 服务器收到一个请求时，他不会重新 fork 一个进程（因为这个进程在 web 服务器启动时就开启了，而且不会退出），web 服务器直接把内容传递给这个进程（进程间通信，但 fastcgi 使用了别的方式，tcp 方式通信），这个进程收到请求后进行处理，把结果返回给 web 服务器，最后自己接着等待下一个请求的到来，而不是退出。




### 请解释Nginx如何处理HTTP请求。

Nginx 是一个高性能的 Web 服务器，能够同时处理大量的并发请求。它结合多进程机制和异步机制 ，异步机制使用的是异步非阻塞方式 ，接下来就给大家介绍一下 Nginx 的多线程机制和异步非阻塞机制 。



**1、多进程机制**

服务器每当收到一个客户端时，就有 服务器主进程 （ master process ）生成一个 子进程（ worker process ）出来和客户端建立连接进行交互，直到连接断开，该子进程就结束了。

使用进程的好处是各个进程之间相互独立，不需要加锁，减少了使用锁对性能造成影响，同时降低编程的复杂度，降低开发成本。其次，采用独立的进程，可以让进程互相之间不会影响 ，如果一个进程发生异常退出时，其它进程正常工作， master 进程则很快启动新的 worker 进程，确保服务不会中断，从而将风险降到最低。

缺点是操作系统生成一个子进程需要进行 内存复制等操作，在资源和时间上会产生一定的开销。当有大量请求时，会导致系统性能下降 。

**2、异步非阻塞机制**

每个工作进程 使用 异步非阻塞方式 ，可以处理 多个客户端请求 。

当某个 工作进程 接收到客户端的请求以后，调用 IO 进行处理，如果不能立即得到结果，就去 处理其他请求 （即为 非阻塞 ）；而 客户端 在此期间也 无需等待响应 ，可以去处理其他事情（即为 异步 ）。

当 IO 返回时，就会通知此 工作进程 ；该进程得到通知，暂时 挂起 当前处理的事务去 响应客户端请求 。



### 为什么Nginx性能这么高？

因为他的事件处理机制：异步非阻塞事件处理机制：运用了epoll模型，提供了一个队列，排队解决



### 长连接和短连接区别

**长连接： **连接->传输数据->保持连接 -> 传输数据-> ...........->直到一方关闭连接，多是客户端关闭连接。 长连接指建立SOCKET连接后不管是否使用都保持连接，但安全性较差。

**短连接：** 连接->传输数据->关闭连接 比如HTTP是无状态的的短链接，浏览器和服务器每进行一次HTTP操作，就建立一次连接，但任务结束就中断连接。 因为连接后接收了数据就断开了，所以每次数据接受处理不会有联系。 这也是HTTP协议无状态的原因之一。



### HTTP和HTTPS的区别

- http是超文本传输协议，信息是明文传输，https则是具有安全性的加密传输协议。

- http和https使用的是完全不同的连接方式，用的端口也不一样，前者是80，后者是443。

- http的连接很简单，是无状态的；HTTPS是由SSL+HTTP协议构建的,可进行加密传输、身份认证的网络协议，比http协议安全。



### Nginx负载均衡的规则有哪些

**1、轮询（默认）**

每个请求按时间顺序逐一分配到不同的后端服务器，如果后端服务器down掉，能自动剔除

**2、指定轮询几率**

weight和访问比率成正比，用于后端服务器性能不均的情况默认选项，当weight不指定时，各服务器weight相同，数字越大，表明请求到的机会越大

**3、ip_hash**

每个请求按访问ip的hash值分配，这样同一客户端连续的Web请求都会被分发到同一服务器进行处理，可以解决session的问题。当后台服务器宕机时，会自动跳转到其它服务器。

**4、url_hash（第三方）**

nginx按访问url的hash结果来分配请求，使每个url定向到同一个后端服务器，后端服务器为缓存服务器、文件服务器、静态服务器时比较有效。缺点是当后端服务器宕机的时候，url_hash不会自动跳转的其他缓存服务器，而是返回给用户一个503错误。

**5、fair（第三方）**

按后端服务器的响应时间来分配请求，响应时间短的优先分配


### 在Nginx中，如何使用未定义的服务器名称来阻止处理请求?

只需将请求删除的服务器就可以定义为：

![图片](https://mmbiz.qpic.cn/mmbiz_png/gUFHIUJJ6iay23sEXiaRGraGvdj7G5yy6ibTl7UrMM5DQkGlNtTcrFloUSUdaUt5AiaO1icO4sC2W96Y8iaSyQvBHsJQ/640?tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

这里，服务器名被保留为一个空字符串，它将在没有“主机”头字段的情况下匹配请求，而一个特殊的Nginx的非标准代码444被返回，从而终止连接。



### Nginx应用场景？

- http服务器。Nginx是一个http服务可以独立提供http服务。可以做网页静态服务器。
- 虚拟主机。可以实现在一台服务器虚拟出多个网站，例如个人网站使用的虚拟机。
- 反向代理，负载均衡。当网站的访问量达到一定程度后，单台服务器不能满足用户的请求时，需要用多台服务器集群可以使用nginx做反向代理。并且多台服务器可以平均分担负载，不会应为某台服务器负载高宕机而某台服务器闲置的情况。
- nginz 中也可以配置安全管理、比如可以使用Nginx搭建API接口网关,对每个接口服务进行拦截。



### 请解释Nginx服务器上的Master和Worker进程分别是什么?

**Master进程：**读取及评估配置和维持

**Worker进程：**处理请求



### 请解释你如何通过不同于80的端口开启Nginx?

为了通过一个不同的端口开启Nginx，你必须进入/etc/Nginx/sites-enabled/，如果这是默认文件，那么你必须打开名为“default”的文件。编辑文件，并放置在你想要的端口：

Like server { listen 81; }



### Nginx负载均衡的算法怎么实现的?策略有哪些?

为了避免服务器崩溃，大家会通过负载均衡的方式来分担服务器压力。将对台服务器组成一个集群，当用户访问时，先访问到一个转发服务器，再由转发服务器将访问分发到压力更小的服务器。

Nginx负载均衡实现的策略有以下五种：

**1、 轮询(默认)**

每个请求按时间顺序逐一分配到不同的后端服务器，如果后端某个服务器宕机，能自动剔除故障系统。

```
upstream backserver { 
 server 192.168.0.12; 
 server 192.168.0.13; 
} 
```

**2、权重 weight**

weight的值越大分配

到的访问概率越高，主要用于后端每台服务器性能不均衡的情况下。其次是为在主从的情况下设置不同的权值，达到合理有效的地利用主机资源。

```
upstream backserver { 
 server 192.168.0.12 weight=2; 
 server 192.168.0.13 weight=8; 
} 
```

权重越高，在被访问的概率越大，如上例，分别是20%，80%。

**3、 ip_hash( IP绑定)**

每个请求按访问IP的哈希结果分配，使来自同一个IP的访客固定访问一台后端服务器，并且可以有效解决动态网页存在的session共享问题

```
upstream backserver { 
 ip_hash; 
 server 192.168.0.12:88; 
 server 192.168.0.13:80; 
} 
```



**4、 fair(第三方插件)**

必须安装upstream_fair模块。

对比 weight、ip_hash更加智能的负载均衡算法，fair算法可以根据页面大小和加载时间长短智能地进行负载均衡，响应时间短的优先分配。

```
upstream backserver { 
 server server1; 
 server server2; 
 fair; 
} 
```

哪个服务器的响应速度快，就将请求分配到那个服务器上。



**5、url_hash(第三方插件)**

必须安装Nginx的hash软件包

按访问url的hash结果来分配请求，使每个url定向到同一个后端服务器，可以进一步提高后端缓存服务器的效率。

```
upstream backserver { 
 server squid1:3128; 
 server squid2:3128; 
 hash $request_uri; 
 hash_method crc32; 
} 
```



### Nginx配置高可用性怎么配置？

当上游服务器(真实访问服务器)，一旦出现故障或者是没有及时相应的话，应该直接轮训到下一台服务器，保证服务器的高可用

Nginx配置代码：

```
server {
        listen       80;
        server_name  www.lijie.com;
        location / {
            ### 指定上游服务器负载均衡服务器
            proxy_pass http://backServer;
            ###nginx与上游服务器(真实访问的服务器)超时时间 后端服务器连接的超时时间_发起握手等候响应超时时间
            proxy_connect_timeout 1s;
            ###nginx发送给上游服务器(真实访问的服务器)超时时间
            proxy_send_timeout 1s;
            ### nginx接受上游服务器(真实访问的服务器)超时时间
            proxy_read_timeout 1s;
            index  index.html index.htm;
        }
    }
```



### Nginx怎么判断IP不可访问？

```
# 如果访问的ip地址为192.168.9.115,则返回403
if  ($remote_addr = 192.168.9.115) {  
     return 403;  
}  
```



### 怎么限制浏览器访问？

```
## 不允许谷歌浏览器访问 如果是谷歌浏览器返回500
if ($http_user_agent ~ Chrome) {   
    return 500;  
}

```



### 请解释ngx_http_upstream_module的作用是什么?

ngx_http_upstream_module用于定义可通过fastcgi传递、proxy传递、uwsgi传递、memcached传递和scgi传递指令来引用的服务器组。



### 解释Nginx是否支持将请求压缩到上游?

您可以使用Nginx模块gunzip将请求压缩到上游。gunzip模块是一个过滤器，它可以对不支持“gzip”编码方法的客户机或服务器使用“内容编码:gzip”来解压缩响应。



### Nginx目录结构有哪些？

```
[root@localhost ~]# tree /usr/local/nginx
/usr/local/nginx
├── client_body_temp
├── conf                             # Nginx所有配置文件的目录
│   ├── fastcgi.conf                 # fastcgi相关参数的配置文件
│   ├── fastcgi.conf.default         # fastcgi.conf的原始备份文件
│   ├── fastcgi_params               # fastcgi的参数文件
│   ├── fastcgi_params.default       
│   ├── koi-utf
│   ├── koi-win
│   ├── mime.types                   # 媒体类型
│   ├── mime.types.default
│   ├── nginx.conf                   # Nginx主配置文件
│   ├── nginx.conf.default
│   ├── scgi_params                  # scgi相关参数文件
│   ├── scgi_params.default  
│   ├── uwsgi_params                 # uwsgi相关参数文件
│   ├── uwsgi_params.default
│   └── win-utf
├── fastcgi_temp                     # fastcgi临时数据目录
├── html                             # Nginx默认站点目录
│   ├── 50x.html                     # 错误页面优雅替代显示文件，例如当出现502错误时会调用此页面
│   └── index.html                   # 默认的首页文件
├── logs                             # Nginx日志目录
│   ├── access.log                   # 访问日志文件
│   ├── error.log                    # 错误日志文件
│   └── nginx.pid                    # pid文件，Nginx进程启动后，会把所有进程的ID号写到此文件
├── proxy_temp                       # 临时目录
├── sbin                             # Nginx命令目录
│   └── nginx                        # Nginx的启动命令
├── scgi_temp                        # 临时目录
└── uwsgi_temp                       # 临时目录
```



### Nginx配置文件nginx.conf有哪些属性模块?

```xml
worker_processes  1；                            # worker进程的数量
events {                                          # 事件区块开始
    worker_connections  1024；                  # 每个worker进程支持的最大连接数
}                                           # 事件区块结束
http {                                       # HTTP区块开始
    include       mime.types；                     # Nginx支持的媒体类型库文件
    default_type  application/octet-stream；            # 默认的媒体类型
    sendfile        on；                       # 开启高效传输模式
    keepalive_timeout  65；                   # 连接超时
    server {                                    # 第一个Server区块开始，表示一个独立的虚拟主机站点
        listen       80；                          # 提供服务的端口，默认80
        server_name  localhost；                # 提供服务的域名主机名
        location / {                            # 第一个location区块开始
            root   html；                   # 站点的根目录，相当于Nginx的安装目录
            index  index.html index.htm；           # 默认的首页文件，多个用空格分开
        }                                  # 第一个location区块结果
        error_page   500502503504  /50x.html；          # 出现对应的http状态码时，使用50x.html回应客户
        location = /50x.html {                      # location区块开始，访问50x.html
            root   html；                              # 指定对应的站点目录为html
        }
    }  
    ......
```



### 为什么Nginx性能这么高？

因为他的事件处理机制：异步非阻塞事件处理机制：运用了epoll模型，提供了一个队列，排队解决



### Nginx静态资源?

静态资源访问，就是存放在nginx的html页面，我们可以自己编写



### 如何用Nginx解决前端跨域问题？

使用Nginx转发请求。把跨域的接口写成调本域的接口，然后将这些接口转发到真正的请求地址。



### Nginx怎么处理请求的？

nginx接收一个请求后，首先由listen和server_name指令匹配server模块，再匹配server模块里的location，location就是实际地址

```xml
    server {                            # 第一个Server区块开始，表示一个独立的虚拟主机站点
        listen       80；                      # 提供服务的端口，默认80
        server_name  localhost；            # 提供服务的域名主机名
        location / {                        # 第一个location区块开始
            root   html；               # 站点的根目录，相当于Nginx的安装目录
            index  index.html index.htm；        # 默认的首页文件，多个用空格分开
        }                          # 第一个location区块结果
    }   
```



### Nginx虚拟主机怎么配置?

**1、**基于域名的虚拟主机，通过域名来区分虚拟主机——应用：外部网站

**2、**基于端口的虚拟主机，通过端口来区分虚拟主机——应用：公司内部网站，外部网站的管理后台

**3、**基于ip的虚拟主机。

**基于虚拟主机配置域名**

需要建立/data/www /data/bbs目录，windows本地hosts添加虚拟机ip地址对应的域名解析；对应域名网站目录下新增index.html文件；

```
#当客户端访问www.lijie.com,监听端口号为80,直接跳转到data/www目录下文件
    server {
        listen       80;
        server_name  www.lijie.com;
        location / {
            root   data/www;
            index  index.html index.htm;
        }
    }

    #当客户端访问www.lijie.com,监听端口号为80,直接跳转到data/bbs目录下文件
    server {
        listen       80;
        server_name  bbs.lijie.com;
        location / {
            root   data/bbs;
            index  index.html index.htm;
        }
    }
```



**基于端口的虚拟主机**

使用端口来区分，浏览器使用域名或ip地址:端口号 访问

```
    #当客户端访问www.lijie.com,监听端口号为8080,直接跳转到data/www目录下文件
    server {
        listen       8080;
        server_name  8080.lijie.com;
        location / {
            root   data/www;
            index  index.html index.htm;
        }
    }

    #当客户端访问www.lijie.com,监听端口号为80直接跳转到真实ip服务器地址 127.0.0.1:8080
    server {
        listen       80;
        server_name  www.lijie.com;
        location / {
        proxy_pass http://127.0.0.1:8080;
                index  index.html index.htm;
        }
    }
```





### location的作用是什么？

location指令的作用是根据用户请求的URI来执行不同的应用，也就是根据用户请求的网站URL进行匹配，匹配成功即进行相关的操作

**location的语法能说出来吗？**

注意：~ 代表自己输入的英文字母

![图片](https://mmbiz.qpic.cn/mmbiz_png/8KKrHK5ic6XCsMRO2nqOkIPRzZSApnnmSFVQKNm59WSFBgV6NuDd39txkhicDA0BmQ2a6CON8ickGsJFnpRT6oEqg/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)



### **Location正则案例**

示例：

```
#优先级1,精确匹配，根路径
    location =/ {
        return 400;
    }

    #优先级2,以某个字符串开头,以av开头的，优先匹配这里，区分大小写
    location ^~ /av {
       root /data/av/;
    }

    #优先级3，区分大小写的正则匹配，匹配/media*****路径
    location ~ /media {
          alias /data/static/;
    }

    #优先级4 ，不区分大小写的正则匹配，所有的****.jpg|gif|png 都走这里
    location ~* .*\.(jpg|gif|png|js|css)$ {
       root  /data/av/;
    }

    #优先7，通用匹配
    location / {
        return 403;
    }
```



### Nginx常用变量

- $host: 请求的主机头

  ```xml
  if ($host = 'bbs.gitlib.com') {
  	rewrite ^/$ http://bbs.bliwan.com permanent;
  }
  ```

- $remote_addr: 客户端IP地址
- $remote_port: 客户端端口号
- $remote_user: 已经经过Auth Basic Module验证的用户名
- $http_referer: 请求引用地址
- $http_user_agent: 客户端代理信息(UA)
- $http_x_forwarded_for: 相当于网络访问路径
- $body_bytes_sent: 页面传送的字节数
- $time_local: 服务器时间
- $request: 客户端请求
- $request_uri: 请求的URI,带参数, 不包含主机名
- $request_filename: 请求的文件路径
- $request_method: 请求的方法，如GET、POST
- $args: 客户端请求中的参数
- $query_string: 等同于$args, 客户端请求的参数
- $nginx_version: 当前nginx版本
- $status: 服务器响应状态码
- $server_addr: 服务器地址
- $server_port: 请求到达的服务器端口号
- $server_protocol: 请求的协议版本
- $content_type: HTTP请求信息里的Content-Type字段
- $content_length: HTTP请求信息里的Content-Length字段
- $uri: 请求中的当前URI(不带请求参数，参数位于$args)
- $document_root: 当前请求在root指令中指定的值
- $document_uri: 与$uri相同



### Nginx设置重定向

**return形式**

```java
# 301永久重定向，302临时重定向
return 301 https://example.com$request_uri;
	
# return 返回形式
return code;
return code URL;
return URL;
```



**rewrite形式**

```xml
rewrite ^/$ http://bbs.gitlib.com permanent;
```



**rewrite flag说明:**

```xml
last: 停止处理后续rewrite指令集，然后对当前重写的新URI在rewrite指令集上重新查找

break: 停止处理后续rewrite指令集，并不在重新查找,但是当前location内剩余非rewrite语句和location外的非rewrite语句可以执行

redirect: 如果replacement不是以http:// 或https://开始，返回302临时重定向

permant: 返回301永久重定向
```



### 限流怎么做的？

Nginx限流就是限制用户请求速度，防止服务器受不了

限流有3种

- 正常限制访问频率（正常流量）
- 突发限制访问频率（突发流量）
- 限制并发连接数

Nginx的限流都是基于漏桶流算法，底下会说道什么是桶铜流

**实现三种限流算法**

**1、正常限制访问频率（正常流量）：**

限制一个用户发送的请求，我Nginx多久接收一个请求。

Nginx中使用ngx_http_limit_req_module模块来限制的访问频率，限制的原理实质是基于漏桶算法原理来实现的。在nginx.conf配置文件中可以使用limit_req_zone命令及limit_req命令限制单个IP的请求处理频率。

```
    #定义限流维度，一个用户一分钟一个请求进来，多余的全部漏掉
    limit_req_zone $binary_remote_addr zone=one:10m rate=1r/m;

    #绑定限流维度
    server{

        location/seckill.html{
            limit_req zone=zone;    
            proxy_pass http://lj_seckill;
        }

    }
```

1r/s代表1秒一个请求，1r/m一分钟接收一个请求， 如果Nginx这时还有别人的请求没有处理完，Nginx就会拒绝处理该用户请求。



**2、突发限制访问频率（突发流量）：**

限制一个用户发送的请求，我Nginx多久接收一个。

上面的配置一定程度可以限制访问频率，但是也存在着一个问题：如果突发流量超出请求被拒绝处理，无法处理活动时候的突发流量，这时候应该如何进一步处理呢？

Nginx提供burst参数结合nodelay参数可以解决流量突发的问题，可以设置能处理的超过设置的请求数外能额外处理的请求数。我们可以将之前的例子添加burst参数以及nodelay参数：

```
  #定义限流维度，一个用户一分钟一个请求进来，多余的全部漏掉
    limit_req_zone $binary_remote_addr zone=one:10m rate=1r/m;

    #绑定限流维度
    server{

        location/seckill.html{
            limit_req zone=zone burst=5 nodelay;
            proxy_pass http://lj_seckill;
        }

    }
```

为什么就多了一个 burst=5 nodelay; 呢，多了这个可以代表Nginx对于一个用户的请求会立即处理前五个，多余的就慢慢来落，没有其他用户的请求我就处理你的，有其他的请求的话我Nginx就漏掉不接受你的请求



**3、 限制并发连接数**

Nginx中的ngx_http_limit_conn_module模块提供了限制并发连接数的功能，可以使用limit_conn_zone指令以及limit_conn执行进行配置。接下来我们可以通过一个简单的例子来看下：

```
 http {
    limit_conn_zone $binary_remote_addr zone=myip:10m;
    limit_conn_zone $server_name zone=myServerName:10m;
    }

    server {
        location / {
            limit_conn myip 10;
            limit_conn myServerName 100;
            rewrite / http://www.lijie.net permanent;
        }
    }
```

上面配置了单个IP同时并发连接数最多只能10个连接，并且设置了整个虚拟服务器同时最大并发数最多只能100个链接。当然，只有当请求的header被服务器处理后，虚拟服务器的连接数才会计数。



### 为什么要做动静分离？

- Nginx是当下最热的Web容器，网站优化的重要点在于静态化网站，网站静态化的关键点则是是动静分离，动静分离是让动态网站里的动态网页根据一定规则把不变的资源和经常变的资源区分开来，动静资源做好了拆分以后，我们则根据静态资源的特点将其做缓存操作。
- 让静态的资源只走静态资源服务器，动态的走动态的服务器
- Nginx的静态处理能力很强，但是动态处理能力不足，因此，在企业中常用动静分离技术。
- 对于静态资源比如图片，js，css等文件，我们则在反向代理服务器nginx中进行缓存。这样浏览器在请求一个静态资源时，代理服务器nginx就可以直接处理，无需将请求转发给后端服务器tomcat。
- 若用户请求的动态文件，比如servlet,jsp则转发给Tomcat服务器处理，从而实现动静分离。这也是反向代理服务器的一个重要的作用。



### Nginx怎么做的动静分离？

只需要指定路径对应的目录。location/可以使用正则表达式匹配。并指定对应的硬盘中的目录。如下：（操作都是在Linux上）

```
        location /image/ {
            root   /usr/local/static/;
            autoindex on;
        }
```

**1.创建目录**

```
mkdir /usr/local/static/image
```

**2.进入目录**

```
cd  /usr/local/static/image
```

**3.放一张照片上去**

```
1.jpg
```

**4.重启 nginx**

```
sudo nginx -s reload
```

打开浏览器 输入 server_name/image/1.jpg 就可以访问该静态图片了



### LVS、Nginx、HAproxy 有什么区别？

- LVS ：是基于四层的转发。

- HAproxy ： 是基于四层和七层的转发，是专业的代理服务器。

- Nginx ：是 WEB 服务器，缓存服务器，又是反向代理服务器，可以做七层的转发。

  > Nginx 引入 TCP 插件之后，也可以支持四层的转发。



### Nginx条件判断

**if判断**

```java
if ($http_user_agent ~ (125LA|WinHttpRequest|360Spider)) {
	return 444;
}
	
if ($http_referer ~* "filter=author&orderby=dateline") {
	return 444;
}
	
if ($host = 'bbs.gitlib.com') {
	rewrite ^/$ http://bbs1.gitlib.com permanent;
}
```

比较符说明:

- 使用=、!= 比较的一个变量和字符串，true/false
- 使用~、~*与正则表达式匹配的变量，如果这个正则表达式中包含右花括号}或者分号;则必须给整个正则表达式加引号
- 使用-f、!-f 检查一个文件是否存在
- 使用-d、!-d 检查一个目录是否存在
- 使用-e、!-e 检查一个文件、目录、符号链接是否存在
- 使用-x、!-x 检查一个文件是否可执行



**set设置变量**

```java
if ( $host ~* (.*)\.yzz\.cn) {
	set $domain $1;
}
root /www/website/www/gitlib/$domain/;
	
# set语法
set variable value;
```

