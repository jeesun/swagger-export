<p align="center">
<a href="http://www.oracle.com/technetwork/java/javase/overview/index.html"><img src="https://img.shields.io/badge/language-java%208.0-orange.svg"></a>
<img src="https://img.shields.io/badge/release-1.0.0-brightgreen.svg">
</p>

# swagger-export

[Chinese Documentation](README.md)

## Introduce
`swagger-export` is a micro-service that provides export swagger document function. Support exported document's types are HTML and PDF.

## Export examples
[index.html](docs/index.html)

## Export steps
1. start api service;
2. modify pom.xml, change `properties` named `swaggerInputPath`'s value to api service that you have started;
3. run `mvn clean compile`;
4. Exported document's types are HTML and PDF, documents are generated in following folders:
```$xslt
target\docs\asciidoc\html\index.html
target\docs\asciidoc\pdf\index.pdf
```
The PDF file exported exists display problems when it contains Chinese characters. You can use word2016 open it, and transform the type of file to '.doc'.