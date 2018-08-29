# Core包

## 简介

`core`是所有七芒星项目的公共父类包, 其只包含一个`pom`文件, 没有任务功能代码。 主要对项目中常用的`java`包的版本进行了定义和规范。

* 定义常用工具包的版本信息, 如`spring-boot`等;
* 定义公司`nexus`仓库地址;

所有的七芒星项目`pom`文件都应该继承该包, 有特殊情况请另行说明。

## 使用说明

### maven继承使用

在项目的`pom`文件中,应该继承自该包, 使用方式如下:

```pom
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>
    
    <groupId>com.zhongfl.work.order</groupId>
    <artifactId>work-order</artifactId>
    <version>1.0.0-SNAPSHOT</version>

    <packaging>pom</packaging>

    <parent>
        <groupId>com.heptagram.core</groupId>
        <artifactId>core</artifactId>
        <version>4.0.0-RELEASE</version>
    </parent>
    
    .......
```

## 版本指南

`core`包当前版本为`4.0.0-REALEASE`, 主要基于`spring-boot 2.0.0.RELEASE`定义。

```pom

```

