# Front-End-Dynamic

本文主要搜集一些前端的前沿技术. - 2016/10/20

## vue/weex简单介绍

### vue

Vue.js是2013年由尤雨溪创立的一个前端MVVM框架，其简洁的语法设计、轻量快速的特点深受技术社区的喜爱.

Vue.js是用于构建交互式的Web界面的库。它提供了MVVM数据绑定和一个可组合的组件系统，具有简单、灵活的API。从技术上讲， Vue.js集中在MVVM模式上的视图模型层，并通过双向数据绑定连接视图和模型。实际的DOM操作和输出格式被抽象出来成指令和过滤器。相比其它的MVVM框架，Vue.js更容易上手。

Vue.js的生态不仅体现在趋势榜上，其配套的数据管理库Vuex、路由管理库Vue-router、打包工具、开发者调试插件和项目脚手架等工具和库 也都逐步打造成型，同时拥有非常活跃的开发者社区。

欲了解Vue.js的MVVM模式请查看[Vue.js 60 分钟快速入门](http://mp.weixin.qq.com/s?__biz=MzAxODE2MjM1MA==&mid=2651551140&idx=1&sn=5b791228d7978a837bb83063cf6e07d6&scene=0#wechat_redirect).

### weex

阿里巴巴旗下跨平台移动开发工具weex其实也可以被叫做vue-native.官方支持iOS、Android、HTML5. Write Once, Run Everywhere。一次编写可生成三平台代码。DSL模板学习超简单，直接写HTML、CSS、JS。这意味着可以直接用现有编辑器和IDE的代码补全、提示、检查等功能。轻量级、可扩展、高性能。集成花样多，可在HTML5页面嵌入，也可嵌在原生UI中. 



#### weex与vue的关系

Weex由多个关键模块组成，分别是DSL transformer、JS Framework、HTML5/iOS/Android Renderer和工具链 ， 其中JS Framework就直接使用了部分来自Vue.JS的代码。不过这种使用也是遵守开源协议的（Vue使用MIT协议，Weex使用Apache协议），Weex团队在源码的说明文件中记录了来自Vue.JS和其他开源项目的贡献.


#### weex与react-native的关系

也有人把weex比作react-native + vue, 使用vue的API风格，两端的实现方式则和react-native相像，weex相比react-native的优点就是一次编写三端运行.


查看[关于Weex你需要知道的一切](http://www.imooc.com/article/6961)中的章节**为什么不用React Native**.



### vue/react/angular对比

[vue对比其他框架](http://cn.vuejs.org/guide/comparison.html#Angular)这篇文章说明了vue和其他框架对比的一些优点和缺点.


[ARV 渲染实现比较总结](http://blog.sprabbit.com/2016/03/08/Angular-React-Vue-Rendering-4/)这篇文章直观的说明在渲染性能上vue > react > angular. 文中还提出了一个新的渲染性能在vue之上的框架[Mithril](http://mithril.js.org/).目前该框架仍在开发当中,使用的人并不是很多.


### weex/ReactNative对比

更多关于两者的对比可以查看[weex&ReactNative对比](https://zhuanlan.zhihu.com/p/21677103),不过文章看起来更像是对weex的推广.


## Flash游戏和HTML5游戏

### HTML5游戏用到的技术

- Canvas
- SVG
- WebGL
- Cocos2d-js
- CreateJS
- Flash
- Unreal
- Egret
- Phaser

在极客学院搜了一下关于HTML5游戏开发的教程,展示了如上一些课程...


### 两者比较


HTML5的JS,CANVAS游戏主要面向是移动端，比如手机、iPad, 在PC上还不如FLASH， 在PC上超越FLASH还是相当有难度，但是在移动设备上，因为有天然的屏障IOS(出自商业利益的考虑不支持FLASH，但支持HTML5, 安卓不用说了,全支持。移动设备终端上以后的html5会有更大空间.)， 再加上flash移动版不算太给力，随着硬件的提升以及HTML5各种特型浏览器支持度提高， HTML5不管是CANVAS还是SVG，都会有越来越多的应用的.

更过可以查看[曾嵘](https://www.zhihu.com/question/21985107)在知乎的回答.


### 游戏案例

[10款经典的H5游戏及源码](http://www.html5tricks.com/10-html5-game-with-code.html) 


## 全景技术

- [打造H5里的“3D全景漫游”秘籍](https://isux.tencent.com/3d.html)
- [iOS全景漫游](http://www.jianshu.com/p/e09646ebcc64)


## Go语言

首先来看下[十月编程语言排行榜](https://zhuanlan.zhihu.com/p/22842618).接着查看[在Github上活跃的开源计算机语言(居然没有Node?)](https://github.com/showcases/programming-languages),貌似Go语言还是很火? 

貌似Go语言的前身是C语言(C语言相对还是比较熟悉),查看[我们为什么选择了Go语言](http://kevin.doyeden.com/2016/09/24/why-we-choose-go/)可以清晰直观的了解到Go语言的设计理念. 同时从'世界上最好的语言(PHP)'转到'世界上另一个最好的语言'的人深刻讲述了[我为什么选择使用Go语言？](https://www.sdk.cn/news/2836),使我们对Go语言有一个更深刻的认识和了解.


选用Atom作为Go语言的IDE,[给Python开发者的Go语言入门指南](http://mp.weixin.qq.com/s?__biz=MzI0NjIxMzE5OQ==&mid=2656697874&idx=1&sn=5c0964e436fe4e16aad3e83e5403c528#rd).

[D语言、GO语言、Rust语言，谁更有前途？](https://www.sdk.cn/news/3058)说明了Go语言和其他语言的有一些比较.


知乎上关于[nodejs与go语言比较如何，它们的发展前景怎样，网站后台开发，选择nodejs好还是go好？](https://www.zhihu.com/question/24378012)的见解. 貌似Node容易上手,但是Node限制较多,从扩展性考虑Go的扩展性比Node强,可以搭出更大的架子.



