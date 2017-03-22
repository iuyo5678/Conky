# Conky CN
我自己的conky配置.基于[antoniocarelli/Conky](https://github.com/antoniocarelli/Conky)的配置
主要进行了如下的改进：

1. 对其中部分进行了汉化，更改了部分图标。
2. 修正bug，包括程序不显示，部分进程显示的重影等问题。

## 测试
自己在fedora 25上进行了测试。其余不保证效果，有问题随时咨询，我帮你解决吧。

## 效果
效果如下图：

横版配置的效果如下图

![横版](./Conky_Carelli.png)

竖版配置的效果如下图

![竖版](./Conky_Carelli-Vertical.png)

## 安装 
安装步骤如下：

1. 首先安装代码里面的里面的图标文件，`Conky Icons by Carelli.ttf` 安装方式和安装字体一样。
2.  将安装包中的配置拷贝到个人用户根目录，更名为`.conkyrc` 命令如下：
	```shell
	cp conky_carelli.conf ~/.conkyrc
	```
3. 进行配置，主要配置如下几项
   1. 替换成自己的网络设备名， 自己的网络设备名称可以通过`ifconfig`  可以查看到，比如自己的无线网卡名称是`wlp2s`  需要将文件中的`wlp2s0` 全部替换成`wlp2s` 如果自己的有线网卡的名称是`enp370`需要将文件中的`enp3s0` 全部替换成`enp370`
   
   2. 替换自己的外接硬盘挂载位置，可以方便的查看U盘容量。 我的配置文件中文件挂载位置是`/run/media` 你需要全部改成自己的
			
至此，就安装准备完成了。

启动`conky`应该就看到效果了。

Enjoy it!
