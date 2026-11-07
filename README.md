# 神衍 (Logorythia)

<div align="center">


**演化万物，连接未来**

[官网](https://huaxiaxufu.com/LogorythiaCode) · [反馈](https://huaxiaxufu.com/support)

**现在不只是代码！神衍·工作、计算机控制等正陆续上线。**

</div>

## 简介

自然语言驱动的多智能体工作平台，通过描述即可完成办公任务、计算机任务、代码编写、Bug 修复、办公文档创建、表格创建等。内置浏览器专家支持网络检索、浏览器操作等。内置终端专家支持PTY，可协同处理远程ssh与本地。全新记忆系统与上下文架构接近真无限上下文，超长任务更稳定。

### 多智能体专家

自 v0.5.0 版本起，神衍采用全新 `多主多邀请` 架构。拓展能力大幅提升，远超 Skill 机制，兼容 MCP 协议；在工程任务基准中达到与单体相同水准，在分析等任务上大幅领先。

| 专家 | 说明 |
|------|------|
| 负责人 | 负责调度和沟通，但不担任主智能体 |
| 架构师 | 专为架构设计优化 |
| 质量 | 审计代码、文档等质量 |
| 终端 | 拥有 PTY 终端，可处理 SSH、Vim、Sudo 等交互式命令及 alt 备用缓冲区 |
| 浏览器 | 拥有完整浏览器，支持认证、多标签页与复杂文件下载 |
| 文档 | 轻松构建 docx 文档 |
| 表格 | 轻松构建 xlsx 表格 |
| 幻灯 | 轻松构建 pptx 幻灯片 |
| 控制 | 更优秀地操作电脑 |

... 更多专家正在陆续上线，尽请期待。若有需求请在讨论中提出，并提供推荐的技术方案。

以上专家，在开始时由负责人邀请构建初始团队，除负责人外其他成员可自由退出，有除负责人外的其他团队成员时邀请需要经过其他团队成员的同意。根据我们的测试，一般情况下只会激活4位专家，部分情况可激活更多。

### 变更快照与撤销

神衍使用全新终端读写追踪技术。无论智能体使用终端编辑文件还是编辑工具，神衍都会保存变更差异并支持撤销。相较于 Codex 等智能体，神衍不依赖与 Git 或 SVN 等代码管理技术，也不会创建项目目录的全部快照，且变更追踪是针对于当前系统物理连接的所有磁盘（不同系统略有差异）。

#### macOS
在 macOS 上，神衍当前使用 APFS 快照和沙盒技术完成追踪，未来预计换成 ES。

#### Linux 和 Windows
在 Linux 和 Win 上，神衍使用读写追踪拦截技术。

#### 说明

- 全部功能均在 macOS 的 GUI 和 CLI 中提供，部分功能 Linux 和 Win 需要稍后才能提供支持。
- 控制专家目前仅在 macOS 的 GUI 版中提供，Win GUI 版的控制专家稍后随 Win GUI 上线，各端 CLI版及将来的 Linux GUI 版不会提供（但可查看GUI版的聊天历史记录。）

## 系统要求

### 桌面版

- macOS 15.0+ (inter / 苹果硅)

### CLI版

- macOS 15.0+ (inter / 苹果硅)
- Linux 
  - **主程序**：amd64或arm64。 musl 全静态链接编译。
  - **浏览器**：由于涉及 `GTK/WebKit` ，在以下系统会被自动禁用。
    - Ubuntu 20 或更低版本
    - debian 11 或更低版本
    - apline
    
    - 尚未进行更广泛的测试，但安装脚本有对各发行版提供支持。
    - 神衍使用动态识别，若您在这些系统里配置了 GTK 及 WebView 4.0 ，浏览器子智能体会自动激活。

- Windows 11+

> **版本状态**：macOS 桌面、CLI 版本正在公测中。Windows 及 Linux 的桌面版本将于稍后提供。
> 神衍的 CLI 版使用 zxs702/SwiftTUI 构建，支持鼠标点击、滚动等，界面操作与桌面版基本一致。


## 下载与安装

### 桌面版
当前仅 macOS 版本提供桌面版。

> Win GUI 版将于最近开发下载，敬请期待。

#### macOS
1. 访问本仓库的 [Releases](../../releases) 页面
2. 访问 [神衍 Code 官网](https://huaxiaxufu.com/LogorythiaCode) 下载最新版本。

---

### CLI：

#### 如果您使用 macOS、Linux
```bash
curl -fsSL https://huaxiaxufu.com/api/logorythiaCode/cli | bash
```
在终端中运行此命令以自动完成环境配置与安装。

#### 如果您使用 Windows

Windows 现已支持 Logorythia CLI 。在 Windows 上您有两种选择。

###### 安装 msvc 编译的 Logorythia.exe

```pwsh
irm https://huaxiaxufu.com/api/logorythiaCode/cli/win | iex
```

###### 使用 `WSL` 安装 Linux 版本

```bash
wsl --install

# 在 WSL 中运行
curl -fsSL https://huaxiaxufu.com/api/logorythiaCode/cli | bash
```

## 常见问题

### Q: 神衍 Code 是否免费？
A: 神衍 Code 完全免费。您可以自由的配置任何模型，当前我们对国内主流厂商和国际厂商均提供了模型支持。

### Q: 如何获取技术支持？
A: 您可以通过以下方式获取帮助：
- 访问 [官网支持页面](https://huaxiaxufu.com/LogorythiaCode/support)
- 在本仓库提交 Issue

### Q: 数据安全如何保障？
A: 神衍 Code 重视用户隐私，所有代码数据均经过加密处理，详情请参阅[隐私政策](https://huaxiaxufu.com/law/privacy)。


## 相关链接

- [官方网站](https://huaxiaxufu.com/LogorythiaCode)
- [技术支持](https://huaxiaxufu.com/support)

## 许可证

使用本软件即表示您同意神衍 Code 的使用条款和隐私政策。


# 提供帮助
> **如果您期望与我们合作并提供帮助，欢迎与我联系。**
> 
> 知阳：zhiyang@huaxiaxufu.com

<div align="center">

**© 2025-2026 华夏旭府**

</div>
