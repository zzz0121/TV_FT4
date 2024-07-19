# 自动获取酒店源  组播源 #

使用方法：

1.电视盒子

  在看电视直播软件中直接输入以下任一地址即可：
  
      https://ghproxy.net/https://raw.githubusercontent.com/zzz0121/TV_FT4/main/itvlist.txt
      https://cdn.jsdelivr.net/gh/zzz0121/TV_FT4/itvlist.txt
      https://raw.githubusercontent.com/zzz0121/TV_FT4/main/itvlist.txt
  
2.想自己获取电视直播地址的可采用以下方法：

  windows电脑：
  
      1.1 电脑安装最新的chrome，同时执行文件目录下要有对应版本的chromedriver.exe，
      1.2 下载windows目录下的itv.exe及itvtest.exe,
      1.3 首先运行itv.exe，完成后再运行itvtest.exe，
      1.4 运行完成后在当前目录下生成电视直播文件itvlist.txt。
  
  有安装python的电脑：
  
      2.1 电脑安装chrome，下载对应版本的chromedriver
      2.2 下载itv.py cctv.py weishi.py qita.py
      2.3 pip install selenium requests futures eventlet opencv-python
      2.4 依次运行itv.py cctv.py weishi.py qita.py
      2.5 运行完成后在当前目录下生成电视直播文件itvlist.txt。

3.在openwrt或群辉的docker运行：

        1.安装：docker pull liuxipo/itvall:latest
        2.运行：docker run -v /www/itvall:/app itvall
        3.访问：http://本地ip/itvall/itvlist.txt
  
4.推荐在本地电脑运行，不推荐在github运行。github获得的数据不准确，测速不准。

5.udpxy目录为部分组播源。

