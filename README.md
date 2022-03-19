# 36tz_cn_245
Java读源码之Netty深入剖析
Java读源码之Netty深入剖析
👇👇👇👇👇👇👇👇点击下载地址👇👇👇👇👇👇👇
[![download](https://51xueit.vip/muke_img/5fcdfcac09ee0e7f05400304.jpg "下载地址")](http://www.36tz.cn "下载地址")
### 第1章 课程介绍 

#### 介绍本课程需要的前提知识和内容概要
1-1 Netty深入剖析 (11:26)


### 第2章 Netty基本组件

#### 使用一个简单的socket例子概括Netty里面的基本组件，包括NioEventLoop，Channel，ByteBuf，Pipeline，ChannelHandler
2-1 一个简单的socket例子 (06:17)

2-2 Netty对于socket的抽象 (05:05)

2-3 Netty组件简单介绍 (12:40)


### 第3章 Netty服务端启动 

#### 分析服务端启动流程，包括服务端Channel的创建，初始化，以及注册到selector
3-1 服务端启动demo (03:43)

3-2 服务端Channel的创建 (12:20)

3-3 服务端Channel的初始化 (08:07)

3-4 注册selector (07:27)

3-5 服务端口的绑定 (08:16)

3-6 服务端启动总结 (01:05)


### 第4章 NioEventLoop

#### 分析Netty reactor线程处理过程，包括事件监听，事件处理，常规任务处理和定时任务处理
4-1 NioEventLoop概述 (01:57)

4-2 NioEventLoop创建概述 (03:20)

4-3 ThreadPerTaskThread (06:08)

4-4 创建NioEventLoop线程 (03:20)

4-5 创建线程选择器 (05:36)

4-6 NioEventLoop的启动 (07:47)

4-7 NioEventLoop执行概述 (03:14)

4-8 检测IO事件 (08:59)

4-9 处理IO事件 (10:44)

4-10 -reactor线程任务的执行 (10:39)

4-11 -NioEventLoop总结 (03:31)


### 第5章 新连接接入 

#### 分析新连接接入以及绑定reactor线程，绑定到selector的过程
5-1 新连接接入概述 (01:42)

5-2 新连接检测 (07:46)

5-3 NioSocketChannel的创建 (08:07)

5-4 Channel的分类 (10:53)

5-5 新连接NioEventLoop的分配和selector注册 (09:58)

5-6 NioSocketChannel读事件的注册 (06:22)

5-7 新连接接入总结 (02:03)


### 第6章 pipeline

#### 分析pipeline的创建，初始化，添加和删除ChannelHandler，事件传播机制，异常传播机制
6-1 pipeline概述 (01:31)

6-2 pipeline初始化 (12:08)

6-3 添加ChannelHandler (12:57)

6-4 删除ChannelHandler (07:03)

6-5 inBound事件的传播 (20:40)

6-6 outBound事件的传播 (15:17)

6-7 异常的传播 (15:25)

6-8 pipeline总结.mp4 (04:46)


### 第7章 ByteBuf

#### 详细分析ByteBuf种类，如何减少多线程内存分配竞争，不同大小内存是如何分配的
7-1 内存分配概述 (02:22)

7-2 ByteBuf结构以及重要api (06:38)

7-3 ByteBuf分类 (15:54)

7-4 内存分配器ByteBufAllocator分析 (08:39)

7-5 UnPooledByteBufAllocator分析 (11:09)

7-6 PooledByteBufAllocator概述 (13:28)

7-7 directArena分配direct内存的流程 (07:26)

7-8 内存规格的介绍 (04:08)

7-9 缓存数据结构 (10:55)

7-10 命中缓存的分配流程 (11:40)

7-11 arena、chunk、page、subpage概念 (07:37)

7-12 page 级别内存分配 (18:15)

7-13 subpage 级别的内存分配 (12:29)

7-14 ByteBuf的回收 (09:25)

7-15 总结 (03:39)


### 第8章 Netty解码

#### 详细分析Netty解码原理，解码器抽象，以及几种常见的解码器
8-1 Netty解码概述 (01:53)

8-2 抽象解码器ByteToMessageDecoder (11:30)

8-3 基于固定长度解码器分析 (04:03)

8-4 行解码器分析 (12:02)

8-5 基于分隔符解码器分析 (12:14)

8-6 基于长度域解码器参数分析 (11:11)

8-7 基于长度域解码器分析 (16:27)

8-8 解码器总结 (04:45)


### 第9章 Netty编码及writeAndFlush()

#### writeAndFlush传播流程，编码器抽象，writeAndFlush详细流程
9-1 Netty编码概述 (03:45)

9-2 writeAndFlush()抽象步骤 (06:29)

9-3 抽象编码器MessageToByteEncoder (11:50)

9-4 写buffer队列 (12:33)

9-5 刷新buffer队列 (13:19)

9-6 总结 (03:19)


### 第10章 Netty性能优化工具类解析

#### 详细分析Netty里面最高频使用的两个性能优化类FastThreadLocal以及轻量级对象池Recycler
10-1 性能优化工具类概述 (01:27)

10-2 FastThreadLocal的使用 (04:18)

10-3 FastThreadLocal的创建和get()实现 (17:18)

10-4 FastThreadLocal的set实现 (04:12)

10-5 Recycler的使用 (04:21)

10-6 Recycler的创建 (08:09)

10-7 从Recycler中获取对象 (06:03)

10-8 同线程回收对象 (04:31)

10-9 异线程回收对象 (12:51)

10-10 异线程收割对象 (16:07)

10-11 性能优化工具类总结 (03:50)


### 第11章 Netty设计模式应用

#### 分析各类常见设计模式以及在Netty中的应用
11-1 单例模式在Netty里面的应用 (04:50)

11-2 策略模式在Netty里面的应用 (03:34)

11-3 装饰者模式在Netty里面的应用 (07:19)

11-4 观察者模式在Netty里面的应用 (15:44)

11-5 迭代器模式在Netty里面的应用 (05:35)

11-6 责任链模式在Netty里面的应用 (08:44)


### 第12章 Netty高性能并发调优

#### 系统层面单机如何支持百万连接，如何提升应用层面性能
12-1 性能调优概述 (00:25)

12-2 单机百万连接模拟与瓶颈 (08:14)

12-3 单机百万连接调优过程 (20:49)

12-4 Netty应用级别性能瓶颈 (06:18)

12-5 Netty应用级别性能调优过程 (16:39)


### 第13章 课程总结

#### 对本课程做一个回顾总结
13-1 课程回顾和总结 (07:36)


[下载地址](http://www.36tz.cn "下载地址")
