安装JDK：1.5以上，设环境变量JAVA\_HOME，添加%JAVA\_HOME%/bin到PATH环境变量，

安装Ant：建议1.7，设环境变量ANT\_HOME，添加%ANT\_HOME%/bin到PATH环境变量，

安装Ivy：到http://ant.apache.org/ivy/download.cgi 下载，复制ivy.jar到ANT\_HOME/lib，

运行命令：ant resolve，Ivy会把需要的jar下载到lib目录

复制lib/test/junit-4.5.jar 到ANT\_HOME/lib，

运行命令：ant test，如果测试成功，说明一切就绪。

运行命令ant war，成功后把dist下的war包拷贝到tomcat/webapps(也可从http://code.google.com/p/smartpagination/downloads/list 直接下载sample)；

启动tomcat，IE访问Sample应用：http://127.0.0.1:8080/smart_pagination/
【注意，界面很丑】，firefox下分页条不太正常，

进入Sample首页后，点“初始化数据”，又会回到首页；

然后就可以点“简单查询”和“高级查询”这两个功能了，

它们分别实现了简单分页和复杂条件查询分页，并且两个都带排序功能。