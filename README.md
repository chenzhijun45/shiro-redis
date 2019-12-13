shiro-redis
=============

## Introduction

shiro only provide the support of ehcache and concurrentHashMap. Here is an implement of redis cache can be used by shiro. Hope it will help you!

## Documentation

Official documentation [is located here](http://alexxiyang.github.io/shiro-redis/).

## 修复了作者的一个bug
https://github.com/alexxiyang/shiro-redis/issues/113
这个bug会导致崩溃,已经修复好向作者发起pr,还未被合并,作者已经有段时间不维护了
可以先使用我修复后发布的版本,接入方法
在pom.xml的project节点加入
```
	<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
  ```
  然后将作者的库 替换为我的
  ```
  <dependency>
	    <groupId>com.github.manondidi</groupId>
	    <artifactId>shiro-redis</artifactId>
	    <version>3.2.10</version>
	</dependency>
  ```

