# 信鸽推送sdk 
fork 自 [https://github.com/xingePush/xinge-api-java](https://github.com/xingePush/xinge-api-java)

代码比较简单，然而bug和不满意的地方总是存在。故决定还是自己fork,自由自在。

## 修改内容：
- 1、custom字段，类型由String变为Map<String,String>
- 2、maven，引入github deploy插件。方便开发和使用。

## 引用：

    <dependencies>
     	<dependency>
            <groupId>com.github.xingePush</groupId>
            <artifactId>xinge</artifactId>
            <version>1.2.2-fix</version>
        </dependency>
    </dependencies>

    <repositories>
        <!-- 引用了github的xingesdk。没有在中心仓库。考虑下载到本地中心仓库。去除此仓库       -->
        <repository>
            <id>maven-repo</id>
            <url>https://raw.githubusercontent.com/fanlushuai/maven-repo/master/</url>
        </repository>
    </repositories>
    
## 使用：

和fork源一致，参见测试代码

## 建议姿势：

fork本项目到自己github账户，参见https://github.com/fanlushuai/maven-repo  readme的maven github repo配置。建立并修改成自己的github的maven repo。
自己本地build，自动deploy到自己的maven-repo。相当方便灵活。
