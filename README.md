# iP2P Chat

**多协议冗余P2P加密聊天室 | 抗审查 · 端到端加密 · 零服务器**

[![在线访问](https://img.shields.io/badge/%E5%9C%A8%E7%BA%BF%E8%AE%BF%E9%97%AE-ip2pchat.top-brightgreen)](https://ip2pchat.top)

## 项目简介

基于 [webconnect.js](https://webconnect.js.org) 构建的纯前端P2P加密聊天应用。单HTML文件，无需安装，打开即用。

## webconnect.js 是什么？

**[webconnect.js](https://webconnect.js.org) 是一个强大的多协议P2P连接库**，它同时集成了三种去中心化网络协议：

- **WebTorrent** - DHT网络
- **MQTT** - 消息队列协议  
- **Nostr** - 去中心化社交协议

这个库太NB了！它让P2P通信不再依赖单一信令服务器，三种协议冗余备份，任意一种被封锁都能自动切换。WebRTC + 三重协议 = 无敌穿透能力！

## iP2P Chat 做了什么

在 webconnect.js 基础上增加了：

- **端到端加密**：AES-GCM + ECDSA签名
- **身份系统**：本地生成加密指纹，可导出/导入
- **图片传输**：压缩后加密发送
- **多语言界面**：中/英/日/俄

## 核心优势

| 特性 | 说明 |
|------|------|
| 📁 单HTML | 一个文件搞定，无依赖 |
| 🚫 无服务器 | 纯P2P，无中间人可以封杀 |
| 🔐 E2EE | 端到端加密，只有你们能看 |
| 🌐 多协议 | WebTorrent + MQTT + Nostr |
| 🔓 无历史 | 隐私设计，不留痕迹 |
| 🧬 可导出身份 | 指纹可备份，换设备不换身份 |

## 技术栈

- [webconnect.js](https://webconnect.js.org) - 多协议P2P通信引擎
- WebRTC - 浏览器点对点连接
- AES-GCM - 消息加密
- ECDSA - 身份签名验证

## 在线体验

[https://ip2pchat.top](https://ip2pchat.top)

---

> 🤖 **本项目由AI辅助制作**
