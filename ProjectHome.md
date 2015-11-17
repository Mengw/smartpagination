QuickStart：

安装JDK：1.5以上，设环境变量JAVA\_HOME，添加%JAVA\_HOME%/bin到PATH环境变量，

安装Ant：建议1.7，设环境变量ANT\_HOME，添加%ANT\_HOME%/bin到PATH环境变量，

安装Ivy：到http://ant.apache.org/ivy/download.cgi 下载，复制ivy.jar到ANT\_HOME/lib，

运行命令：ant resolve，Ivy会把需要的jar下载到lib目录

复制lib/test/junit-4.5.jar 到ANT\_HOME/lib，

运行命令：ant test，如果测试成功，说明一切就绪。

运行命令ant war，成功后把dist下的war包拷贝到tomcat/webapps(也可从http://code.google.com/p/smartpagination/downloads/list 直接下载sample)；

启动tomcat，IE访问Sample应用：http://127.0.0.1:8080/smart_pagination/ ，firefox下分页条不太正常，

进入Sample首页后，点“初始化数据”，又会回到首页；

然后就可以点“简单查询”和“高级查询”这两个功能了，它们分别实现了简单分页和复杂条件查询分页，并且两个都带排序功能。


---

QuickStart\_en:

Install JDK version 1.5 or higher,create JAVA\_HOME environment variable,then add %JAVA\_HOME%/bin to PATH;

Install Ant(prefer 1.7),create ANT\_HOME environment variable,then add %ANT\_HOME%/bin to PATH;

Install Ivy:download ivy.jar from http://ant.apache.org/ivy/download.cgi ,then copy ivy.jar to ANT\_HOME/lib;

Run commond "ant resolve",and Ivy will download dependency jars to /lib;

Copy lib/test/junit-4.5.jar to ANT\_HOME/lib，

Run commond "ant test",if get success message,it means every thing done;

Run commond "ant war",then copy the war in /dist to tomcat/webapps;

Start tomcat and access the Sample application by IE from http://127.0.0.1:8080/smart_pagination/ ,so far it doesn't work very well in firefox;

Now you should be at the index page of the sample application,click "Init data",you will return after success;

Now there is enough data to demonstrate the sample,please click "Simple query" and "Advanced query".


---

smartpagination框架的优势：

1、跨数据库：底层可以采用ORM、iBatis、JDBC等技术访问数据库，甚至可以不是数据库（比如可以是一台远程socket server）；

2、提供了Web层的封装简化开发，但并不绑定某种MVC框架；

3、提供分页标签库，可显示翻页链接、总记录数、总页数，可定制pagesize，可直接跳转；

4、提供排序标签库，可按列升序、降序；

5、支持复杂查询条件表单、查询结果分页、排序、翻页和排序过程中表单状态记忆；

6、是服务器端分页，每次只取出一页数据，不会因数据量大而占用大量内存；

7、集成了安全框架HDIV，可防御XSS跨站脚本攻击，防止系统敏感信息泄露；

8、采用Ivy做依赖管理，可灵活打包；

9、可扩展性：开发新的标签库，以满足个性化需求；