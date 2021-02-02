# ASIAINFO-FABRIC-SDK 介绍

## 源码

组件在[fabric-sdk-java](https://github.com/hyperledger/fabric-sdk-java.git?_blank) 基础上结合spring进行开发

## 配置文件
 提供两种文件配置方式,格式如下：
- [JSON](config/connection-json.md)
- [YAML](config/connection-yaml.md)
 
文件组成主要是机构、节点、用户的MSP，如网络使用到TLS，需要配置TLS部分


## 使用

依赖引入
```
<dependency>
    <groupId>com.hyperledger.fabric.boot</groupId>
    <artifactId>hyperledger-fabric-spring-boot-starter</artifactId>
    <version>1.0.0</version>
</dependency>
```

在 `application.properties` 指定 网络配置文件路径 spring.fabric.path

```
@Autowired
private FabricTemplate fabricTemplate;
```
执行交易
```
fabricTemplate.submit(method, body);
```

执行查询
```
fabricTemplate.query(method, body);
```