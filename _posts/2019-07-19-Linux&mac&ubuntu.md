# linux与mac

```

linux&macos命令行：主要在苹果机下面执行的 。



service sshd start							 开启服务

 ping 192.168.137.103 						查ip的延迟。

 ssh -p22 xyl@192.168.137.103  用ssh服务端控制客户端
终止目录 control +c 控制
				ctrl+c

```





### 读写执行权限:

```
r（read）读

w（write）写

x	执行exe（execute）  --运行文件
```





### 权限：

```
所有者（u）root：只能有一个，也可以换成他人(rw读写权限)

所属组(g)root：我授权（只有读的权限）

其他人（0）other：不能碰

文件所属者->文件所属组-> 文件的修改时间->文件名
```





### 文件类型（用ls -l查出的含义）

```
-二进制文件 r

d目录

l软链接文件
```





### 1目录处理命令：ls

```
执行权限为所有用户
ls -l（lang）		详细信息显示
ls -a 	（add）	查看隐藏
ls  -d （ document）查看目录属性
ls -h (help)人性化的查找,配合-l -hl（-lh） 显示文件大小


ls -i		19714802 404.html
ls -r		tags.htmlls

通配符的使用：
*			任意个数个字符	

?			一个字符，至少一个
[]		表示匹配其中任意一个
[abc] 匹配a,b,c中
[a-f] 匹配从a到f内
```

### 1.2目录处理命令：mkdir

```
make directiries	做目录
mkdir -p [目录名]  创建新目录，-p递归创建

	mkdir 1								可以
 mkdir -p sad/2 				可以
 mkdir -p ddsd1/d32d2/d 可以
  mkdir  1/2/d  1/2/c 前提 1/2 存在
 
 mkdir -p /ddsd1/d32d2/d 不可以
 
 mkdir /1/2/3 删除空目录
```

### 1.3目录处理命令：pwd

（显示当前目录Print Working Directory）

### 1.4目录处理命令：cp

```
copy 拷贝（复制文件或者目录）

cp -rp[原文件或者目录][目标目录]
	-r	复制目录
	-p 保留文件属性（很不错）（拷贝）
cp /Users/ti/Desktop/今日收获.md   /Users/ti/Desktop/lianxi\js.md
就会出现lianxijs.md 


```

### 1.5目录处理命令：mv

```
mv move [原文件的绝对路径][目标路径] 剪切文件 改名
mv /tmp/ja/longze /root/ns  					两个名字不同就是改名

```





### 1.6目录处理命令：r m

```
remove 删除(搬家)
-rf [文件或目录]  
-r 是删除目录  -f 是强制执行 （false)

例子： rm /tmp/
rm 	/Users/tianzi/Desktop/lianxijs.md  				成功
rm -rf 	/Users/tianzi/Desktop/lianxi\ /d2dsd1 	成功
```



### 2文件处理命令：touch（创建空文件）

```
touch 'sd sd'  创建一个sd sd的文件。 但是对他查找一定要‘' 。
 
```

### 计算机中文件大小的表示（科普）



|单位|含义|
| -      | -    |
| 字节B（Byte） | 在计算机中作为一个数字单位，一般为8位二进制数 |
| 千Kibi-byte | 1k，千字节 |
| 兆Mebi-byte | 1m，百万字节 |
| 千兆Giga- | 1g，千兆字节 |
| 太T | |
| 拍P |      |
| 艾E |  |
| 泽Z |  |
| 尧Y | 一亿亿字节 |
|||

​    





# Lamp：

支撑互联网的开源技术（补充）

操作系统		linux
服务器			apache Web

数据库				Mysql 

编译语言				PHP、python、java、c



# Linux命令





### 命令1



| 列表1                                                        |                  |
| ------------------------------------------------------------ | ---------------- |
| ls =list                                                     | 查看文件夹下内容 |
| pwd= print wor directory                                     | 确认工作的文件夹 |
| clean                                                        | 清屏             |
| ~.~                                                          | -.-              |
| cd = change directory+路径                                   | 切换文件夹       |
| touch摸+文件名（参数）                                       | 新建文件         |
| mkdir+文件夹（参数）                                         | 新建文件夹       |
| rm=remove +文件名                                            | 删除文件         |
| re（命令command） -r(带-为选项options) +文件夹（参数paramaster） | 删除文件夹       |
|                                                              |                  |

### 命令2

| 目标-列表2          |                         |
| ------------------- | ----------------------- |
| ls                  | 查看目录内容            |
| cd                  | 切换目录                |
| touch  mkdir rm     | 创建文档 目录 和删除    |
| cp mv               | 拷贝和移动              |
| cat more grep       | 查看文件内容            |
| echo    重定向>和>> | 以及管道 \| (end上面的) |
|                     |                         |

### 命令3

```
ifconfig网络接口配置

ls / 根目录的列表显示


df 显示文件系统的磁盘使用情况统计
Filesystem    512-blocks    

```







### linux单词

```
folder 		文件夹

netcraft		网站

skip				 跳过

basic 			基本

local loopback (lo)本地回路

accept 			接受

Config 			配置



常见报错

command not found 					命令未找到

no such file or directory  	没有这样的文件或目录

```





# linux的类型：

```
Redhat	 红帽
fedoro
suse 
genloo linux 
红旗Linux
Mandriva
turbo linux



debian
ubuntu  乌班图
knoppix


centos 7
deepin 2G
```

### 安装日志：

```
/root/install.log: 				存储了系统中的软件包及其 版本信息

/root/install.log.syslog: 存储了安装过程中留下的 事件记录

/root/anaconda-ks.cfg	:以Kickstart配置文件的格式记录过程中设置的 选项信息
```



### 服务器： 

远程服务器 只能重启（不允许关机）



### 虚拟机的小问题：

```
nat：两个一样
无线 vmware



桥接 :独立的网络号
ifconfig eth0 网络地址

Linux 必须通过挂在之后使用 （是所有的存储设备）
```







### linux目录

（严谨的系统）

```

bin存放 系统命令

home 数组目录 ；tmp 临时目录 做练习的时候在这里面

lib 函数库保存位置

dev 设备文件保存目录

etc 配置文件保存位置

media 媒体设备   ； mnt u盘；  misc nfs服务；这三个都是挂载目录

var 动态保存目录，日志，邮件
usr: 不是user，是Uinx Software Resource=Unix系统软件资源目录，占用的内存目录


```

