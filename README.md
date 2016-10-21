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


[更轻更快的Vue.js 2.0与其他框架对比](http://mp.weixin.qq.com/s?__biz=MzIwNjQwMzUwMQ==&mid=2247484329&idx=1&sn=f79da7c92cda7352c8a651f459ef4172&chksm=9723616ba054e87df94522a9c67de26c9ac1f2532198506f47f9c589070d4c530a66ed37dd70&scene=0#wechat_redirect)更综合性的说明了Vue.js的特点以及易学程度.


更多关于vue和react的对比查看[Vue和React的使用场景和深度有何不同？](https://www.zhihu.com/question/31585377?rf=35892450)


### weex/ReactNative对比

更多关于两者的对比可以查看[weex&ReactNative对比](https://zhuanlan.zhihu.com/p/21677103),不过文章看起来更像是对weex的推广.


>结论: React学习路线比较陡峭,不容易上手,而且对于大型的项目需求设计可能也存在一些弊端.React能火最大一部分是因为移动端的React-Native.Vue的渲染性能在React之上,而且之后还有适应于三种平台的weex扩展(weex已经在淘宝,天猫等大型移动项目上经过考验,毕竟他们之前想用react-native来做结果发现存在很多问题),目前而言是值得学习的一个框架,并且比React容易上手,需要



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

这篇问答告诉我们很多关于[如何从头开始学习制作一款HTML5 小游戏？](https://www.zhihu.com/question/19954833).
还有这样的文章[微信公众号怎么发布HTML5游戏?](https://www.zhihu.com/question/25434838).

### 两者比较


HTML5的JS,CANVAS游戏主要面向是移动端，比如手机、iPad, 在PC上还不如FLASH， 在PC上超越FLASH还是相当有难度，但是在移动设备上，因为有天然的屏障IOS(出自商业利益的考虑不支持FLASH，但支持HTML5, 安卓不用说了,全支持。移动设备终端上以后的html5会有更大空间.)， 再加上flash移动版不算太给力，随着硬件的提升以及HTML5各种特型浏览器支持度提高， HTML5不管是CANVAS还是SVG，都会有越来越多的应用的.

更过可以查看[曾嵘](https://www.zhihu.com/question/21985107)在知乎的回答.


### 游戏案例

[10款经典的H5游戏及源码](http://www.html5tricks.com/10-html5-game-with-code.html) 


## 全景技术

- [微信360全景制作步骤及常见问题](http://jingyan.baidu.com/article/425e69e6b290dcbe15fc168a.html) 这是教程?
- [H5全景图-朋友圈全景图-720°全景-VR -----工具使用](http://blog.csdn.net/lipengshiwo/article/details/52550808) 这也是教程?
- [打造H5里的“3D全景漫游”秘籍](https://isux.tencent.com/3d.html)
- [iOS全景漫游](http://www.jianshu.com/p/e09646ebcc64)


## Go语言

首先来看下[十月编程语言排行榜](https://zhuanlan.zhihu.com/p/22842618).接着查看[在Github上活跃的开源计算机语言(居然没有Node?)](https://github.com/showcases/programming-languages),貌似Go语言还是很火? 

貌似Go语言的前身是C语言(C语言相对还是比较熟悉),查看[我们为什么选择了Go语言](http://kevin.doyeden.com/2016/09/24/why-we-choose-go/)可以清晰直观的了解到Go语言的设计理念. 同时从'世界上最好的语言(PHP)'转到'世界上另一个最好的语言'的人深刻讲述了[我为什么选择使用Go语言？](https://www.sdk.cn/news/2836),使我们对Go语言有一个更深刻的认识和了解.


选用Atom作为Go语言的IDE,[给Python开发者的Go语言入门指南](http://mp.weixin.qq.com/s?__biz=MzI0NjIxMzE5OQ==&mid=2656697874&idx=1&sn=5c0964e436fe4e16aad3e83e5403c528#rd).

[D语言、GO语言、Rust语言，谁更有前途？](https://www.sdk.cn/news/3058)说明了Go语言和其他语言的有一些比较.


知乎上关于[nodejs与go语言比较如何，它们的发展前景怎样，网站后台开发，选择nodejs好还是go好？](https://www.zhihu.com/question/24378012)的见解. 

以下是vue.js创始人的说法

作者[TJ Holowaychuck](https://github.com/tj)是Node界最高产的开发者之一，最近转投 go 了。当然，原因是他现在更多地开始搞分布式系统了，如果做网站他还是会选择 Node。

从大型工程的角度来说，go 是完爆 Node 的。性能，内存开销，静态类型，对异步的处理，异常的处理，可调试性，系统稳定度，工具链的成熟度，等等，都是 go 占优。但是 Node 在依赖处理方面更好，npm 对依赖版本的管理 （go 的依赖不能指定版本，还需要借助非官方的工具）非常优秀，另外 Node 社区的活跃度要比 go 好，如果你想要快速做一个东西，npm 上各种现成的包可以用。


作者：尤雨溪
链接：https://www.zhihu.com/question/24378012/answer/27591423
来源：知乎
著作权归作者所有，转载请联系作者获得授权。


Node在做网站这方面，尤其是需要直接面向用户的http服务器这方面，有一个天然的优势，那就是前后端的语言统一。一方面可以减少切换语言的脑力成本，提高开发者的效率，另一方面可以实现前后端共享模板，从而实现首屏服务器渲染，局部更新浏览器渲染的架构，提高首屏的加载速度。

如果你做的网站后台就是个简单的CRUD应用，或者是做产品原型，或者你同时还想兼顾前端，Node 会是更好的选择；但如果你的后台很复杂，需要区分各种服务，搞数据分析，分布式集群等等，那绝对是选go。

最后，其实两者结合起来用也是完全可以的，把Node 作为面向用户的大前端的一部分，专门负责页面的生成，后端用go 或者其他语言实现，前后端之间通过规范的数据接口通信。关于这样的解决方案，参见[如何评价淘宝 UED 的 Midway Framework 前后端分离？](https://www.zhihu.com/question/23512853)


一个golang使用者的说法


如果团队水平参差不齐的话，建议使用golang 
如果团队对于异步流程控制很熟悉的话，并且也喜欢JS的话建议可以express之类的Node库。

另外，如果技术选型，还要从维护成本来看，异步调用的代码需要在设计之初考虑好，否则更改一个回调可能影响到多个。比如以删除粉丝为列，首先你要查找这个粉丝是否存在，然后等待回调，在这个里面你又要查找两者的关系，然后又是一个回调，在之后你又要去看是否能删除 ，最后在删除 后做动作，，，，，一个又一个回调。


其他人的回答

真的要选还是golang吧，解决方法比较多，后期的扩展方便。问题也是版本有点跳，已经上线的功能真不晓得跟不跟，看团队的人更熟悉那个，就用那个。Nodejs还不太适合做企业后台，虽说跟别人说的时候很溜，但这没什么卵用。


一个是限制较多的世界，一个是限制较少的世界。限制少的，自然就更依赖你的独立思考和求证能力；而限制多的，则可以少犯错误少动脑子。接受什么样的权利和义务的平衡点，每个人都不一样。


就发展前景来说，目前我觉得 node 的势头比 go 要好。就网站后台的开发来说，用 node 更快，学习资料也更多。网站后台不是个适合 go 的场景。
你可以看看 node 的 express 框架，跟 go 的 web 框架之间的 helloworld 对比。node 的简单很多，而且 npm 上面的模块优势目前看不出 go 可以追的上。



>结论: 学习Go语言是有需求的,但不是必要的,可以私下里学习.目前Node在业务上足可以满足需求.而且Go语言学习可能需要一个积累的过程,毕竟是一门新的语言,不过在Go学习上还是有优势的,毕竟更接近C语言.

