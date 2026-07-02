<div align="center">

# MoonProxyHQ · 月神代理

**把内网服务，拥有公网地址。一键完成。**

GUI desktop client for [fatedier/frp](https://github.com/fatedier/frp) —
intranet exposure with no command line, no config files, no router wrangling.
**macOS · Windows · MIT · 开源免费**

<br/>

<a href="https://moonproxy.app/"><img src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87%E5%AE%98%E7%BD%91-moonproxy.app-2563eb?style=for-the-badge" alt="中文官网"></a>
<a href="https://moonproxy.app/en/"><img src="https://img.shields.io/badge/English-moonproxy.app/en-2563eb?style=for-the-badge" alt="English site"></a>
<a href="https://github.com/MoonProxyHQ/moonproxy-desktop/releases/latest"><img src="https://img.shields.io/github/v/release/MoonProxyHQ/moonproxy-desktop?include_prereleases&style=for-the-badge&label=%E4%B8%8B%E8%BD%BD&color=brightgreen" alt="立即下载"></a>

<br/>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/MoonProxyHQ/moonproxy-desktop/blob/main/LICENSE)
[![Tauri v2](https://img.shields.io/badge/Tauri-v2-blue)](https://tauri.app)
[![Vue 3](https://img.shields.io/badge/Vue-3-brightgreen)](https://vuejs.org)
[![Rust](https://img.shields.io/badge/Rust-orange)](https://www.rust-lang.org)

</div>

---

## 我们做了什么

**月神代理**（MoonProxy）是一款让**非技术用户**也能玩转**内网穿透**的
桌面应用。你有一台本地的服务（家里的 NAS / 公司 ERP / 自己搭的 Minecraft
服务器 / 本地起的博客）想放到公网上——以往要么折腾路由器端口转发，要么
学 frp 命令行，要么花钱用 ngrok。MoonProxy 把这件事变成「像填表一样新增隧道，
像点开关一样启停」。

- **零命令行** · 像填表一样配置 TCP / UDP / HTTP / HTTPS 隧道
- **可视化状态** · 启动按钮分 4 态（已停止 / 连接中 / 已连接 / 连接错误），
  「已连接」由 frpc 真实证据驱动
- **健康监测** · 每 3 秒探测本地端口可达性，提前发现隧道断裂
- **系统托盘常驻** · 关窗即收托盘，服务不停
- **开机自启** · 自启即静默，不打扰工作
- **定时连接** · 按星期 + 时段自动启停，不在公网留任何入口
- **引擎自更新** · frpc 从上游 GitHub Release 拉取，SHA256 校验后原子替换
- **应用自更新** · 基于 `tauri-plugin-updater` 的「重启并安装」

## 核心仓库

| 仓库 | 说明 |
| --- | --- |
| [MoonProxyHQ/moonproxy-desktop](https://github.com/MoonProxyHQ/moonproxy-desktop) | 桌面应用源码（Tauri v2 + Vue 3 + Rust + TypeScript） |

## 链接

- 官网：[https://moonproxy.app](https://moonproxy.app/) · [English](https://moonproxy.app/en/)
- 下载：[GitHub Releases](https://github.com/MoonProxyHQ/moonproxy-desktop/releases/latest)
- 文档：[moonproxy-desktop/README](https://github.com/MoonProxyHQ/moonproxy-desktop#readme)
- LLM 友好摘要：[llm.txt](https://moonproxy.app/llm.txt) · [llm-full.txt](https://moonproxy.app/llm-full.txt)
- 社区：[Discussions](https://github.com/MoonProxyHQ/moonproxy-desktop/discussions)
- 安全：[security@moonproxy.app](mailto:security@moonproxy.app)
- 状态页：[moonproxy.app](https://moonproxy.app/)（域名即产品页）

## 适用场景

- 🏠 **家里有 NAS** —— 出差路上也能取文件
- 🏢 **远程办公** —— 公司 ERP / OA 不用 VPN 也能访问
- 🎮 **联机游戏** —— Minecraft / Palworld / Terraria 跟朋友联机不用端口转发
- 💻 **本地 Web 服务** —— AI 生成的网页 / 本地起的博客 / 演示页一条链接发出去
- 🔌 **远程桌面** —— 远程连回家里的电脑 / 树莓派

## 技术栈

- **应用框架**：[Tauri v2](https://tauri.app)（Rust core + WebView UI）
- **UI**：[Vue 3](https://vuejs.org) + TypeScript
- **穿透引擎**：[fatedier/frp](https://github.com/fatedier/frp) frpc（二进制
  通过 Tauri sidecar 机制打包）
- **构建**：Vite + pnpm + GitHub Actions
- **部署**：Cloudflare Pages

## 独立声明

MoonProxy / 月神代理 **与 fatedier/frp 项目相互独立**。frp 的发布与许可
归原项目所有；MoonProxy 仅作为其桌面 GUI 客户端。

## 联系

- Bug / Feature：[GitHub Issues](https://github.com/MoonProxyHQ/moonproxy-desktop/issues)
- 讨论：[GitHub Discussions](https://github.com/MoonProxyHQ/moonproxy-desktop/discussions)
- 安全报告：[security@moonproxy.app](mailto:security@moonproxy.app)

---

<div align="center">
<sub>Made with Tauri v2 + Vue 3 + Rust. © MoonProxyHQ.</sub>
</div>
