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

```
<!--stackedit_data:
eyJwcm9wZXJ0aWVzIjoiZXh0ZW5zaW9uczpcbiAgcHJlc2V0Oi
BnZm1cbiIsImhpc3RvcnkiOlstMTkwNzk0NTY2MSwzMzUyMTM5
MjMsLTc1MjI3MzI0MCwxOTA1NjcwMDFdfQ==
-->