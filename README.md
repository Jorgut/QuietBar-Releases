# QuietBar

QuietBar is a native macOS utility that makes a crowded menu bar calmer and
easier to manage. Place less-used items to the left of the QuietBar divider,
then reveal or compact them with one click.

**Chinese name:** 悄悄吧

[Product website](https://quietbar.altn.vision) ·
[Privacy policy](PRIVACY.md) ·
[Support](SUPPORT.md) ·
[Release notes](CHANGELOG.md)

> **Release status**
>
> QuietBar 1.0 build 6 is the current Mac App Store release candidate. No
> public binary is attached yet. Download QuietBar only from this repository or
> the Mac App Store after an official release is published.

## Why QuietBar

Chat, design, development, networking, and system utilities can quickly fill a
Mac menu bar, especially on MacBook displays with a notch. QuietBar gives those
items a compact area without quitting their applications or changing their own
settings.

## Features

- Reveal or compact menu bar items with one click.
- Open the QuietBar panel with a right-click.
- Show recognized application names and icons when Accessibility access is
  enabled.
- Group duplicate items from the same application.
- Refresh detected menu bar items live.
- Launch automatically at login.
- Compact automatically after 5, 15, 30, or 60 seconds, or remain expanded.
- Toggle globally with `Control-Option-Q` (`⌃⌥Q`).
- Switch between English and Simplified Chinese.
- Operate locally without an account, analytics, advertising, or cloud storage.

## Requirements

- macOS 13.0 or later.
- Apple silicon or Intel Mac.
- Accessibility permission is optional for reveal/compact behavior and is used
  locally for application-name and icon recognition.

## First Setup

1. Open QuietBar and leave the menu bar expanded.
2. Hold `Command` and drag the items you want to compact to the left of the
   QuietBar divider.
3. Left-click the QuietBar icon to reveal or compact those items.
4. Right-click the icon to open the panel and preferences.
5. To display available application names and icons, enable QuietBar in
   **System Settings > Privacy & Security > Accessibility**.

## Privacy

QuietBar processes menu bar information on your Mac. It does not require an
account, upload menu bar information, or include analytics and advertising
SDKs. See [PRIVACY.md](PRIVACY.md) for the complete policy.

## Known Limitations

- Some macOS helper processes, including `SystemUIServer` and
  `TextInputMenuAgent`, do not provide a standalone application icon.
- Some third-party menu bar apps expose incomplete Accessibility metadata, so
  their name or icon may be unavailable.
- Broader runtime testing on older macOS releases, unusual multi-display
  layouts, and full-screen spaces remains part of release validation.

## Current Verification

- Version 1.0 build 6 archives successfully for the Mac App Store.
- The signed archive contains App Sandbox and Accessibility entitlements.
- The release candidate contains Apple silicon and Intel architectures.
- All 24 unit tests pass.
- The application bundle contains only production assets and localization
  resources.
- The product website, English demonstration video, interactive web demo, and
  localized App Store screenshots are prepared.

## Downloads

There is currently no official downloadable build. A GitHub Release will be
published only after the package has the appropriate Apple signing,
notarization, and Gatekeeper validation. The Mac App Store release will be
linked here after it becomes publicly available.

## Source and License

This repository is the official public release, support, and documentation
surface for QuietBar. The development source repository remains private. No
open-source license has been granted.

Copyright 2026 Altankhuu JORGUTYN. All rights reserved.

---

## 中文简介

悄悄吧是一款原生 macOS 菜单栏整理工具。将暂时不用的图标拖到分隔线左侧，
之后即可一键展开或收起。它支持开机启动、自动收起、全局快捷键、程序名称与
图标识别，以及中英文切换。所有信息均在本机处理，不需要账号，也不包含广告或
分析追踪。

当前版本为 1.0 build 6 App Store 候选版，尚未提供公开安装包。正式发布后，
请仅从本仓库或 Mac App Store 下载。
