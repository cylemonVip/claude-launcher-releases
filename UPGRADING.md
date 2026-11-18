# 升级说明

当前采用 GitHub 下载、手动替换应用的升级方式。

1. 在启动器“设置 → 版本与更新”点击“检查更新”，或直接访问 [GitHub Releases](https://github.com/cylemonVip/claude-launcher-releases/releases)。
2. 阅读新版本说明，下载 `ClaudeLauncher-<版本>-arm64.zip`。请勿下载 GitHub 自动生成的 `Source code` 作为安装包。
3. 保存 Claude 中尚未提交的工作。在启动器点击“安全退出 Claude”，等待退出完成；若提示需要处理，请先完成退出，不要强制结束 Claude。
4. 完全退出旧启动器，将新版“Claude 启动器.app”复制到“应用程序”，替换旧应用。
5. 打开新版。账号和订阅数据沿用本机存储；若提示更新系统网络组件，按“安装与修复”引导完成授权，再重新连接、检测并打开 Claude。

升级时无需先执行“完全卸载”。不要同时运行多个版本的启动器。

发行附件提供 `SHA256SUMS.txt`。可以在终端进入下载目录，执行 `shasum -a 256 -c SHA256SUMS.txt` 检查安装包完整性。

尚未发布正式安装包时，“检查更新”会提示版本准备中；网络错误会提供直接访问下载页的入口。
