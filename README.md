# tomcat7-maven-plugin

```
 _                                   _    _____                                                             _                _
| |_   ___   _ __ ___    ___   __ _ | |_ |___  |        _ __ ___    __ _ __   __  ___  _ __          _ __  | | _   _   __ _ (_) _ __
| __| / _ \ | '_ ` _ \  / __| / _` || __|   / /  _____ | '_ ` _ \  / _` |\ \ / / / _ \| '_ \  _____ | '_ \ | || | | | / _` || || '_ \
| |_ | (_) || | | | | || (__ | (_| || |_   / /  |_____|| | | | | || (_| | \ V / |  __/| | | ||_____|| |_) || || |_| || (_| || || | | |
 \__| \___/ |_| |_| |_| \___| \__,_| \__| /_/          |_| |_| |_| \__,_|  \_/   \___||_| |_|       | .__/ |_| \__,_| \__, ||_||_| |_|
                                                                                                    |_|               |___/
```

> **欢迎使用和Star支持，如使用过程中碰到问题，可以提出Issue，我会尽力完善**

------------------

## 介绍
&#160;&#160;&#160;&#160;**The Tomcat Maven Plugin provides goals to manipulate WAR projects within the Tomcat 7.x servlet container.**

## 此插件在官方插件`tomcat7-maven-plugin`基础上做了以下功能升级
1. 添加post请求不限制大小

## 开始使用

> 在`pom.xml`配置文件中引入 `tomcat7-maven-plugin`

```xml
<build>
    <plugins>
        <plugin>
            <groupId>org.apache.tomcat.maven</groupId>
            <artifactId>tomcat7-maven-plugin</artifactId>
            <version>2.1.1-SNAPSHOT</version>
            <configuration>
                <path>/</path>
                <uriEncoding>UTF-8</uriEncoding>
                <warSourceDirectory>src/main/webapp</warSourceDirectory>
                <port>80</port>
            </configuration>
        </plugin>
    </plugins>
</build>
```

## 开发者
#### 编译部署
```bash
mvn clean
mvn install
mvn deploy
```

##### Tips

> 报错 Too many unapproved licenses:
- 解决办法：在`pom.xml`文件的插件`apache-rat-plugin`添加`excludes`

--------

## 其它项目支持

- ### 一款简洁优雅的hexo主题：[hexo-theme-yilia-plus](https://github.com/JoeyBling/hexo-theme-yilia-plus)
- ### 一款简洁优雅的VuePress主题：[vuepress-theme-yilia-plus](https://github.com/JoeyBling/vuepress-theme-yilia-plus)
- ### VuePress集成Live2D看板娘：[vuepress-plugin-helper-live2d](https://github.com/JoeyBling/vuepress-plugin-helper-live2d)
- ### VuePress回到页首插件Plus：[vuepress-plugin-gotop-plus](https://github.com/JoeyBling/vuepress-plugin-gotop-plus)

## LICENSE
[![LICENSE](https://img.shields.io/github/license/JoeyBling/tomcat7-maven-plugin "LICENSE")](https://github.com/JoeyBling/tomcat7-maven-plugin/blob/master/LICENSE "LICENSE")
