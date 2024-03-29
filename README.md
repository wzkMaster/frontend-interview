# 前端校招面试复习指南

我的[这篇文章](https://wzkmaster.github.io/WHU-SIM-Life-Saver/%E5%B0%B1%E4%B8%9A.html)讲解了关于简历制作和面试的技巧，可以作为本文的补充阅读。

## 互联网企业校招面试流程介绍

大厂的面试通常包括这几个阶段：

1. **简历投递**。可以是在官网直接也可以内推。比较建议采用内推的方式，这样有利于获得更多信息，也容易找到更缺人的部门。内推人可以是身边的同学，也可以是在牛客网、boss直聘的软件上找的网友。可以在上述两个软件上面注册一个账号并填写简历，会有很多人来邀请投递，这些通常是缺人的部门，成功的几率更大。
2. **测评**。测评的内容通常是一些心理学的量表题，也有一些智力题。基本上所有厂用的都是同一套系统，可以提前在网上看一些答题套路，这个阶段一般都不是问题。只要记得及时填写，不要错过时间就好。
3. **笔试**。不一定所有的公司都有这个阶段。笔试通常会有算法题，有的公司还有选择题、问答题等。前者一般是leetcode简单到中等难度的题目，后者的内容一般都是前端相关的基础知识，也会涉及计算机基础知识。准备笔试的话最重要的当然是刷题，leetcode最好是刷有两百题左右，关于刷题我后面会细讲。知识性的题目背好八股文一般就问题不大。笔试通常只要通过某个及格线就可以进入后续的面试阶段，例如华为是100分，因此如果笔试的时候发现有题目完全不会做也不用紧张，尽量把会做的做出来就好。
4. **两到三轮技术面试**。这个是决定是否求职成功的**最重要阶段**，问的内容通常包括基础知识、算法题、项目相关以及软素质相关。
5. **HR面**。到了这个阶段基本上说明已经成功了，HR面主要是用于了解你的求职意向等，同时也会做一些基本素质的考察，只要不乱说话一般就能过。

## 前端知识地图

面试的过程中最重要的当然是基本的技术知识，其实也就是所谓的“八股文”。但很多大厂的考察方式现在都比较灵活，所以还是得把相关的知识真正学通才能更好地应对面试。我这里就不列举具体的知识点内容了，主要是说一些要注意的点和总体的知识框架。

### HTML

这块没啥好问的。有可能会问到的两个问题就是语义化和meta标签。这两个知识点可以稍微了解一下，最好是有项目中的实际应用案例，会更加分。

### CSS

CSS通常都是考察的重点之一，常见的问题包括`position`的不同取值，`grid`和`flex`的相关知识，垂直居中、两栏三栏布局等的实现（记得越多种越好），伪类和伪元素等等。相关的八股在掘金上面有很多很好的整理了，找一篇过一过就好。同样的也要想一想相关知识点在实际项目中的应用。

有些面试官也会问一些比较冷门的知识点，例如我之前就被问了一个`nth-of-type`这个伪类，这种只能看平时的积累了。推荐FrontendMasters上面[Jen Kramer](https://frontendmasters.com/courses/intermediate-html-css/)的课程，她会用到一些比较少见的HTML和CSS的东西，可以开拓一下视野。CSS secrets 这本书也很值得一看。

### JS

JS无疑是最重点的考察项目，但JS的优质资料是非常多的，例如**犀牛书、红宝书、[现代JS教程](https://zh.javascript.info/)、[你不知道的JS](https://github.com/getify/You-Dont-Know-JS)**，前面说的那两本书的目录可以作为复习提纲。一些难理解的知识（例如事件循环，JS引擎原理等）可以看一些讲座视频，例如JSConf等，在Youtube上面检索关键词（英文）就好。Frontend Masters上[Kyle Simpson](https://frontendmasters.com/courses/deep-javascript-v3/)和[hard parts](https://frontendmasters.com/courses/javascript-hard-parts-v2/)系列课程对JS中的类型、时间循环、异步编程、闭包等概念的阐释也非常棒。

### 计算机网络

计算机网络如果之前没有学过且有耐心看体系化的课程，可以看[b站湖科大教书匠](https://www.bilibili.com/video/BV1c4411d7jb/?spm_id_from=333.337.search-card.all.click&vd_source=c5a5aa45b307809696ff99ad8744fc8f)的视频学习一下整个计算机网络的知识体系。前端比较常问的是`HTTP`和`TCP`的相关知识。HTTP可以通过极客时间上的[这个课程](https://time.geekbang.org/column/intro/100029001)，TCP的知识点看湖科大教书匠视频中对应的章节学习即可。

### 浏览器原理和性能优化

一个很经典的面试问题是“输入一个URL按回车，发生了什么”，这个问题的回答涉及了计算机网络和浏览器原理的基本知识，如果能把这个问题讲好是很体现基本功的。同时技术面试中也会有很多问题涉及到浏览器的一些具体运行原理，对此我推荐阅读[这个课程](https://time.geekbang.org/column/intro/100033601)。

基本上所有的面试都会问关于项目中性能优化的问题，可以阅读[这本小册](https://juejin.cn/book/6844733750048210957?enter_from=course_center)以及[这个课程](https://frontendmasters.com/courses/web-performance/)来系统学习性能优化的方法。谷歌的[Web Vitals](https://www.youtube.com/watch?v=5Ox0nqa_pPc&list=PLqC58yKM1FYFrV1BnF-M7TplnKG-_eOpM&index=16&t=1459s)也可以了解一下。

### Vue & React

对于自己项目经历中有用到的框架要比较了解，基本的API、设计思想、配套工具（路由、状态管理）等要熟悉，这些可以通过官方文档来学习。对于框架原理也要有一定的了解，最好是能够学习一下源码。Vue的源码学习可以看[尤雨溪本人的讲解](https://www.bilibili.com/video/BV1rC4y187Vw/?spm_id_from=333.337.search-card.all.click&vd_source=c5a5aa45b307809696ff99ad8744fc8f)，React可以看[卡颂的源码解析](https://react.iamkasong.com/)。
### 前端工程化

**Typescript:** Frontend Masters上[Mike North](https://frontendmasters.com/teachers/mike-north/)的课程讲的极好。

**Webpack:** 如果没怎么用过，至少了解基本的概念，毕竟许多项目的打包都是基于Webpack或者其衍生框架。可以跟着[Brad的课程](https://www.youtube.com/watch?v=IZGNcSuwBZs)敲一个React项目的基本配置熟悉一下。对于`vite`与`webpack`的原理区别要有一定的了解。

### 新技术

要保持对新技术的关注，例如最近比较火的vite、层出不穷的各种SSR框架，最好是可以简单讲一下其原理，要是有实际使用的经历就更好了。这方面可以关注[fireship](https://www.youtube.com/c/Fireship)这个博主，他会有很多对新技术的讲解。掘金上面也有很多新技术的相关博客。
## 算法题和计算机基础

算法题可以跟着[这本小册](https://juejin.cn/book/6844733800300150797?enter_from=course_center)的思路学习，学完之后自己再刷一刷leetcode的top 100热题就好。常见的数据结构和算法也要了解，手写快速排序、归并排序、树的遍历等的考察也是非常常见的。

除了常规的算法题，面试的时候也会考察一些JS的手写代码题目，通常是一些原生API的实现，这类题目掘金上也有很多整理，找一篇看一看就好，看的同时要自己写一写，印象才会更深刻。

学习设计模式可以帮你写出更好的代码，学了之后要学会用于日常的编码实践中。面试的时候设计模式也是经常会被考察到的。这方面曾探的**JavaScript设计模式与开发实践**是经典书籍，[这本小册](https://juejin.cn/book/6844733790204461070?enter_from=course_center)讲的更简单一点，时间不够的话就选择后者。

计算机基础最好的参考资料是著名的CSAPP，但这本书是真的厚，反正我看不下去。推荐看一下[Computer Science Crash Course](https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)，了解基本的知识体系。还有System Design Interview和How Software Works这两本书，了解一下关于系统设计、密码学、图像视频编码的基本知识，这些都是可能会问到的。[Scott Hansleman](https://www.youtube.com/playlist?list=PL0M0zPgJ3HSesuPIObeUVQNbKqlw5U2Vr)的这个播放列表也非常值得一看。

## 项目和软素质

推荐看一下[这个专栏](https://time.geekbang.org/column/intro/100023401)。

## 关于资料

### 付费资料获取途径

付费资料的优点是更加体系化，而且质量通常也相对较好。不可否认有很多免费的优质资料存在，但付费资料通常都是优于免费资料的，而且它们集中于平台上，可以减少很多无谓的检索时间。想想自己学完了可以找到年薪几十万的工作，出一点小钱来学点技术显然也不应该是问题。

极客时间新用户有7天的免费会员，其实足够用来看完一个专栏了；他们时不时也会有活动免费赠送若干天的会员，可以利用那些时间白嫖；在他们的微信公众号可以进行学生认证，然后可以五折购买课程。

Frontend Masters可以通过注册github education来获得六个月的免费观看权利。

掘金小册时不时会有打折活动，通过关注他们的公众号领一个优惠码可以获得7折优惠。

### 免费资料推荐

Youtube上面的一些技术会议演讲，最经典的当然就是JSConf。另外推荐几个前端博主：Web Dev Simplify是我比较喜欢的；Traversy Media比较入门向，Fireship的视频节奏快内容紧凑，比较有趣。当需要了解某个知识点或者某项技术的时候可以看看他们的讲解。[这个播放列表](https://www.youtube.com/playlist?list=PLqC58yKM1FYFrV1BnF-M7TplnKG-_eOpM)里面收集了一些我觉得比较好的技术相关视频
