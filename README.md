# qqProject
【项目技术】 在这个项目中，运用了多线程和网络通讯等技术，使用了监听者设计模式。
【项目介绍】 这个项目分为服务器端和客户端。服务器端为文件：qq_s1 ;客户端为文件：qq_c1。
【服务器端】 整个文件夹被分为五个包：qq.dao,qq.bean,qq.db,qq.pub,qq.server
               在qq.pub中定义了一些客户端和服务器端公用的端口号等公用类TCPSocket包装了tcp通讯的类，UDPSocket包装了UDP通讯的类。
               在qq.dao包中将sqlServer数据库与本项目连接时使用的数据传输进行包装。
               在qq.bean中有两个实体类：用户实体类和好友实体类。
               在qq.db中将数据库与本项目连接。
               在qq.server中迭代了8个版本的服务器，启动时使用最后一版服务器：即启动服务器server8。serverThread8为服务器线程。
【客户端】   整个文件夹被分为五个包：qq.client,qq.bean,qq.component,qq.listener,qq.ui
               在qq.pub Commonuse中定义了一些客户端和服务器端公用的端口号等公用类;TCPMessage定义了报文类;TCPSocket包装了tcp通讯的类，UDPSocket包装了UDP通讯的类。
               在qq.client包里迭代了三个版本的client，主要是测试I/O流时创建的项目。使用时无需在意这个包。
               在qq.bean中有两个实体类：用户实体类和好友实体类。
               在qq.component中ClientImgCell定义了好友列表的样式;imgPanel重写了SWING的Jpanel类，使图片作为背景。
               在qq.listener中使用设计者模式中的监听者模式，进行用户间的消息互发
               在qq.UI中的LoginFrame中使用SWING书写了登陆界面，MainFrame使用SWING书写了登陆后的主界面，ReceiveFrame使用SWING书写了接受消息框，SendFrame使用SWING书写了
               发送消息框，RegisterFrame迭代了三个版本，这里主要使用SWING书写了注册界面，使用最后一个版本即可
               
               
               
【必读：启动手册】 先运行 qq_s1中的sever8，再启动qq-c1的loginFrame。               
