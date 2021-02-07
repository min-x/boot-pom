
[项目GitHub链接](https://github.com/min-x/min-x-boot.git) 

本项目是根据SpringBoot和SpringCloud为基础，构建更适合快速开发及上手的基础boot pom。

## 项目使用
在pom.xml引入如下配置即可：
```aidl
<parent>
    <groupId>com.x</groupId>
    <artifactId>min-x-boot</artifactId>
    <version>2.4.2</version>
    <relativePath/> <!-- lookup parent from repository -->
</parent>
```

## 项目内容
1.版本与SpringBoot保持一致，引用SpringCloud，引用SpringCloud版本请详见properties配置，如果需要更改请添加对应version。

2.maven打包使用默认打包为jar，并且打包的jar为普通jar，需要打包成启动jar的模块请添加如下配置：
```aidl
<plugin>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-maven-plugin</artifactId>
    <configuration>
        <skip>false</skip>
    </configuration>
</plugin>
```

3.maven使用的java版本配置为java.version，需要更改请修改对应的properties。

## Reference
> 2021年2月6日11
>> SpringBoot 2.4.2  
>> SpringCloud 2020.0.1
