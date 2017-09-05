1. 创建数据库 jeesite
2. 运行脚本 db/jeesite_mysql.sql
3. 安装缺少的 jar
    mvn install:install-file -Dfile=lib/analyzer-2012_u6.jar -DgroupId=org.wltea -DartifactId=analyzer -Dversion=2012_u6 -Dpackaging=jar
    mvn install:install-file -Dfile=lib/apache-ant-zip-2.3.jar -DgroupId=com.ckfinder -DartifactId=apache-ant-zip -Dversion=2.3 -Dpackaging=jar
    mvn install:install-file -Dfile=lib/ckfinder-2.3.jar -DgroupId=com.ckfinder -DartifactId=ckfinder -Dversion=2.3 -Dpackaging=jar
    mvn install:install-file -Dfile=lib/ckfinderplugin-fileeditor-2.3.jar -DgroupId=com.ckfinder -DartifactId=ckfinderplugin-fileeditor -Dversion=2.3 -Dpackaging=jar
    mvn install:install-file -Dfile=lib/ckfinderplugin-imageresize-2.3.jar -DgroupId=com.ckfinder -DartifactId=ckfinderplugin-imageresize -Dversion=2.3 -Dpackaging=jar
    mvn install:install-file -Dfile=lib/UserAgentUtils-1.13.jar -DgroupId=bitwalker -DartifactId=UserAgentUtils -Dversion=1.13 -Dpackaging=jar

4. 修改 resources/jeesite.properties 中数据库配置
5. 启动 tomcat