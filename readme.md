# 大威天龙_fofa无边

# **没有导出!没有导出!!没有导出!!!**

## 变更说明

### 2021-5-29  V1.2



1. 修改UI样式,相同视觉范围内显示更多信息
2. 搜索条件输入框中响应回车键,输入完以后直接回车获得结果
3. 添加TAB页签关闭按钮
4. 表格隔行显色
5. 配置文件自定义返回表头
6. 修改右击使用默认浏览器打开,改为右击菜单
7. 添加一键telnet对方端口,省去打开命令行操作
8. 添加一键redis未授权访问,省去打开命令行操作
9. 使用Super-portScan进行全端口扫描
10. 添加1个彩蛋

### 目录结构如下

E:.
│  config.properties -------------------配置文件
│  dwtl.wav
│  fofa_bate.jar      -------------------启动主程序
│  Super-PortScan.py -----------------端口扫描
│
├─fofa_lib                 -------------------依赖包
│      fastjson-1.2.62.jar
│      flatlaf-1.0-rc1.jar
│      fofa-core-1.0.2.RELEASE.jar
│      jackson-annotations-2.9.10.jar
│      jackson-core-2.9.9.jar
│      jackson-databind-2.9.10.4.jar
│
└─tmp------------------------------临时文件夹,可以不用,但不能没有



## 整体效果如下

![1622302041701](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/1622302041701.png)

### 启动过程

过程如下,启动后4秒打开主界面

![init](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/init.gif)



### 回车响应

![huiche](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/huiche.gif)

### 右击浏览器打开

![liulanqi](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/liulanqi.gif)

### 右击telnet端口

![telnet](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/telnet.gif)



### 右击扫描全端口

![portscn](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/portscn.gif)

### 右击redis未授权访问

![redis](https://raw.githubusercontent.com/naozibuhao/fofatools/main/readme.assets/redis.gif)

### 自定义表格头

支持表格头如下:

```
ip,port,domain,title,country,province,city,country_name,header,protocol,banner,cert,isp,as_number,as_organization,latitude,longitude
```

1. 表格头之间使用","间隔调整配置文件中表头顺序即可调整在GUI中显示的顺序
2. 表格头后面添加:1 在大威天龙中将默认被选中,否则默认不选中

![1622302728738](https://github.com/naozibuhao/fofatools/blob/main/readme.assets/1622302728738.png?raw=true)

### 结果数量及关闭按钮

![1622303018001](https://github.com/naozibuhao/fofatools/blob/main/readme.assets/1622303018001.png?raw=true)

## 配置文件说明

```
email=邮箱
key=key
#选择排序要显示的列, 列名:int[1/0] title:1 表示title这一列默认选中 0 或者啥也没有表示非默认选中 
#不要填写host 已经默认添加了,你多加也没用 
fields=ip:1,port:1,domain:1,title:1,country,province,city,country_name,header,protocol,banner,cert,isp,as_number,as_organization,latitude,longitude
#fields=host,title,ip,domain,port,country
# python3位置,如果设置了环境变量,可直接填写python3 即可为端口扫描做准备
pythonpath=python38
#临时文件夹,用于存放window系统所有的命令,及所有系统下所有全端口扫描结果HTML文件
tmp=tmp
# 测试redis未授权访问 值为redis-cli的环境变量,或者redis-cli的物理路径
redis=redis-cli
# 为以后直接awvs做准备
awvsurl=1
awvskey=1
```

# 再说一遍,没有导出!没有导出!!没有导出!!!

如果需要导出数据,可以在表格中全选,Ctrl+C,打开一个EXCEL,然后Ctrl+V

导出功能作者认为没必要