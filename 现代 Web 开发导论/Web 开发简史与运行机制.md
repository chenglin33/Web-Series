[![返回目录](https://parg.co/U0y)](https://parg.co/UHU)

# Web 开发简史与运行机制

这是一个最好的时代，也是最坏的时代，我们亲身经历着激动人心的变革，也往往会陷入选择的迷茫。随着浏览器版本的革新与硬件性能的提升，Web 前端开发进入了高歌猛进，日新月异的时代，无数的前端开发框架、技术体系争妍斗艳，让开发者们陷入困惑，乃至于无所适从。特别是随着现代 Web 前端框架（Angular 、 React、Vue.js ）的出现，JavaScript 、 CSS、HTML 等语言特性的提升，工程化、跨平台、大前端等理论概念的提出，Web 前端开发的技术栈、社区也是不断丰富完善。

任何一个编程生态都会经历三个阶段，首先是原始时期，由于需要在语言与基础的 API 上进行扩充，这个阶段会催生大量的辅助工具。第二个阶段，随着做的东西的复杂化，需要更多的组织，会引入大量的设计模式啊，架构模式的概念，这个阶段会催生大量的框架。第三个阶段，随着需求的进一步复杂与团队的扩充，就进入了工程化的阶段，各类分层 MVC，MVP ， MVVM 之类，可视化开发，自动化测试，团队协同系统；这个阶段会出现大量的小而美的库。我们可以简要地将 JavaScript 出现以来至今的发展历史划分为以下时代：

| Era/ 时代   | Timeline/ 时间线 | Problems/ 问题                         | Innovations/ 创新                       | Dominant Browsers/ 主流浏览器                                |
| ----------- | ---------------- | -------------------------------------- | --------------------------------------- | ------------------------------------------------------------ |
| 蛮荒时代    | 大概 1996 – 2004 | 基础 DOM 操作，用户交互                | JavaScript 本身，XHR 与 AJAX            | Netscape Navigator, Microsoft Internet Explorer              |
| jQuery 时代 | 大概 2004 – 2010 | 增长的网页复杂度，大量的浏览器兼容需求 | 健壮的 DOM 操作，早期的 SPA 单页应用    | Microsoft IE，Mozilla Firefox                                |
| SPA 时代    | 大概 2010-2014   | DHTML 过载，大规模数据操作，性能       | MVC 框架，双向数据流，DOM 自动化        | Google Chrome，Microsoft IE ， Mozilla Firefox，Apple Safari |
| 现代        | 大概 2014- 现在  | 性能，复杂应用的状态管理，可用性       | Virtual DOM，单向数据流，类型系统，测试 | Google Chrome，Apple Safari                                  |

Web 前端开发可以追溯于 1991 年蒂姆 · 伯纳斯 - 李公开提及 HTML 描述，而后 1999 年 W3C 发布 HTML4 标准，这个阶段主要是 B/S 架构，没有所谓的前端开发概念，网页只不过是后端工程师的顺手之作，服务端渲染是主要的数据传递方式。接下来的几年间随着互联网的发展与 REST 等架构标准的提出，前后端分离与富客户端的概念日渐为人认同，我们需要在语言与基础的 API 上进行扩充，这个阶段出现了以 jQuery 为代表的一系列前端辅助工具。2009 年以来，智能手机开发普及，移动端大浪潮势不可挡，SPA 单页应用的设计理念也大行其道，相关联的前端模块化、组件化、响应式开发、混合式开发等等技术需求甚为迫切。这个阶段催生了 Angular 1、Ionic 等一系列优秀的框架以及 AMD、CMD 、 UMD 与 RequireJS、SeaJS 等模块标准与加载工具，前端工程师也成为了专门的开发领域，拥有独立于后端的技术体系与架构模式。

而近两年间随着 Web 应用复杂度的提升、团队人员的扩充、用户对于页面交互友好与性能优化的需求，我们需要更加优秀灵活的开发框架来协助我们更好的完成前端开发。这个阶段涌现出了很多关注点相对集中、设计理念更为优秀的框架，譬如 React、Vue.js 、 Angular 2 等组件框架允许我们以声明式编程来替代以 DOM 操作为核心的命令式编程，加快了组件的开发速度，并且增强了组件的可复用性与可组合性。而遵循函数式编程的 Redux 与借鉴了响应式编程理念的 MobX 都是非常不错的状态管理辅助框架，辅助开发者将业务逻辑与视图渲染剥离，更为合理地划分项目结构，更好地贯彻单一职责原则与提升代码的可维护性。在项目构建工具上，以 Grunt、Gulp 为代表的任务运行管理与以 Webpack、Rollup 、 JSPM 为代表的项目打包工具各领风骚，帮助开发者更好的搭建前端构建流程，自动化地进行预处理、异步加载、Polyfill 、压缩等操作。

JavaScript 虽匆匆而生却自由生长，历经，在 ES6 之后；在 TypeScript、Flow 等静态类型语言的。最负盛名的当是 Chrome 内置的 V8 引擎，也是 Node.js 的基石。而 像 Java 8 中内置的 Nashorn 也。笔者并不反对使用模板指令、CSS-in-JS 等杂糅的方式，但是还是

经过多年的发展，Node.js 已经完全具备了支撑企业级应用的能力，在 Lowe、Netflix 、阿里等国内外诸多的公司中有着海量的实践；并且 Node.js 天然地语言亲和性，使开发人员更易承担全栈的职责。

[![](https://github.com/wxyyxc1992/OSS/blob/master/ProcessOn/IT%E6%9E%B6%E6%9E%84.png?raw=true)](https://www.processon.com/view/link/59c200c0e4b0cfa0d53bae4a)

业务引领技术，技术驱动业务。前端工程化是根据具体的业务特点，将前端的开发流程、技术、工具、经验等规范化、标准化。它的目的是让前端开发能够 “ 自成体系 ”，最大程度地提高前端工程师的开发效率，降低技术选型、前后端联调等带来的协调沟通成本。

[![](https://github.com/wxyyxc1992/OSS/blob/master/ProcessOn/%E7%8E%B0%E4%BB%A3Web%E5%BC%80%E5%8F%91.png?raw=true)](https://www.processon.com/view/link/59c20128e4b0cfa0d53bae9a)

![](https://hacks.mozilla.org/files/2017/10/01-768x459.png)

![](https://parg.co/UrS)

Client (What happens when you click Order Now?)

Networking (How does information travel across internet?)

Security (How do we prevent hackers from stealing our passwords?)

Server (What does “the cloud” mean exactly?)

Application (What are web servers and web frameworks?)

Database (How do applications retrieve data? SQL vs NoSQL?)

Scaling (How do applications handle millions of requests?)

Rendering (How do browsers work? Basics of JavaScript.)

![](https://cdn-images-1.medium.com/max/2000/1*FjnCt0TCWaxY91E0WQq2DQ.png)

当我们在浏览器内输入某个地址后，经历了如下的步骤网页才最终呈现在我们面前：（ 1）URL 解析浏览器会首先判断你输入的是否为有效的 URL，还是属于需要传输给搜索引擎的默认搜索关键字。并且浏览器还会检查自带的 “ 预加载 HSTS（HTTP 严格传输安全）” 列表，这个列表里包含了那些请求浏览器只使用 HTTPS 进行连接的网站。如果网站在这个列表里，浏览器会使用 HTTPS 而不是 HTTP 协议，否则，最初的请求会使用 HTTP 协议发送。接下来，浏览器会检查你的输入字符是否含有特殊非 ASCII 关键字，如果含有特殊的字符会进行 UTF8 编码，部分特殊的网站会要求进行 GBK 编码。

（ 2）DNS 解析在 URL 解析完成之后，浏览器会根据本地的 hosts 文件或者向本机 / 网关设置的 DNS 服务器发起域名解析请求。DNS 的解析过程中，浏览器会首先检查本机是否有域名缓存，如果没有的话会向 DNS 服务器发起请求，如果子 DNS 服务器不存在该记录则会递归向父层级的 DNS 发起请求。我之前在进行 iOS 开发的时候还碰到 IPV6 的问题，即苹果要求 iOS 应用能够在 IPV6 环境下正常运行，那么这个时候 DNS 服务器发现如果你请求的是 IPV6 的地址，对于仅有 IPV4 地址的服务器其会提供一个 NAT64 的功能，即保证客户端虽然为 IPV6 地址，也能和 IPV4 的服务器正常通信。

（ 3）TCP/IP 协议传输

当浏览器得到了目标服务器的 IP 地址，以及 URL 中给出来端口号（http 协议默认端口号是 80， https 默认端口号是 443），它会调用系统库函数 socket ，请求一个 TCP 流套接字，对应的参数是 AF_INET/AF_INET6 和 SOCK_STREAM 。TCP 的建立连接与关闭连接分别是三次握手与四次握手，概述如下 :

1. 第一次握手：Client 将标志位 SYN 置为 1，随机产生一个值 seq=J，并将该数据包发送给 Server，Client 进入 SYN_SENT 状态，等待 Server 确认。 2. 第二次握手：Server 收到数据包后由标志位 SYN=1 知道 Client 请求建立连接，Server 将标志位 SYN 和 ACK 都置为 1，ack=J+1 ，随机产生一个值 seq=K，并将该数据包发送给 Client 以确认连接请求，Server 进入 SYN_RCVD 状态。 3. 第三次握手：Client 收到确认后，检查 ack 是否为 J+1，ACK 是否为 1，如果正确则将标志位 ACK 置为 1，ack=K+1 ，并将该数据包发 送给 Server，Server 检查 ack 是否为 K+1，ACK 是否为 1，如果正确则连接建立成功，Client 和 Server 进入 ESTABLISHED 状态，完成三次握手，随后 Client 与 Server 之间可以开始传输数据了。

关闭连接时 : 1. 第一次挥手：Client 发送一个 FIN，用来关闭 Client 到 Server 的数据传送，Client 进入 FIN_WAIT_1 状态。 2. 第二次挥手：Server 收到 FIN 后，发送一个 ACK 给 Client，确认序号为收到序号 +1（与 SYN 相同，一个 FIN 占用一个序号）， Server 进入 CLOSE_WAIT 状态。 3. 第三次挥手：Server 发送一个 FIN，用来关闭 Server 到 Client 的数据传送，Server 进入 LAST_ACK 状态。 4. 第四次挥手：Client 收到 FIN 后，Client 进入 TIME_WAIT 状态，接着发送一个 ACK 给 Server，确认序号为收到序号 +1，Server 进入 CLOSED 状态，完成四次挥手。

（ 4）HTTP 请求封装

通常 HTTP 消息包括客户机向服务器的请求消息和服务器向客户机的响应消息。这两种类型的消息由一个起始行，一个或者多个头域，一个只是头域结束的空行和可选的消息体组成。HTTP 的头域包括**通用头，请求头，响应头和实体头**四个部分。每个头域由一个域名，冒号（: ）和域值三部分组成。域名是大小写无关的，域值前可以添加任何数量的空格符，头域可以被扩展为多行，在每行开始处，使用至少一个空格或制表符。

我们在正常的开发中主要会遵循 RESTful 风格，即主要以 GET、POST 、 PUT、DELETE 这四个动词进行请求，每个动词表征不同的含义，同时会将资源名与资源编号放在 URL 中增加可读性。

（ 5）Nginx/Apache 中间件服务器在 Nginx、Apache 服务器中，可以配置 Virtual Host，即根据不同的域名指向不同的目录。而对于 PHP 这样需要动态处理的请求，会考虑使用 FastCGI 进行处理。同时，在服务器中我们也往往需要进行 XSS/SQLInjection/CSRF 等常见的网络攻击手段的防护。

（ 6）前端页面渲染在浏览器接收到服务器返回的前端页面之后，即开始服务器的渲染过程。渲染主要包含了 HTML DOM 解析与 CSS 解析以及最终的页面渲染这几个部分。HTML 解析器的主要工作是对 HTML 文档进行解析，生成解析树。解析树是以 DOM 元素以及属性为节点的树。DOM 是文档对象模型 (Document Object Model) 的缩写，它是 HTML 文档的对象表示，同时也是 HTML 元素面向外部 ( 如 Javascript) 的接口。树的根部是 "Document" 对象。整个 DOM 和 HTML 文档几乎是一对一的关系。

1. 通过遍历 DOM 节点树创建一个 “Frame 树 ” 或 “ 渲染树 ”，并计算每个节点的各个 CSS 样式值 2. 通过累加子节点的宽度，该节点的水平内边距 (padding)、边框 (border) 和外边距 (margin)，自底向上的计算 "Frame 树 " 中每个节点首的选 (preferred) 宽度 3. 通过自顶向下的给每个节点的子节点分配可行宽度，计算每个节点的实际宽度 4. 通过应用文字折行、累加子节点的高度和此节点的内边距 (padding)、边框 (border) 和外边距 (margin)，自底向上的计算每个节点的高度 5. 使用上面的计算结果构建每个节点的坐标 6. 当存在元素使用 floated，位置有 absolutely 或 relatively 属性的时候，会有更多复杂的计算，详见http://dev.w3.org/csswg/css2/ 和 http://www.w3.org/Style/CSS/current-work 创建 layer( 层 ) 来表示页面中的哪些部分可以成组的被绘制，而不用被重新栅格化处理。每个帧对象都被分配给一个层页面上的每个层都被分配了纹理 (?) 7. 每个层的帧对象都会被遍历，计算机执行绘图命令绘制各个层，此过程可能由 CPU 执行栅格化处理，或者直接通过 D2D/SkiaGL 在 GPU 上绘制 8. 上面所有步骤都可能利用到最近一次页面渲染时计算出来的各个值，这样可以减少不少计算量计算出各个层的最终位置，一组命令由 Direct3D/OpenGL 发出，GPU 命令缓冲区清空，命令传至 GPU 并异步渲染，帧被送到 Window Server。

（ 7）Ajax 数据获取我在前端开发中是习惯使用 fetch 库进行数据抓取，同时如果涉及到跨域数据抓取，还会使用 JSONP 跨域或者 CORS 跨域请求协议。

# Rendering

![](https://coding.net/u/hoteam/p/Cache/git/raw/master/2016/6/4/56A2BDBE-4ABE-4269-B961-2BB1EA253F48.png)

![](http://delai.me/code/content/images/2016/01/render-tree-construction.png)

## Create/Update DOM

## Request Resources

## Create/Update Render CSSOM(CSS Object Model)

## Create/Update Render Tree

## Layout

布局，就是浏览器计算 DOM 元素的几何信息的过程：元素大小和在页面中的位置。每个元素都有一个显式或隐式的大小信息，决定于其 CSS 属性的设置、或是元素本身内容的大小、抑或是其父元素的大小。在 Blink/WebKit 内核的浏览器和 IE 中，这个过程称为布局。在基于 Gecko 的浏览器（比如 Firefox）中，这个过程称为 Reflow。虽然称呼不一样，但二者在本质上是一样的。

## Painting

![](https://cdn-images-1.medium.com/max/1600/0*gMqY9IVJXuBbE8DF.)

![1_wqinzmpqggcmx9aoonn76g](https://user-images.githubusercontent.com/5803001/34674559-647cae30-f4c1-11e7-9fea-cbed3a3d2de5.jpeg)
