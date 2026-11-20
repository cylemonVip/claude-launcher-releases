# Claude 启动器

为 macOS 上的官方 Claude 桌面版提供独立代理连接、网络环境检测与断网保护。

**[下载最新版本](https://github.com/cylemonVip/claude-launcher-releases/releases/latest)** · 当前公开版本 **3.2.6** · Apple Silicon Mac／macOS 14+

3.2.6 修复 Claude 打开后偶发无法联网的问题，并增加本机累计上传、下载流量。重启或覆盖升级后可继续累计，点击「Claude 流量」卡片右上角的「清零」并确认即可重新统计。[3.2.6 发行说明](https://github.com/cylemonVip/claude-launcher-releases/releases/tag/v3.2.6)

干净 Mac 首次安装、完整系统故障矩阵和公网邮件登录的完整流程尚未完成实机验收。初版功能及验证范围见 [3.0.0 发行说明](https://github.com/cylemonVip/claude-launcher-releases/releases/tag/v3.0.0)。

## 下载与安装

- 当前支持 Apple Silicon Mac、macOS 14 及以上；Windows 版暂未提供。
- 请先安装官方 Claude 桌面版，并准备自己的 HTTP／HTTPS 代理订阅。
- 下载发行附件中的 `ClaudeLauncher-<版本>-arm64.zip`，解压后将“Claude 启动器.app”放入“应用程序”。
- 首次打开按引导登录邮箱账号、启用网络保护，并完成 macOS 的必要授权。服务有效期与试用以账号页面显示为准。
- 点击“新增订阅”保存链接，选择一条订阅并连接代理，选好节点后点击“检测并打开 Claude”。

正式安装包使用 Developer ID 签名及 Apple 公证，不需要 Xcode 或开发者账号。具体安装与保护范围见 [安装说明](INSTALL.md)。

## 更新

启动器中的“检查更新”会查询此仓库的最新正式版本，并提供 GitHub 下载入口。当前采用手动下载安装；替换应用前先保存工作并安全退出 Claude，再退出启动器。账号、订阅等本机数据沿用已有存储。

已启用 Guard 2.2.7 的用户可直接替换启动器。如果仍使用旧版 Guard，请保持 Claude 完全退出，进入「设置 → 安装与修复」，在「启用网络保护」下点击「启用保护」。按 macOS 提示授权或重启，确认保护已生效后，再连接代理并点击「检测并打开 Claude」。

也可以直接访问 [Releases](https://github.com/cylemonVip/claude-launcher-releases/releases) 查看版本说明。下载发行附件中的安装包；GitHub 自动生成的 `Source code` 文件只包含本仓库文档，不能安装。详细步骤见 [升级说明](UPGRADING.md)。

## 保护范围

本产品不修改或重签官方 Claude.app。网络保护针对当前用户的官方 Claude 及已支持的 Helper；其他应用、外部浏览器、Claude Code、MCP 和外部工具不自动纳入。断开或关闭启动器后，Claude 网络会被阻断；网络检测结果不等同于 Claude 账号安全保证。

## 完全卸载与恢复 Claude 联网

> [!IMPORTANT]
> 如果把启动器直接拖进废纸篓，macOS 可能仍保留 Claude 专用的网络配置和保护组件。即使启动器已经删除，直接打开 Claude 仍可能无法联网。要恢复 Claude 直接启动时的正常联网，请先使用启动器内的「完全卸载启动器」完成清理。

1. 保存工作并完全退出 Claude，然后打开启动器。
2. 进入「设置 → 安装与修复 → 完全卸载启动器」，按向导移除 Claude 专用网络配置、网络过滤器和系统扩展。
3. 若提示重启 Mac，重启后重新打开启动器并继续卸载。向导确认清理完成后，点击「移到废纸篓并退出」。
4. 卸载完成后，直接打开 Claude，它会使用 macOS 当前的网络连接。

如果已经手动删除启动器，请先从废纸篓恢复到「应用程序」，或从发行页重新下载安装，再运行完全卸载向导。

## 反馈与许可

- 问题反馈请使用 [Issues](https://github.com/cylemonVip/claude-launcher-releases/issues)，附 macOS 版本、启动器版本及复现步骤。请勿公开订阅地址、验证码、个人账号或聊天内容。
- 本仓库用于产品发行与用户文档，自研客户端和服务端源码不在本仓库公开。
- 第三方组件按各自许可证提供，详见 [第三方组件说明](THIRD_PARTY.md)。本项目与 Anthropic 无隶属关系，不是官方 Claude 产品。
