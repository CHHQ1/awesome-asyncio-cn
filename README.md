<p align="center">
    <img src="https://user-images.githubusercontent.com/19553554/43752023-efd9010c-9a31-11e8-80cc-4c4d9ad9de87.png" alt="Awesome" width="200" height="200"/>
</p>
<h1 align="center">Awesome-Asyncio-CN</h1>
<p align="center">
    <em>Python Asyncio 精选资源列表，囊括了网络框架，库，软件等资源</em>
</p>
<p align="center">
    <a href="https://github.com/sindresorhus/awesome">
        <img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="awesome-list">
    </a>
    <a href="https://github.com/chenjiandongx/awesome-python-cn/issues">
        <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat" alt="contributions-welcome">
    </a>
</p>

[Awesome-asyncio](https://github.com/timofurrer/awesome-asyncio) 是 [Timo Furrer](https://github.com/timofurrer) 发起并维护的 Python Asyncio 资源列表。我觉得这个是很赞的想法，所以维护了一个中文版本的，在这里，收集了大量的 [Asyncio](https://docs.python.org/3/library/asyncio.html) 的最棒、最新的资源，供大家探索 Python 异步编程世界。

Python 3.4 引入了 Asyncio 模块作为标准库，通过协程、多路 I/O 访问 Socket 和其他资源来编写单线程并发代码，并在网络客户端与服务器上运行。Asyncio 内置了对异步 I/O 的支持，其编程模型类似于消息循环，从 Asyncio 模块可以直接获取 EventLoop 引用，再把需要执行的协程放到 EventLoop 中执行，就实现了异步 I/O。Asyncio 是由 Python 之父 Guido 领导的项目，该项目被命名为 Tulip（郁金香）。

[Asyncio](https://docs.python.org/3/library/asyncio.html) 并不是新出现的黑科技，一些社区有名的第三库如 Twisted、gevent 早就推出了异步编程模型。不过，自从 2016 年 3 月，Python 3.4 推出以后，这两年来，Asyncio 变得越来越流行，并且特别受到 Python 社区追捧。


## 贡献代码

欢迎大家为列表贡献高质量的新资源，提交 PR 时请参照以下要求

* 注明推荐理由
* 确保项目相对活跃

## 目录

* [Web 框架](#Web框架)
* [消息队列](#消息队列)
* [数据库驱动](#数据库驱动)
* [网络](#网络)
* [爬虫](#爬虫)
* [测试](#测试)
* [备选事件循环](#备选事件循环)
* [并行](#并行)
* [其他](#其他)
* [文献](#文献)
* [演讲](#演讲)


## Web框架

*构建 Web 应用的库*

* [aiohttp](https://github.com/KeepSafe/aiohttp) - 支持 Asyncio (PEP-3156) 的 HTTP 客户端/服务端网络库。
* [sanic](https://github.com/channelcat/sanic) - Python 3.5+ Web 服务器，主打速度与性能。
* [Quart](https://gitlab.com/pgjones/quart) - 支持 Asyncio 的 Web 微框架，使用与 Flask 相同的 API。
* [Kyoukai](https://github.com/SunDwarf/Kyoukai) - 使用 Asyncio 编写的 Python3.5+ 完全异步 Web 框架。
* [cirrina](https://github.com/neolynx/cirrina) - 基于 aiohttp 的异步 Web 框架。
* [autobahn](https://github.com/crossbario/autobahn-python) - 支持 Asyncio 与 Twisted 的 WebSocket 及 WAMP，用于客户端与服务端。
* [websockets](https://github.com/aaugustin/websockets/) - Python 构建的 WebSocket 客户端/服务端的库，致力于简洁、正确地编写代码。
* [Tornado](http://www.tornadoweb.org/en/stable/) - 高性能 Web 框架以及异步网络库。
* [Japronto!](https://github.com/squeaky-pl/japronto) - 基于 uvloop 和 picohttpparse 构建的实验性 HTTP 工具箱。
* [uvicorn](https://github.com/encode/uvicorn) - 轻量级的，快速的 ASGI 服务器。

## 消息队列

*使用消息队列执行应用的库*

* [aioamqp](https://github.com/Polyconseil/aioamqp) - 使用 Asyncio 异步执行 AMQP。
* [aiozmq](https://github.com/aio-libs/aiozmq) - 集成了 Asyncio (pep 3156) 的 ZeroMQ。
* [crossbar](https://github.com/crossbario/crossbar) - Crossbar.io 是提供分布式和微服务应用的网络平台。

## 数据库驱动

*数据库的驱动库*

* [asyncpg](https://github.com/MagicStack/asyncpg) - 快速访问 PostgreSQL 数据库客户端的异步驱动。
* [asyncpgsa](https://github.com/CanopyTax/asyncpgsa) - 提供 Sqlalchemy Core 支持的 Asyncpg。
* [aiopg](https://github.com/aio-libs/aiopg/) - 访问 PostgreSQL 数据库的异步驱动。
* [aiomysql](https://github.com/aio-libs/aiomysql) - 访问 MySQL 数据库的异步驱动。
* [aioodbc](https://github.com/aio-libs/aioodbc) - 访问 ODBC 数据库的异步驱动。
* [motor](https://github.com/mongodb/motor) - 访问 MongoDB 数据库的异步驱动。
* [aioredis](https://github.com/aio-libs/aioredis) - [aio-libs](https://github.com/aio-libs) 提供的异步 Redis 客户端 (PEP 3156)。
* [asyncio-redis](https://github.com/jonathanslenders/asyncio-redis) - 访问 Redis 客户端 (PEP 3156)的异步驱动。
* [aiocouchdb](https://github.com/aio-libs/aiocouchdb) - 基于 aiohttp (Asyncio) 构建的 CouchDB 客户端。
* [aioinflux](https://github.com/plugaai/aioinflux) - 基于 aiohttp 构建的 InfluxDB 客户端。
* [aioes](https://github.com/aio-libs/aioes) - 兼容 elasticsearch 的 Asyncio 驱动。
* [peewee-async](https://github.com/05bit/peewee-async) - 基于 [peewee](https://github.com/coleifer/peewee) 和 aiopg 实现的 ORM。
* [GINO](https://github.com/fantix/gino) - 基于 [SQLAlchemy](https://www.sqlalchemy.org/) Core 和 [asyncpg](https://github.com/MagicStack/asyncpg) 方言的轻量级 Python 异步 ORM。
* [aiocache](https://github.com/argaen/aiocache) - 支持多个后端 (Memory、Redis 和 Memcached) 的 Asyncio 缓存管理器。
* [aiomcache](https://github.com/aio-libs/aiomcache) - 访问 Memcached 的 Asyncio(PEP 3156) 驱动库。

## 网络

*网络通讯库*

* [AsyncSSH](https://github.com/ronf/asyncssh) - 提供执行 SSHv2 协议的异步客户端/服务端。
* [asks](https://github.com/theelous3/asks) - 与 [requests](https://github.com/requests/requests) 接口相似的异步 HTTP 库。
* [aioftp](https://github.com/aio-libs/aioftp) - 基于 Asyncio 的 ftp 服务。
* [aiodns](https://github.com/saghul/aiodns) - 简单的 Asyncio DNS 服务解析器。
* [websockets](https://github.com/aaugustin/websockets) 构建于 Asyncio 之上的异步 websockets 库。

## 爬虫

*应用于网络爬虫的库*

* [gain](https://github.com/gaojiuli/gain) - 基于 Asycnio 的网络爬虫框架。
* [aspider](https://github.com/howie6879/aspider) - 基于 Asyncio 和 aiohttp 的网络爬虫框架。
* [Scrapy](https://github.com/scrapy/scrapy) - 一个为了爬取网站数据，提取结构性数据而编写的应用框架。

## 测试

*测试 Asyncio 应用程序的库*

* [aiomock](https://github.com/nhumrich/aiomock/) - 支持异步的 Python mock 库。
* [asynctest](https://github.com/Martiusweb/asynctest/) - 一个增强标准 unittest 包的测试库。
* [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) - 支持 Asyncio 的 Pytest 库。
* [aioresponses](https://github.com/pnuckowski/aioresponses) - 一个适用于 aiohttp 的模拟请求库。

## 备选事件循环

*备选的 Asyncio 循环库*

* [uvloop](https://github.com/MagicStack/uvloop) - 基于 libuv 实现的 Asyncio 事件循环库。
* [curio](https://github.com/dabeaz/curio) - 协程并发库。
* [trio](https://github.com/python-trio/trio) - 人性化的，Pythonic 的异步 IO 库。

## 并行

*并行异步编程的库*

* [aioprocessing](https://github.com/dano/aioprocessing) - 结合 multiprocessing 与 Asyncio 的进程库，支持 Python3.4+。
* [aiomultiprocess](https://github.com/jreese/aiomultiprocess) - 进一步提升异步性能的多进程库。
* [asynq](https://github.com/quora/asynq) - Quora 出品的 Python 异步编程库。

## 其他

*未归类的优秀 Asnycio 库*

* [aiofiles](https://github.com/Tinche/aiofiles/) - 基于 Asyncio，支持文件异步操作。
* [aiodebug](https://github.com/qntln/aiodebug) - 用于监控和测试 Asyncio 程序的微型库。
* [aiorun](https://github.com/cjrh/aiorun) - 提供处理通用 Asyncio 样板，启动和关闭事件驱动的 `run` 函数。
* [aiozipkin](https://github.com/aio-libs/aiozipkin) - 使用 zipkin 的分布式 Asyncio 追踪测量仪。
* [faust](https://github.com/robinhood/faust) - 纯 Python 的流处理库，用于处理流数据和事件。
* [paco](https://github.com/h2non/paco) - 协程驱动的异步编程的工具库 (Python3.4+)。
* [aiortc](https://github.com/jlaine/aiortc) - 使用 Python asyncio 实现的 WebRTC 和 ORTC。
* [aiotools](https://github.com/achimnol/aiotools) - 通用的 Asyncio 工具集。

## 文献

*关于 Asyncio 的文档、博客等文献*

* [Asyncio 官方文档](https://docs.python.org/3/library/asyncio.html) - 介绍了异步 I/O、事件循环、协程及任务等内容。
* [Asyncio 精编简介](http://masnun.com/2015/11/13/python-generators-coroutines-native-coroutines-and-async-await.html) - 生成器，协程，原生协程及 async/await。
* [异步窥探](https://hackernoon.com/async-through-the-looking-glass-d69a0a88b661) - 非常好的一篇文章，列出了哪些用例应该使用 Asyncio ，哪些用例无需使用 Asyncio。
* [异步 Python](https://hackernoon.com/asynchronous-python-45df84b82434) - 介绍如何进行 Python 异步编程。
* [用 Asyncio 进行 Python 开发](https://hackernoon.com/asyncio-for-the-working-python-developer-5c468e6e2e8e) - 介绍异步编程的开发，从简单示例说起，一直到 URL 爬取。
* [Python Aiohttp 的测试极限](https://pawelmhm.github.io/asyncio/python/aiohttp/2016/04/22/asyncio-aiohttp.html) - 使用 Python Aiohttp 进行百万量级的并发测试。
* [Python Asyncio 入门介绍](https://hackernoon.com/a-simple-introduction-to-pythons-asyncio-595d9c9ecf8c) - 通俗易懂的 Python asyncio 库入门介绍。
* [深入理解 Python 异步编程（上）](http://aju.space/2017/07/31/Drive-into-python-asyncio-programming-part-1.html) - 彻底理解异步编程是什么、为什么、怎么样。深入学习 asyncio 的基本原理和原型，了解生成器、协程在 Python 异步编程中是如何发展的。

## 演讲

*关于 Asyncio 的主题演讲*

* [Topics of Interest (Python Asyncio)](https://www.youtube.com/watch?v=ZzfHjytDceU) - David Beazley 的主题演讲。
* [Python Asynchronous I/O Walkthrough](https://www.youtube.com/playlist?list=PLpEcQSRWP2IjVRlTUptdD05kG-UkJynQT) - Philip Guo 的主题演讲。
* [Thinking Outside the GIL with AsyncIO and Multiprocessing](https://www.youtube.com/watch?v=0kXaLh8Fz3k&t=1279s) - John Reese 的主题演讲
* [Asynchronous Python for the Complete Beginner](https://www.youtube.com/watch?v=iG6fr81xHKA) - Miguel Grinberg 的主题演讲
