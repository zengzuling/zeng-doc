第一步:将需要的包加载进来，如有架包直接在pom文件中引用就可以，如:
![a1](picture/a1.png "a1.png")
第二步：配置相关的配置文件rabbitmq-connection-mq.xml 用于连接rabbitmq服务端 rabbitmq-receive-mq.xml监听接收消息，rabbitmq-send-mq.xml发送消息。。。
rabbitmq-connection-mq.xml:
![a2](picture/a2.png "a2.png")
rabbitmq-receive-mq.xml:
![a3](picture/a3.png "a3.png")
rabbitmq-send-mq.xml:
![a4](picture/a4.png "a4.png")
第三步：配置properties 。。连接rabbitmq rabbitmq.properties 
![a5](picture/a5.png "a5.png")
第四步：引用相关的properties和接收发的xml文件 Properties在applicationContext-resources.xml 中配置
![a6](picture/a6.png "a6.png")
接收发xml在web.xml中配置:
![a7](picture/a7.png "a7.png")
第五步 ：写发消息的方法:
![a8](picture/a8.png "a8.png")
第六步 ：写接收消息的方法:
![a9](picture/a9.png "a9.png")
第七步：controller 中引用方法:
![a10](picture/a10.png "a10.png")