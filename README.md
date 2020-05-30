# TOMCAT 源码学习
## 一、搭建步骤
### 1.下载源码解压
### 2.创建pom文件，用idea打开项目并编译
### 3.注释掉报错的TestCookieFilter代码
### 4.删除webapps下的example（报listener找不到的错，不影响启动）
### 5.ContextConfig中的（777行左右）webConfig();添加context.addServletContainerInitializer(new JasperInitializer(), null);（注册jsp初始化器，否则访问首页报错）
### 6.运行org.apache.catalina.startup.Bootstrap中的main方法启动tomcat容器

## 二、部署
### 1.war包
### 2.文件夹
### 3.标记符