# Change log
## v2.0 
###新增功能
 - 增加种子
 - 所有种子从主站获取
 - 现在程序正在我的服务器上跑着，服务器在美国，元旦前上线91主站所有种子
### fix 
- 原来redis中key的存储不太合理

# v1.0 功能 
- 原始程序，基本能跑

-----------------------------------------------------------------------

# 91 介绍与获取
[91 porn](http://91porn.com/) 是一个知名的自拍视频网站
- 本程序获取所有视频url-
- 然后将视频的下载地址保存到文件，每个文件1000个，可以直接拖到迅雷里下载，一晚上可以下载<label style="color:red"> 300~400GB </label> 没有任何问题
- 可以输入指定的页码进行抓取

# 新版更新说明
- 将原来所有的种子从备站获取改为从主站获取
- 原来只是适配windows目录，现在将记录上次获取的页码数改为当前项目的log目录，种子也放在当前目录sed下

# 这次所有的种子全部来自91主站，如果出现下载不了的情况，那就是91服务器的问题了

# 安装
- [python3](http://www.python.org)
- [redis](redis.io)

On Windows

    redis-server.exe redis.window.conf    

Or on Unix-like OS

    $ redis-server redis.conf 

安装 requests, 快速获取html

    $ pip install requests    


# 启动

    python run.py    

或者

### 双击  <label style="color:red">**run.bat**</label>运行

## 说明
- parse.bat 解析Redis中的列表，获取视频的具体地址
- run.bat 获取所有视频列表，具体视频地址由parse.bat批处理文件解析
- src2file.py 将所有视频source复制到文本中，将文本的内容 `Ctrl` + `C`, 然后`Ctrl` + `V` 复制到迅雷里疯狂的下载吧

# 忠告
  爱惜自己

# 免责声明
  本程序仅做学习交流之使用，如有其它用途并产生其它后果，本人概不负责。
