# tomcat-source-code
### [tomcat8.5.x-source](https://github.com/wmouren/tomcat-source-code/tree/master/tomcat8.5.x-source)

​	`tomcat8.5.x`的源码可以直接导入 `IDEA`中，启动时需要在`IDEA`添加`VM option`参数:

```cmd
-Dcatalina.home=home
-Dcatalina.base=home
-Djava.endorsed.dirs=catalina-home/endorsed
-Djava.io.tmpdir=catalina-home/temp
-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager
-Djava.util.logging.config.file=home/conf/logging.properties
```

设置`Main class`：`org.apache.catalina.startup.Bootstrap`即可直接启动。

`IDEA`导入`Tomcat`源码遇到的问题参考连接:

- https://www.cnblogs.com/jhxxb/p/10768580.html
- https://gongxufan.github.io/2017/10/20/tomcat-source-debug/
- https://blog.csdn.net/zhoutaoping1992/article/details/104751705/