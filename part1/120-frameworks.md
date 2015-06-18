# Meteor VS 其他框架

在了解完Meteor的基本概念之后，我们来简单介绍一下Web开发工具的演化历史并对比一下Meteor与当今其它流行技术栈不同的地方。

在很早很早以前 Web 1.0阶段，大概还只是
早期 Frontpage，网页制作三剑客 Dreamweaver Flash Fireworks

前面的发展无疑就是两块，内容与样式分离，内容与交互分离，前后端分离。

## LAMP 架构
LAMP是一组用来搭建动态网站或者服务器的开源软件，它们是各自独立的程序，但是因为常被放在一起使用，拥有了越来越高的兼容度，共同组成了一个强大的Web应用程序平台。

通常，经典的LAMP架构是指这几样东西：以Linux为代表的开源服务器操作系统，如Ubuntu，CentOS等Linux发行版；以Apache为代表的开源Web服务器软件；以MySQL为代表的开源数据库管理系统和PHP这个服务端脚本语言。

当然，广义的LAMP架构可以替换其中的任何一样或几样软件。如Linux发行版可以用FreeBSD等代替，Apache可以用Nginx代替（通常被称为LNMP或LEMP），MySQL用MariaDB代替，PHP用Perl或Python代替等等。倘若切换到Windows体系，则可以使用IIS作为服务器软件，也可以使用PHP等脚本语言而不是ASP。

大概在2010年之前，LAMP架构与J2EE，.Net形成了三足鼎立之势，国内的大多数网站都无出这三种架构，而其中的LAMP架构又是最为低成本的网站解决方案，所以大多数中小企业和个人站点都使用LAMP这种架构。从网站流量上来说，70%以上的访问流量都是LAMP提供的[ref]，LAMP是当时最强大的网站解决方案。

基于LAMP架构有许多著名的开源项目，最著名的莫过于Wordpress和Drupal这两套系统了。曾几何时，Wordpress几乎成为了每个Web开发者必须鼓捣过的东西，你可以不会PHP，但你必须鼓捣过Wordpress。虽然WordPress因为过于臃肿，存在性能缺陷而广受诟病，但它的易用性仍使得它在博客系和或CMS领域立于不败之地。相较Wordpress来说，Drupal的名声要好很多，但是Drupal更类似一个CMS系统的开发框架，易用性上远远不如Wordpress，但是它的可定制性远超前者。所以，Drupal的使用者一般有专业的团队提供技术支持，而Wordpress则可以单枪匹马上阵。

美国的政府网站大多数采用了Drupal，例如白宫网站。国内一些企业网站也采用了Drupal。美国的自媒体和国内的自媒体通常采用Wordpress。

此外还有MediaWiki，维基百科的
discuz国内的论坛
各种cms系统，phpwind，dedecms等等，国内的大多数公司及新闻网站都是用的这些系统。
此外著名的站点还有Wikipedia，基于MediaWiki。

## Rails + Backbone
在2010年之前，网页的渲染基本上还处于静态页面的阶段，也就是说，由服务端生成好HTML代码再传输到客户端，也就是浏览器。

### Rails

### Backbone
Backbone 为复杂Javascript应用程序提供模型(models)、集合(collections)、视图(views)的结构。其中模型用于绑定键值数据和自定义事件；集合附有可枚举函数的丰富API； 视图可以声明事件处理函数，并通过RESTful JSON接口连接到应用程序。

Backbone 其实是一个十分久远的前端框架, 或者说, 在 Angular 之前, 它是事实的标准. 而且在很多重前端的项目中, 都应用很不错. 随着时间的推进, 小而美( 核心只有 1000 多行 )不太适合普通开发者使用, 重复开发的轮子太多, 人们开们转向 Angular 与 Ember 了.

## Express + Angular

### Express
Express 是一个简洁、灵活的 node.js Web 应用开发框架, 它提供一系列强大的特性，帮助你创建各种 Web 和移动设备应用。

### Angular
AngularJS诞生于2009年，由Misko Hevery 等人创建，后为Google所收购。是一款优秀的前端JS框架，已经被用于Google的多款产品当中。AngularJS有着诸多特性，最为核心的是：MVVM、模块化、自动化双向数据绑定、语义化标签、依赖注入、等等。

AngularJS是为了克服HTML在构建应用上的不足而设计的。HTML是一门很好的为静态文本展示设计的声明式语言，但要构建WEB应用的话它就显得乏力了。所以我做了一些工作（你也可以觉得是小花招）来让浏览器做我想要的事。

通常，我们是通过以下技术来解决静态网页技术在构建动态应用上的不足：

类库 - 类库是一些函数的集合，它能帮助你写WEB应用。起主导作用的是你的代码，由你来决定何时使用类库。类库有：jQuery等

框架 - 框架是一种特殊的、已经实现了的WEB应用，你只需要对它填充具体的业务逻辑。这里框架是起主导作用的，由它来根据具体的应用逻辑来调用你的代码。框架有：knockout、sproutcore等。

AngularJS使用了不同的方法，它尝试去补足HTML本身在构建应用方面的缺陷。AngularJS通过使用我们称为标识符(directives)的结构，让浏览器能够识别新的语法。例如：

使用双大括号{{}}语法进行数据绑定；
使用DOM控制结构来实现迭代或者隐藏DOM片段；
支持表单和表单的验证；
能将逻辑代码关联到相关的DOM元素上；
能将HTML分组成可重用的组件。


### MEAN.js

MEAN.JS is a full-stack JavaScript solution that helps you build fast, robust, and maintainable production web applications using MongoDB, Express, AngularJS, and Node.js.

为什么不选择MEAN而选择Meteor呢？因为Meteor前后端更加的统一。

## Restful API
REST（Representational State Transfer，表现层状态转化）这个词，是 Roy Thomas Fielding 在他2000年的博士论文中提出的。

* 资源（Resources）－ 所谓“资源”，就是网络上的一个实体，或者说是网络上的一个具体信息。
* 表现层（Representation）－ 我们把“资源”具体呈现出来的形式，叫做它的“表现层”。
* 状态转化（State Transfer）－ 如果客户端想要操作服务器，必须通过某种手段，让服务器端发生“状态转化”。


## Meteor

为什么还要两套甚至多套系统呢？为什么不把它们整合到一套系统里面呢？于是便有了Meteor。

一个优秀的框架需要具备那些东西？
* 优雅的设计理念
* 丰富的可拓展性
* 卓越的性能
* 开发者友好