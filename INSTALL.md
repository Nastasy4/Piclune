# Install & update / 安装与更新

## English

1. Use an Apple Silicon Mac (M-series), running macOS 15 or later. Intel Macs are not supported.
2. Download `Piclune-0.7.0-beta.2-arm64.zip` from this repository's release assets.
3. Compare its SHA-256 with `SHA256SUMS.txt` from the same release if desired: `shasum -a 256 Piclune-0.7.0-beta.2-arm64.zip`. A checksum detects file changes; it does not replace an identified developer signature.
4. Unzip, quit any running Piclune, and drag Piclune.app into Applications. Replacing an older app preserves its existing preferences.
5. Open the app. **This beta is ad-hoc signed, not Developer ID signed or Apple-notarized.** If macOS blocks it as an unidentified/unverified developer, only if you trust the download, follow Apple's [official first-open instructions](https://support.apple.com/en-us/102445): System Settings → Privacy & Security → Open Anyway, then confirm Open. Availability depends on system policy; managed Macs may prohibit it.
6. If macOS reports malware, revoked authorization, or a damaged/modified app, stop and check the download/report the issue. Do not disable Gatekeeper, SIP, or antivirus protection. No Terminal security-bypass command is required by these instructions.

Language: Settings → General → Language → System Default / English / 简体中文. Quit with ⌘Q and reopen for language changes, including system menus, to take effect. When following the system, Piclune uses the first supported language in your preference list (Chinese or English); otherwise English. Chinese variants use Simplified Chinese because Traditional Chinese is not included in this beta.

Optional default viewer: Settings → Formats. Choose only the formats you want, then apply. This does not change your files. To restore Preview later, use Finder → Get Info → Open With → Preview → Change All for each file type.

Updates are manual: download a newer release, quit, and replace the application. There is no automatic online updater. Remove the app from Applications to uninstall; preferences may remain in macOS.

## 简体中文

1. 使用 M 系列 Mac，系统为 macOS 15 或更新版本；不支持 Intel。
2. 在 Releases 下载 `Piclune-0.7.0-beta.2-arm64.zip`，不要下载自动生成的源码压缩包。
3. 如需核对完整性，运行 `shasum -a 256 Piclune-0.7.0-beta.2-arm64.zip`，与同一版本 `SHA256SUMS.txt` 比较。校验和不能替代开发者身份认证。
4. 解压，退出旧版，将 Piclune.app 拖入“应用程序”并替换。已有偏好会保留，不强制恢复新默认值。
5. 本包没有 Developer ID 签名和 Apple 公证。若系统提示无法验证开发者，只有在确认下载可信时，才按 [Apple 官方说明](https://support.apple.com/en-us/102445)到“系统设置 → 隐私与安全 → 仍要打开”，再确认打开。受管理的电脑可能禁止此操作。
6. 若提示恶意软件、授权撤销或文件损坏／被修改，应停止并核对下载、反馈问题。不要关闭 Gatekeeper、SIP 或安全软件。本说明不要求执行终端绕过命令。

语言：设置 → 通用 → 语言。选择后用 ⌘Q 退出并重新打开，使应用和系统菜单一起更新。跟随系统时按系统偏好顺序选择中文或英文，均不匹配则使用英文。本版所有中文变体统一使用简体中文。

默认看图器：设置 → 格式，选择需要关联的格式后应用。撤销时在访达“显示简介 → 打开方式 → 预览 → 全部更改”中逐格式恢复。

更新为手动下载与替换，没有联网更新检查。卸载时删除应用即可；macOS 中可能保留偏好。
