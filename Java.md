# JAVA
## 进程和线程
* PROCESS 
    
* THREAD 

## 和网络编程

### Intro 
* 计算机网络：是指将地理位置不同的具有独立功能的多台计算机通过通信网络连接起来，在网络操作系统，
网络管理软件，以及网络通信协议的管理和协调下，实现资源共享和信息传递的计算机系统

* 网络编程
在网络networking protocols 下面，实现网络互连的不同计算机上运行的程序间可以进行数据交换
* 网络编程三要素
1. IP address. 
 在这样的一个网络中我们如何找到对方. (ComputerA & ComputerB). 
 必须为每台计算机指定一个标示号，通过这个标识号来指定要
 接收数据的计算机和识别发送的计算机，而IP地址就是这个标示号。 
2. Port. 
端口port 是对程序的唯一标识. 
网络的通信，本质上是两个应用程序的通信。每台计算机上都有很多的应用
程序。那么在网络通信时，如何区别这些应用程序呢？如果说IP address可以唯一标识网络中的设备，那么端口号port就可以唯一标识设备
中的application,是应用程序的标识.
3. protocol. 通信的规则

## TCP 通信原理
Java为客户端提供了Socket class, 为server 提供了ServerSocket class.
TPC 发送数据：
Steps: 
1. create client side Socket object 
2. get Outflow, write data 
3. release resource 

