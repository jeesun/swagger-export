# swagger-export
`swagger-export`是一个提供swagger文档导出功能的服务，不依赖于具体的API接口服务实现，你可以很方便地导出html和pdf两种格式的静态文档。

## 导出示例
[index.html](docs/index.html)

## 导出步骤
1. 启动待导出的API接口服务；
2. 修改pom文件中`properties`配置的`swaggerInputPath`值为目标服务的IP端口信息；
3. 在当前目录执行`mvn clean compile`命令；
4. 生成的文档有html和pdf两种格式，目录分别为
```$xslt
target\docs\asciidoc\html\index.html
target\docs\asciidoc\pdf\index.pdf
```
导出的pdf格式文件，中文存在显示问题。可用Word2016打开，然后另存为word格式文件。