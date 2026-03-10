# 神衍 Code (Logorythia Code)

<div align="center">


**演化万物，连接未来**

[官网](https://huaxiaxufu.com/LogorythiaCode) · [反馈](https://huaxiaxufu.com/support)

</div>

---

## 简介

自然语言驱动的 AI 编程助手，通过描述需求即可完成代码编写、Bug 修复、代码重构与功能开发。内置浏览器支持文档查阅、资料搜索与文件下载，交互式终端允许 AI 执行 shell 命令，快照系统实现工作状态的保存与回滚，跨会话记忆能力确保上下文连续性。

### 核心能力

| 模块 | 说明 |
|------|------|
| 浏览器 | 多模态浏览器自动化，支持认证、会话管理与文件下载 |
| 终端 | 持久化 PTY 终端，支持 venv、SSH 与交互式 Shell |
| 快照 | 代码变更追踪与回滚，自动附加快照 ID 到上下文 |
| 调试 | 智能 UI/UX 调试，支持 iOS/macOS 与 Web 前端 |
| 记忆 | 双脑记忆架构，上下文感知的记忆片段 |
| 编码 | 智能代码编辑与重构 |

> 部分功能暂时不在 CLI 版本中提供，接下来会进一步完善。

> CLI和桌面端的发展方向略有差异。CLI发展方向为自进化，桌面端为与人更友好的协作。
---

## 系统要求

### 桌面版
- macOS 26.0+

### CLI版
- Linux：
  - Ubuntu 22+
  - debian 12+
  - 尚未进行更广泛的测试，但安装脚本有对各发行版提供支持。
    
  ! 由于 `Apline` 缺少 `Glibc` 或许永远都不会提供支持。

- macOS 15.0+
- WSL2 至少搭配 Ubuntu 22+

> **版本状态**：macOS、CLI 版本正在公测中。CLI Windows版本稍后公测。Windows WinUI版本预计夏季公测。

---

## 下载与安装

### 桌面版
当前仅 macOS 版本提供桌面版。

#### 下载
1. 访问本仓库的 [Releases](../../releases) 页面
2. 访问 [神衍 Code 官网](https://huaxiaxufu.com/LogorythiaCode) 下载最新版本。

---
### CLI：
#### 如果您使用 macOS、Linux
```bash
curl -fsSL https://huaxiaxufu.com/api/logorythiaCode/cli | bash
```
在终端中运行此命令以自动完成环境配置与安装。

##### 如果您使用 Windows
目前 Windows 版本还不支持 `ps` 版本。您需要使用 `WSL` 来运行。
```
wsl --install
curl -fsSL https://huaxiaxufu.com/api/logorythiaCode/cli | bash
```
---

## 常见问题

### Q: 神衍 Code 是否免费？
A: 神衍 Code 完全免费。公测期间不提供模型服务，推荐您自行配置 codingPlan。

### Q: 如何获取技术支持？
A: 您可以通过以下方式获取帮助：
- 访问 [官网支持页面](https://huaxiaxufu.com/LogorythiaCode/support)
- 在本仓库提交 Issue

### Q: 数据安全如何保障？
A: 神衍 Code 重视用户隐私，所有代码数据均经过加密处理，详情请参阅[隐私政策](https://huaxiaxufu.com/law/privacy)。

---

## 相关链接

- [官方网站](https://huaxiaxufu.com/LogorythiaCode)
- [技术支持](https://huaxiaxufu.com/support)

---

## 许可证

使用本软件即表示您同意神衍 Code 的使用条款和隐私政策。

---

<div align="center">

**© 2025-2026 华夏旭府（北京）科技有限公司**

</div>

