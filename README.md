本项目为了解决Windows下，多个jdk版本来回切换不方便的问题。

**jenv**：为切换版本的主程序

**使用方法：**

1. 下载所需的jdk版本，要压缩包不要exe

​	`https://repo.huaweicloud.com/java/jdk/`

​	没有的可以自己去官网下载所需版本，然后在虚拟机中安装，将对应目录拖出来使用即可。

2. 将jdk，jenv整合到一个文件夹中（个人习惯，分开也可）
3. 删除原先你配置好的JAVA_HOME  
4. 配置系统环境变量-->Path-->指向你的这个jenv的文件夹
5. 重启电脑，使系统环境变量生效
6. 常用命令：
`jenv add <name> <java_Path>`
如果目录有空格你就需要用双引号引起来
或者直接在jenv.config中配置

```
java17=C:\java\jdk-17.0.2
java1.8=C:\java\jdk1.8.0_202
java11=C:\java\jdk-11.0.2
```
**其他命令：**

`jenv list`
`jenv use xxx`
`jenv change xxx`

注：不是原作者，程序来源于网络