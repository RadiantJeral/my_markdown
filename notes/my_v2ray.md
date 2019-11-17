> My v2ray notes

## 1. 介绍
[Project V](https://www.v2ray.com/) 是一个工具集合，它可以帮助你打造专属的基础通信网络。Project V 的核心工具称为[`V2Ray`](https://github.com/v2ray/v2ray-core)，其主要负责网络协议和功能的实现，与其它 Project V 通信。[`V2Ray`](https://github.com/v2ray/v2ray-core) 可以单独运行，也可以和其它工具配合，以提供简便的操作流程。

## 2. 安装
官方[安装](https://www.v2ray.com/chapter_00/install.html)手册.

### 2.1 Windowns
### 2.2 Linux
V2Ray 提供了一个在 Linux 中的自动化安装脚本。这个脚本会自动检测有没有安装过 V2Ray，如果没有，则进行完整的安装和配置；如果之前安装过 V2Ray，则只更新 V2Ray 二进制程序而不更新配置。

以下指令假设已在 su 环境下，如果不是，请先运行 sudo su。

运行下面的指令下载并安装 V2Ray。当 yum 或 apt-get 可用的情况下，此脚本会自动安装 unzip 和 daemon。这两个组件是安装 V2Ray 的必要组件。如果你使用的系统不支持 yum 或 apt-get，请自行安装 unzip 和 daemon
```
$ sudo su
[sudo] password for username:
# bash <(curl -L -s https://install.direct/go.sh)
```
或者下载`go.sh`到本地安装
```
$ sudo su
[sudo] password for username:
# wget https://install.direct/go.sh
# bash go.sh
```
此脚本会自动安装以下文件：

-   `/usr/bin/v2ray/v2ray`：V2Ray 程序；
-   `/usr/bin/v2ray/v2ctl`：V2Ray 工具；
-   `/etc/v2ray/config.json`：配置文件；
-   `/usr/bin/v2ray/geoip.dat`：IP 数据文件
-   `/usr/bin/v2ray/geosite.dat`：域名数据文件
此脚本会配置自动运行脚本。自动运行脚本会在系统重启之后，自动运行 V2Ray。目前自动运行脚本只支持带有 Systemd 的系统，以及 Debian / Ubuntu 全系列。

运行脚本位于系统的以下位置：

-   `/etc/systemd/system/v2ray.service`: Systemd
-   `/etc/init.d/v2ray`: SysV

脚本运行完成后，你需要：

1.  编辑 /etc/v2ray/config.json 文件来配置你需要的代理方式；
2.  运行 service v2ray start 来启动 V2Ray 进程；
3.  之后可以使用 service v2ray start|stop|status|reload|restart|force-reload 控制 V2Ray 的运行。

## 3. 使用
### 3.1
### 3.2  Linux
**FireFox**
<!--stackedit_data:
eyJwcm9wZXJ0aWVzIjoiZXh0ZW5zaW9uczpcbiAgcHJlc2V0Oi
BnZm1cbiIsImhpc3RvcnkiOlstNzM5MzMyMjM5LDExNTQzNDc4
MTIsMzM1MjEzOTIzLC03NTIyNzMyNDAsMTkwNTY3MDAxXX0=
-->