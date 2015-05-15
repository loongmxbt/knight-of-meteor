Principles of Meteor

Data on the Wire. Meteor doesn't send HTML over the network. The server sends data and lets the client render it.

One Language. Meteor lets you write both the client and the server parts of your application in JavaScript.

Database Everywhere. You can use the same methods to access your database from the client or the server.

Latency Compensation. On the client, Meteor prefetches data and simulates models to make it look like server method calls return instantly.

Full Stack Reactivity. In Meteor, realtime is the default. All layers, from database to template, update themselves automatically when necessary.

Embrace the Ecosystem. Meteor is open source and integrates with existing open source tools and frameworks.

Simplicity Equals Productivity. The best way to make something seem simple is to have it actually be simple. Meteor's main functionality has clean, classically beautiful APIs.

* Data on the Wire - 数据线路：Meteor从不发送HTML到客户端，服务器只传送数据，由客户端来渲染页面。
* One Language - 同一种语言：Meteor在前后端使用同一种语言Javascript。
* Database Everywhere -数据库无处不在：你的数据库不仅仅存在服务器端，还存在干你的浏览器内部，你可以使用相同的代码获取数据。
* Latency Compensation - 延迟补偿：在客户端，Meteor预先取得数据来渲染页面，这使它看起来像立即从服务端获取结果一样。
* Full Stack Reactivity - 全栈随动：Meteor App都是实时App，从后台数据库到页面模板， 全部都会随着数据的变化而自动更新。
* Embrace the Ecosystem - 拥抱社区：Meteor是开源框架，并和其他已有框架集成共存，比如一套代码同时编译成为Web App和iOS、Android多平台的移动App。
* Simplicity Equals Productivity -简单即是高效：使某事看起来简单的最佳方式就是确实让它变简单。Meteor的主要功能都有简洁优雅的API。


一种语言 前端/后端/web/mobile

你如果想创建一个 web 或 mobile 应用，你可能需要学习除了前端 HTML、CSS、JavaScript 和 之外，还需掌握比如 PHP、Ruby、Python 等其中一个语言来开发服务器端代码，还需要学习 Objective-C/Swift 或 Java/Golang 语言来开发 iOS 或 Andriod app。而对于 Meteor 应用，你只要 JavaScript 语言就可以编写可在客户端和服务器端（Node.js 环境）运行的应用，而且也可以用 PhoneGap/Cordova 来将应用变成可在 iOS 或 Andriod 上运行的 app。所以，用同一个 codebase 来搭建 web, iOS 和 Android 应用是非常高效便捷的。同时，数据库方面你不需要学习繁琐的SQL语句，只需要学习MongoDB，就可以应对大多数的工作，MongoDB也是用Javascript交互的哦。

实时性响应性 Real-time/Reactivity

Meteor 应用具有响应性。每当数据改变时，客户端页面会及时同步自动更新页面。与传统方式不同，每当客户端发送一个链接或指令后，传递回服务器，服务器根据指令读取数据库生成 HTML 页面传递回客户端。想象一下，在两台电脑的两个浏览器打开同一个网页时，当页面有更新时，传统方式是需要浏览者刷新各自的浏览器来查看页面更新；而响应性可以确保不同电脑的两个浏览器可以同步自动更新网页局部来体现页面更新。而传统开发这功能真是使开发者挠头，而 Meteor 可以帮助开发者轻易地完成实时性的应用开发。