# Termux安装archlinux教程
- 同步最新的脚本
- 下载增强工具
- 增强工具的使用
- 关于小广告

-------------------------

## 同步最新脚本

\# 进入主页

**cd** ~

\# 同步最新脚本

**git** clone https://gitlab.com/urain39/termux-archlinux

\# 进入clone的项目目录

**cd** termux-archlinux

\# 安装与运行

**sh** install.sh

----------------------------------------------------------

## 下载增强工具

增强工具其实本来该和最新的脚本写在一起的

但因为github好像只有300M空间的限制，所以我将

包含数据包的代码放在了gitlab上，github只同步了

脚本。下载与使用方法如下

\# 进入termux-archlinux目录

**cd** termux-archlinux

\# 同步脚本

**git** clone https://github.com/urain39/termux-ant

\# 复制到上层目录

**cp** termux-ant/*.sh ..

\# 再次确认

**ls**

目录结构大致是

ant-tool.sh

archlinux

install.sh

termux-ant

---------------------------------------------------------

## 增强工具的使用

sh ant-tool.sh 输出如下

> ant-tool.sh [system] [mount|umount]

> ant-tool.sh [system] [switch]


第一条命令是挂载一些设备和系统映射之类的

第二条命令是切换源为国内源，默认是tuna

这里的 system是你的系统名字，目前我们系统的名字是

archlinux所以我们使用方法如下所示

\# 挂载各种映射

**sh** ant-tool.sh archlinux mount

\# 卸载各种映射

**sh** ant-tool.sh archlinux umount

\# 切换软件源

**sh** ant-tool.sh archlinux switch

----------------------------------------------------

# 关于小广告
更多教程资源欢迎各位[加入termux](http://t.cn/Rx343EW)
