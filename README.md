[![Build Status](https://travis-ci.com/hanwckf/rt-n56u.svg?branch=master)](https://travis-ci.com/hanwckf/rt-n56u)
![GitHub All Releases](https://img.shields.io/github/downloads/hanwckf/rt-n56u/total)
[![release](https://img.shields.io/github/release/hanwckf/rt-n56u.svg)](https://github.com/hanwckf/rt-n56u/releases)

# README

## UI预览

[![5014eK.png](https://z3.ax1x.com/2021/10/19/5014eK.png)](https://imgtu.com/i/5014eK)
[![501fL6.png](https://z3.ax1x.com/2021/10/19/501fL6.png)](https://imgtu.com/i/501fL6)
[![50MtR1.png](https://z3.ax1x.com/2021/10/19/50MtR1.png)](https://imgtu.com/i/50MtR1)

### 宝塔纯净版介绍

如果你正在寻找宝塔面板专业版的免费替代品，尤其是需要支持 Nginx + PHP + MySQL 环境，还自带 WAF 功能，同时坚持开源免费路线，那你的需求其实很明确，也很合理。从实际体验和功能匹配度来看，以下几款开源免费的面板和独立 WAF 方案，可以成为你当前或未来长期使用的稳定选择。

* 基于BT官方剥离了所有与BT官方的通信、上报、下发、以及登录绑定手机号才能使用的功能；
* 所有功能与原版一致，不会有任何异常，如有任何问题请参考宝塔官方解决方案；
* 提升为企业会员，软件商店中的所有[运行环境]、[免费插件]、[宝塔插件]、[专业版插件]、[企业版插件]；部分[第三方应用]安装可能会失败。

### 特别说明

* 1.该项目只是收集网上的开源项目用于本地虚拟机测试以及小白建站测试，请不要使用于违法途径
* 2.开源无情人有情，请不要滥用或者出售脚本，让脚本制作的大佬遭受不白之冤
* 3.脚本不一定什么时候就没了，记得及时建立快照
* 4.emmmm，至于后门问题，大佬说是没有的，但是你要用那么后果你自己承担，懂？周瑜打黄盖，不要出问题后来逼逼赖赖！

***

## 脚本1：宝塔英文版 aaPanel

* 来源: [https://www.aapanel.com/](https://www.aapanel.com/)

aaPanel面板和宝塔面板都是同一家公司在运营，只是aaPanel面板主要服务于海外客户，宝塔面板服务于本地客户。通常如果使用的是海外的服务器部署web环境，建议使用aaPanel面板。

Centos/Ubuntu/Debian 安装命令：
```
URL=https://www.aapanel.com/script/install_6.0_en.sh && if [ -f /usr/bin/curl ];then curl -ksSO "$URL" ;else wget --no-check-certificate -O install_6.0_en.sh "$URL";fi;bash install_6.0_en.sh aapanel
```

## 脚本2：夸父面板 mdserver-web

基于宝塔开发的开源面板工具。

* 核心优势：轻量（内存占用约 20MB）、界面与宝塔高度相似，支持一键安装 Nginx、PHP 多版本、MySQL 等环境；自带基础防火墙（端口管理）和 SSL 证书申请功能。

* 安装方式：支持 Centos/Ubuntu/Debian，一条命令快速安装：

```bash
curl --insecure -fsSL https://cdn.jsdelivr.net/gh/midoks/mdserver-web@latest/scripts/install.sh | bash
```

## 脚本4：hostPanel

* 核心优势：基于宝塔 7.7 改造的”真离线版”，去除云端通信、强制登录及广告；所有插件（如 Nginx/MySQL）本地化安装，无需联网；界面优化更简洁。

* 安装方式：一键脚本安装：
```bash
wget -O install_panel.sh https://download.hostpanel.cc/install_panel.sh && bash install_panel.sh
```

## 脚本3：宝塔破解版

* 来源: [https://baota.sbs/](https://baota.sbs/)

Centos安装命令：

```
yum install -y wget && wget -O install.sh https://install.baota.sbs/install/install_6.0.sh && sh install.sh
```

Ubuntu/Debian安装命令：

```
wget -O install.sh https://install.baota.sbs/install/install_6.0.sh && bash install.sh
```


## 脚本5：宝塔开心版

* 来源: [https://www.btkaixin.net/](https://www.btkaixin.net/)

Linux面板7.9.10安装脚本 专业版：

Centos安装命令：

```
yum install -y wget && wget -O install.sh http://www.btkaixin.net/install/install_6.0.sh && sh install.sh
```

Ubuntu/Debian安装命令：

```
wget -O install.sh http://www.btkaixin.net/install/install_6.0.sh && bash install.sh
```

一键更新脚本：

```
curl http://www.btkaixin.net/install/update6.sh|bash
```

## 脚本5：宝塔 hostcli

* 来源：[https://www.hostcli.com/](https://www.hostcli.com/) 宝塔 7.6.0版本 [推荐/稳定版本]

Centos全新安装命令：根据系统执行框内命令开始安装（大约2分钟完成面板安装）升级后可能需要重启面板

```shell
yum install -y wget && wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && sh install.sh
```

Ubuntu/Deepin全新安装命令：

```shell
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && sudo bash install.sh
```

Debian全新安装命令：

```shell
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && bash install.sh
```

Fedora全新安装命令:：

```shell
wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && bash install.sh
```

已经安装官方面板，执行下列命令升级到7.6.0纯净版：

```shell
curl http://v7.hostcli.com/install/update6.sh|bash
```

其他非官方版本(含开心版、快乐版、纯净版等 7.4.5至7.6.0版本之间所有版本均可)，执行下列命令升级到7.6.0纯净版：

```shell
curl http://v7.hostcli.com/install/update6.sh|bash
```

任意非官方版本还原到官方最新版

```shell
curl http://download.bt.cn/install/update6.sh|bash
```

## 引用

- <https://www.toutiao.com/article/7522003161985466906/>
- <https://www.roamacg.com/1193.html>
- <https://www.hostcli.com/>
