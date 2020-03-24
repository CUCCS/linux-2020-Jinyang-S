# 实验1-无人值守

* 实验部分

1.环境准备完毕后查看ip地址  

​	ifconfig -a  

​	ip:192.168.56.101

2.用putty连接得到的ip  

![连接putty](img\putty_link.png)  

3.用psftp将本地镜像复制进虚拟机  

![镜像上传](img\iso_up.png)  

4.挂载镜像并同步光盘内容到cd  

![光盘同步完成](img\iso_copy.png)  

5.添加新内容到isolinux/txt.cfg  

![添加内容](img\change_txt.png)  

6.添加ubuntu-server-autoinstall.seed并修改isolinux.cfg  

![添加seed](img\add_seed.png)  

7.重新生成md5sum.txt后用ftp下载custom.iso    

![下载新的镜像](img\download_iso.png)  

8.挂载custom.iso自动安装完成并登录  

![安装成功](img\log_in.png)

* 遇到的问题

1.putty无法连接root用户：修改配置文件允许root被ssr连接  

2.psftp无法下载新的镜像：将其重新安装到C盘并保证安装路径无中文和空格

* 思考

1.双网卡设置及用途：网卡1为NAT，保障虚拟机的网络连接；网卡2为Host-Only，用于putty访问  

2.如何在虚拟机和宿主机之间传输文件：使用psftp