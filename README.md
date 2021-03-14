### 配置无人值守安装iso的过程并在Virtual Box中完成自动化安装

首先到该网站：https://releases.ubuntu.com/20.04/?_ga=2.173640228.608551553.1615713687-1954741177.1615604874，下载ubuntu 20.04

![文件 ubuntu 20.04](img/1.jpg)

创建虚拟电脑，设置名称为ub20.04-young，并选择好类型版本

![](img/2.jpg)

![分配好内存](img/3.jpg)

![创建虚拟硬盘，设置文件位置大小](img/4.jpg)

创建的虚拟机如图所示：

![](img/7.png)

在设置界面选择网络，将网卡1，网卡2分别调制如下（NAT，主机host-only）：

![](img/6.jpg)

![](img/5.jpg)

之后，在设置页面的存储中分配光驱处红圈处，导入之前就已经下好的iso文件：Ubuntu 20.04 live-server amd64.iso

![](img/8.png)

![](img/9.png)

操作完成之后，启动虚拟机，运行过程如下：

![](img/10.png)

![选择英文](img/11.png)

![依次选择Done](img/12.png)

记得自己记下自己的用户名以及密码

![等待操作完成之后选择REBOOT NOW](img/13.png)

接着移除上述虚拟机设置-存储的控制器IDE，再在控制器：SATA下新建两个虚拟光盘按顺序挂在Ubuntu 20.04 live-server amd64.iso，再挂载init.iso

![](img/14.png)
![](img/15.png)

运行虚拟机，得到如下指令：
 
 ![](img/16.png)

 选择yes

  ![](img/17.png)