## ***\*部署项目\****

### ***\*1.还原数据库\****

运行Mysql数据库，利用Navicat等可视化数据库软件连接，创建数据库init_database，导入项目中根目录下sql文件下的数据库还原文件init_database.sql。

### ***\*2.导入项目\****

打开IDEA，点击OPEN...选择pku_qiangke_jxiaodong项目根目录下的pom.xml文件，open as project。

### ***\*3.加载maven\****

等待加载Maven，IDEA自带Maven一般不需要配置。但是用的是官方源可能会比较慢，课百度maven 换阿里源解决。若此步不行，可手动安装maven。

### ***\*4.配置项目\****

配置属性文件路径：\src\main\resources\application.properties 注：只需配置和修改sql主机地址，数据库名，用户名，密码， 项目访问路径，这几个属性，项目即可正常运行访问。 如果数据库是8.0以下版本的，注意要在数据库配置的地方把".cj."去掉

\#数据库连接配置

\#数据库主机地址

spring.redis.host=127.0.0.1

\#数据库名

spring.redis.database=online-course

\#数据库用户名

spring.redis.username=填写你的数据库用户名

\#数据库密码

spring.redis.password=填写你的数据库密码