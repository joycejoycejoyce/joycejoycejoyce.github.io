# 我实在是pc上运行不了ruby. maintain 这个blog成本太大了。
我决定还是make everything simple 
直接用.md吧


# CSS
[CSS](./CSS.md)
# javascript 
[JavaScript](./JavaScript.md )
# data structure & algorithm 
[DataStructure&Algorithm](./DS&A.md);
# React 
[React](./React.md);


## 大前端时代
### 什么是大前端
简单的说，大前端就是所有前端的统称。比如说Android, iOS, web,的UI层，将其统一起来，就是大前端。
大前端最大的特点在于一次开发，同时适用于所有的平台。开发者不用为同一个APP做Android 和iOS两种模式。
大前端是web统一的时代，利用web不仅能开发出网站，还可以开发手机端web应用和移动端应用程序。

### 大前端为什么会出现？
因为node的出现，前端工程师不需要依赖后端程序而直接运行，将前后端分离起来。所以当开发一个新产品的时候服务
只需要写一次，但是面向用户的产品可能有很多。例如说网站，Android客户端，iOS客户端，和微信小程序。由于每个
平台实用的技术栈不一样，代码无法复用，所以很浪费人力物力。那么大前端就是用来解决这个痛点的。大前端的
主要核心就是跨平台技术。有了跨平台技术，各个平台的差异性就抹平了，开发者只需要一套技术栈就可以开发出适用于
多个平台的客户端。
### 跨平台方案简介
现在主流的跨平台方案： 
1. Cordova/phoneGap
2. React Native
3. Weex 
4. Wechat 小程序
5. PWA
6. Flutter 
根据原理可以分为四大类：
1. H5+原生（Cordova, lonic, 微信小程序）
2. JS开发＋原生渲染（React Native, Weex, 快应用）
3. 自绘UI + 原生（Flutter）
4. 增强版 Web App (PWA)  
H5+原生混合开发
又称为Hybrid开发。现在很多App都用这种模式去开发。比如说微信，淘宝，美团，爱奇艺等等。
这一框架的主要原理就是将AAPP的一部分需要动态变化的内容通过H5来实现，通过原生的网页加载控件WebView(Android)或者
WKWebView(ios)来加载，H5部分是可以随时改变而不用发版，这样就解决了动态化的需求。同时，由于H5只需要一次开发，就能
同时在Android 和iOS两个平台上运行，这也可以减小开发成本。我们称这种H5＋原生的开发模式为混合开发。采用混合模式
开发的APP我们称为混合应用/Hybrid APP.
由于原生开发可以访问平台所有的功能，而混合开发中，H5代码是运行在WebView中，而WebView实际上就是一个浏览器内核，
其JS依然运行在一个权限受限的沙箱中，所以对于大多数的系统能力都没有访问权限，如无法访问文件系统，不能使用蓝牙等。
所以，对于H5不能实现的功能，都要原生去做。而混合框架一版都会在原生代码中预先实现一些访问系统能力的API，然后暴露给
WebView以供JavaScript调用。这样依赖，WebView就成为了JS 和原生API之间通信的桥梁，主要负责JS和原生之间传递调用
消息。而消息的传递必须遵守一个标准的协议。它规定了消息的格式与含义。我们把依赖于WebView 的用于在JS和原生之间通信的
工具称为WebView JavaScript Bridge, 简称为JSBridge,它也是混合开发框架的核心。
混合应用的有点是动态内容是H5，使用web技术栈就可以开发。社区以及资源丰富，缺点是性能不好，对于复杂的用户界面或者是动画，
webview不堪重任。


