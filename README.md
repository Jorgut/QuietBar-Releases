# QuietBar

QuietBar 是一款轻量、原生、注重隐私的 macOS 菜单栏整理工具。它用一个简单的分隔区域收起暂时不需要的菜单栏图标，需要时可以一键展开，让有限的菜单栏空间重新安静下来。

QuietBar is a lightweight, native, privacy-focused macOS utility that compacts less-used menu bar items and reveals them again with one click.

> **发布状态 / Release status**
>
> 首个公开测试版正在进行 Developer ID 签名与 Apple 公证准备。目前还没有官方安装包，请勿从其他来源下载。
>
> The first public beta is awaiting Developer ID signing and Apple notarization. No official binary is available yet.

## 为什么做 QuietBar

当聊天、设计、网络、同步和开发工具同时常驻时，Mac 菜单栏很快就会被塞满；在带刘海的 MacBook 上，空间更加有限。QuietBar 的目标不是取代这些程序，而是让你决定哪些图标保持可见，哪些图标暂时收起。

## 核心功能 / Features

- 一键展开或收起 QuietBar 分隔线左侧的菜单栏项目。
- 通过辅助功能权限读取可用的项目名称，并展示对应程序图标。
- 默认 15 秒后自动收起，可选择 5、15、30、60 秒或从不自动收起。
- 使用全局快捷键 `Control-Option-Q`（`⌃⌥Q`）快速切换。
- 支持登录时自动启动。
- 中文与英文界面可随时切换，选择会保存在本机。
- 实时刷新菜单栏项目状态。
- 不要求账号，不包含广告、分析追踪或云端服务。

## 工作方式

QuietBar 创建两个属于自己的 macOS 状态栏项目：控制按钮和分隔区域。收起时，分隔区域会占用菜单栏空间，把位于其左侧的项目推离当前可视区域；展开时恢复正常宽度。

QuietBar 不会改写第三方应用的隐藏设置，也不会永久删除系统菜单栏项目。退出 QuietBar 后，它创建的分隔区域会被系统移除。

## 第一次使用 / First setup

1. 启动 QuietBar，先让菜单栏保持展开。
2. 按住 `Command`，将希望收起的图标拖到 QuietBar 分隔线左侧。
3. 左键点击 QuietBar 图标进行展开或收起。
4. 右键点击图标打开项目面板；点击齿轮进入 QuietBar 设置。
5. 如需显示项目名称和程序图标，在 **系统设置 → 隐私与安全性 → 辅助功能** 中启用 QuietBar。

## 下载与安装 / Download and installation

正式测试包发布后：

1. 从本仓库的 **Releases** 页面下载最新的 `QuietBar` 压缩包。
2. 对照发布页提供的 SHA-256 校验值。
3. 解压并将 `QuietBar.app` 拖入 `/Applications`。
4. 首次启动后按应用内引导完成菜单栏排列和权限设置。

每个官方包都会经过 Developer ID 签名、Apple 公证和 Gatekeeper 验证。在这些步骤完成前，本仓库不会提供安装包。

## 系统要求 / Requirements

- 当前测试目标：macOS 26.5 或更高版本。
- 首个公开包的处理器支持范围会在 Release 页面明确标注。
- 辅助功能权限仅用于读取菜单栏项目名称和位置；不授权时仍可使用基础展开与收起功能。

## 隐私 / Privacy

QuietBar 在本机处理菜单栏信息，不上传菜单栏内容，不需要账号，也不包含分析或广告 SDK。完整说明见 [PRIVACY.md](PRIVACY.md)。

## 支持与故障排查

常见问题和反馈要求见 [SUPPORT.md](SUPPORT.md)。版本变化见 [CHANGELOG.md](CHANGELOG.md)。

## 发布路线 / Roadmap

- Developer ID 签名与 Apple 公证。
- 多显示器、刘海屏、全屏空间、休眠唤醒和登录启动真人测试。
- 发布免费 GitHub 公测版并收集首批用户反馈。
- 根据反馈评估兼容更早 macOS 版本及独立的 Mac App Store 精简版。

## 源代码与授权

QuietBar 当前计划作为免费软件发布。源代码保存在私有仓库中，本公开仓库只提供官方安装包、校验值、发布说明和支持文档。
