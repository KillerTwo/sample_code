## 自定义Spring Boot Starter
### 模块介绍
spring-boot-custom-starter: 父模块。
greeter-library: 需要创建Starter的代码库。
greeter-spring-boot-autoconfigure: 包含自动配置代码。
greeter-spring-boot-starter: 自定义starter。
### 打包
```shell
$ cd spring-boot-custom-starter
$ mvn clean install
```
### 使用starter
```xml
<dependency>
    <groupId>org.greeter</groupId>
    <artifactId>greeter-spring-boot-starter</artifactId>
    <version>1.0-SNAPSHOT</version>
</dependency>
```
**此配置greeter-spring-boot-starter模块的jar包并不会把所依赖的jar包打包进去，所以应用程序需要自己下载或引入greeter-library、greeter-spring-boot-autoconfigure的jar包。**