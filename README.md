# iP2P Chat

**多协议冗余P2P加密聊天室 | 端到端加密 · 零服务器 · 单HTML文件**

[![在线访问](https://img.shields.io/badge/在线访问-ip2pchat.top-brightgreen)](https://ip2pchat.top)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/zh-CN/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2020-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript)

## 项目简介

这是一个基于 [webconnect.js](https://webconnect.js.org) 构建的纯前端P2P加密聊天演示应用。**单个HTML文件即可运行**，无需安装任何软件，所有逻辑均在浏览器中执行。

> ℹ️ **网络依赖说明**：首次加载时需联网获取 CDN 资源（webconnect.js 库及 CSS 样式文件）。加载完成后，P2P 通信完全依赖 WebRTC 直连，无需中心服务器中转。

webconnect.js 是一个优秀的P2P连接库，它同时集成了 **WebTorrent、MQTT、Nostr** 三种去中心化网络协议作为信令通道，使浏览器之间可以通过WebRTC直接建立连接，无需中心服务器。

## 本项目实现的功能

在 webconnect.js 的基础上，本项目添加了：

- **端到端加密**：使用 AES-GCM 对消息进行加密，ECDSA 进行身份签名
- **身份管理系统**：本地生成加密后的身份指纹，支持导出/导入
- **图片传输**：图片压缩后加密发送
- **多语言界面**：支持中文、英文、日语、俄语
- **在线成员列表**：实时显示房间内在线用户

## 技术特点

- **纯 HTML5 / JavaScript**：原生 Web API 实现，无第三方框架依赖
- **无服务器**：纯P2P架构，没有中心节点可以封禁
- **多协议冗余**：同时使用三种信令协议，单一协议被封不影响连接
- **无历史消息**：端到端加密设计，服务器端不存储任何聊天记录
- **MIT许可证**：完全开源，可自由使用和修改

## 技术栈

| 组件 | 说明 |
|------|------|
| HTML5 | 页面结构与交互界面 |
| JavaScript (ES2020+) | 核心业务逻辑与加密实现 |
| [webconnect.js](https://webconnect.js.org) | 多协议P2P通信引擎 |
| WebRTC | 浏览器点对点连接 |
| Web Crypto API | AES-GCM 加密 / ECDSA 签名 / PBKDF2 密钥派生 |

## 在线体验

[https://ip2pchat.top](https://ip2pchat.top)

## 本地运行

```bash
# 直接下载 HTML 文件，双击即可在浏览器中打开（需允许联网加载CDN资源）
# 或使用本地服务器
npx serve .
```

> ⚠️ **注意**：由于浏览器安全策略，P2P 连接需要 HTTPS 环境（或 localhost）。在线版本已配置 HTTPS，本地运行建议使用 `npx serve` 等支持 HTTPS 的静态服务器，或直接使用 localhost 访问。

## 许可证

MIT License

## 关于项目

⚠️ **仅供学习交流使用**

本项目是一个技术演示，展示了如何在浏览器中实现去中心化P2P加密通信。如果你需要稳定可靠的通信工具，建议使用 Signal、Wire 等成熟的端到端加密通信软件。

---

> 🤖 **本项目由AI辅助制作**
