# tomcat构建
   ### 基本步骤
       1、下载源码
       2、解压源码
       3、在解压后的源码目录中新建home文件夹
       4、将源码目录文件夹中的conf和webapps文件夹拷贝到home下
       5、在源码目录下新建pom.xml文件
       6、在pom.xml
       7、配置启动参数
       8、修改源码 创建org.apache.jasper.servlet.JasperInitialize
       9、启动执行bootStrap



### 乱码问题
    utf-8编码可以用gbk和iso8859-1解码后编回去
    gbk编码后只能用iso8859-1解码后编回去
    问题在于jdk默认采用Unicode（unicode-16，任何字符两个字节）编码，配置文件为utf-8

### 启动参数
    -Dcatalina.home=C:/Users/Administrator/Desktop/Study/IdeaWorkSpace/tomcat/apache-tomcat-8.5.73-src/apache-tomcat-8.5.73-src/home
    -Dcatalina.base=C:/Users/Administrator/Desktop/Study/IdeaWorkSpace/tomcat/apache-tomcat-8.5.73-src/apache-tomcat-8.5.73-src/home
    -Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager
    -Djava.util.logging.config.file=C:/Users/Administrator/Desktop/Study/IdeaWorkSpace/tomcat/apache-tomcat-8.5.73-src/apache-tomcat-8.5.73-src/home/conf/logging.properties

