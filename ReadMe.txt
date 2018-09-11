导入Swagger静态API文档步骤

1、启动待导出API文档服务
2、修改pom文件中的<properties> <swaggerInputPath>http://localhost:8253/v2/api-docs</swaggerInputPath> </properties>值为目标服务的IP端口信息
3、在当前目录执行 mvn clean compile 命令
4、生成的文档有html和pdf两种格式，目录分别为
     target\docs\asciidoc\html\index.html
     target\docs\asciidoc\pdf\index.pdf
pdf格式文件可用Word2016打开，然后另存为word格式文件