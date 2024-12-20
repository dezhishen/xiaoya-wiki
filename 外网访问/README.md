# 小雅外网访问指南
# 免责申明：
- **本指南仅用于个人学习交流，请勿用于商业用途。**
- **本指南仅供参考，请根据实际情况选择合适的方法。**
- **本指南可能存在错误，请以实际情况为准。**
- **本指南不推荐使用任何商业服务，请自行甄别。**
## 1.基础知识介绍
### 1.1.什么是内网/外网
- [什么是内网/局域网(百度百科)](https://baike.baidu.com/item/%E5%B1%80%E5%9F%9F%E7%BD%91/98626)
- [什么是外网/互联网(百度百科)](https://baike.baidu.com/item/%E4%BA%92%E8%81%94%E7%BD%91/199186)
### 1.2.什么内网穿透
- [内网穿透是什么？(百度百科)](https://baike.baidu.com/item/%E5%86%85%E7%BD%91%E7%A9%BF%E9%80%8F/8597835)
### 1.3.什么是cloudflared
- [cloudflared是什么？(Cloudflare官网)](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/)
- [gihub.com/cloudflare/cloudflared](https://github.com/cloudflare/cloudflared)
### 1.4.场景内网穿透的技术方案
#### 1.4.1.ssh隧道
SSH 隧道（SSH Tunneling），又称为 SSH 端口转发（SSH Port Forwarding），是一种利用SSH协议为其他协议或网络链接加密的方法。通过SSH隧道，用户可以安全地传输未加密的网络流量，通过远程服务器转发到目标目的地，保证了数据传输的私密性和安全性。
#### 1.4.2.frp
frp 是一个快速反向代理工具，支持 TCP、UDP、HTTP、HTTPS 等多种协议。
- [github.com/fatedier/frp](https://github.com/fatedier/frp)
#### 1.4.3.nps
nps 是一个轻量级、高性能、分布式的内网穿透工具，支持 TCP、UDP、HTTP、HTTPS 等多种协议。
- [github.com/ehang-io/nps](https://github.com/ehang-io/nps)
### 1.5.什么是异地组网
- 异地组网是一种将处于不同地理位置的局域网（LAN）或分支机构通过一种网络连接起来的过程，形成一个虚拟的广域网（WAN）的技术和方法。 简单来说，它是以网络连接为手段，将不同地理位置的设备和网络连接起来，以实现远程协同工作、资源共享和数据交换等目的。
- 完成异地组网后，异地的资源会形成一个虚拟的局域网，可以像在本地一样访问异地的资源。
### 2.1.frp供应商服务
请自行检索frp供应商服务，**务必遵守供应商服务条款。**
### 2.2.自建frp服务
- 参考[frp官方仓库](https://github.com/fatedier/frp/blob/master/README_zh.md)
- 参考[frp官方文档](https://gofrp.org/zh-cn/)
### 2.3.自建nps服务
- 参考[nps官方仓库](https://github.com/ehang-io/nps)
- 参考[nps官方文档](https://ehang.io/nps/documents)
## 3.异地组网
### 3.1.ZeroTier
//todo 推荐教程
### 3.2.Tailscale
//todo 推荐教程
### 3.3.Ngrok
//todo 推荐教程
## 4.cloudflared
### 4.1.先决条件
- 一个域名
- 一个cloudflared账号
### 4.2.cloudflared安装
//todo 推荐教程
### 4.3.cloudflared配置
//todo 推荐教程
### 4.4.一键脚本