Install JDK version 1.5 or higher,create JAVA\_HOME environment variable,then add %JAVA\_HOME%/bin to PATH;

Install Ant(prefer 1.7),create ANT\_HOME environment variable,then add %ANT\_HOME%/bin to PATH;

Install Ivy:download ivy.jar from http://ant.apache.org/ivy/download.cgi ,then copy ivy.jar to ANT\_HOME/lib;

Run commond "ant resolve",and Ivy will download dependency jars to /lib;

Copy lib/test/junit-4.5.jar to ANT\_HOME/lib，

Run commond "ant test",if get success message,it means every thing done;

Run commond "ant war",then copy the war in /dist to tomcat/webapps;(Or download demo directly from http://code.google.com/p/smartpagination/downloads/list )

Start tomcat and access the Sample application by IE from http://127.0.0.1:8080/smart_pagination/ ,so far it doesn't work very well in firefox;

Now you should be at the index page of the sample application,click "Init data",you will return after success;

Now there is enough data to demonstrate the sample,please click "Simple query" and "Advanced query".