#HNU My-First-Java-Web-Project
###使用springboot框架集成mybatis，采用注释的方式通过localhost:8080/(path+param)，对test数据库进行增删改查的操作。
###并通过stu_no实现对student表和score表的一对一联查。

resource包为资源配置包，application.properties为数据库配置文件
model包含有Score和Student实体类，service包含有函数的接口及其实现类，mapper包里分别有其映射文件（ScoreMapper、StudentMapper）及
其配置文件XML。

web包里有其控制类。ScoreController只控制Score表的增删查改。StudentController能实现对自己的增删改，并通过stu_no外键实现与Score表
一对一的联查。

在Application里可以运行整个项目，然后在浏览器里进行增删改查。

由于是初次接触SSM框架，因此本份代码并没有采取事务操作，也没有检查异常部分，对数据库的增删查改比较呆板，有待下次进行改善！
