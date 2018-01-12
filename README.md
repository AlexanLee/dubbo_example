# dubbo
spring+maven+dubbo整合:<br>
spring版本：4.2.5.RELEASE <br>
dubbo版本：2.5.3<br>
zookeeper版本：3.4.8<br>

使用方法：<br>
    1.下载安装zookeeper.
     参考：[ZooKeeper 基础知识、部署和应用程序] https://www.ibm.com/developerworks/cn/data/library/bd-zookeeper/index.html
          [深入浅出zookeeper] https://www.gitbook.com/book/holynull/zookeeper/details
    2.下载[dubbo]https://github.com/alibaba/dubbo 源码。
        在dubbo-admin目录下使用：mvn package 打包dubbo-admin.然后将打包好的war包文件拷贝到tomcat的webapps目录下。
        启动tomcat.
        查看[dubbo admin 管理界面]http://localhost:8080/dubbo-admin-2.5.8/ 是否启动成功。
    3.下载本源码，可以在idea中分别配置
        tomcat-1:运行dubbo-provider.war包。端口号：8088
        tomcat-2:运行dubbo-consumer.war包。端口号：8089
        然后查看[客户端]http://localhost:8089/testSay?name=bob 如果显示返回正常，即运行成功。
    
    