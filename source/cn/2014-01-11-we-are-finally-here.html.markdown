---
title: 你好，Github
date: 2014-01-11 00:45 UTC
lang: cn
tags:
---

####起
在将近一个月的努力之后，我们终于释出了[Senkyoyarou.com](http://senkyoyarou.com)的第一个版本。__"Senkyoyarou"__, 在日文中的含义是“大家一起参与选举吧！” (当然，还有一些其他意思，你懂的)。我和N先生大概都在这个IT业界呆了超过五年了，我们之前曾经接触过不少语言和框架，比如 __Django__, __Rails__ 等等。但是，这次我们打算尝试一些新的东西。

####这是啥
一切都起源于上海的一个小酒吧里，在大约午夜11点半的时候，我和N先生打了个赌，说如果谁输了的话，就把负责做这个网站的前端( 不过事后发现前后端都不简单 )。这个网站的目的在于 通过 __实时显示__ 政治家以及政治事件的支持率的方式 __唤醒__ 日本人民 (或者其它任何民主国家之人民)的选举意识。我们相信，通过互联网，人们对于政治家的认知度将有一个很大的提升。

####系统
为了处理可能会到来的流量和实时的Web Socket接口，我们发现正在流行的NodeJS可能会对我们有一些帮助，不过使用NodeJS带来的问题也是很明显的:

*	代码的可读性相当糟糕
*	回调函数地狱
*	在Javascript的世界里，内存泄露是时常发生的

当然，NodeJS也有其好处:

*	使用Javascript在前后端开发都相当的迅捷
*	在NPM上有大量资源可以使用
*	直接支持Websocket
*	直接的异步数据请求处理
*	可移植性很高

####达摩
那么，达摩就是我们用[backbone.js](http://backbonejs.org) 和 [underscore.js](http://underscorejs.org)，搭建出来，用于处理纯API，[无状态](http://zh.wikipedia.org/wiki/%E6%97%A0%E7%8A%B6%E6%80%81%E5%8D%8F%E8%AE%AE)式的网站架构的一个微型框架。这个框架非常小，所以我们认为在手机应用的开发上也应该相当好用。