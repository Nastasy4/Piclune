# Beta scope / 测试范围

## English

- Apple Silicon only; macOS 15 minimum. Build 30 was exercised on macOS 27 beta on the development Mac. macOS 15 and 26, other M-series models, external displays, and input devices still need tester coverage. Deployment-target compatibility is not a substitute for running on those systems.
- Liquid Glass is available on macOS 26+. Native material fallbacks are used on macOS 15. HDR depends on the display and image format.
- Native ImageIO/AppKit decoders only. Some files that older Piclune versions displayed using Quick Look may no longer open. RAW support varies by camera and OS. The app is not a medical image interpretation tool.
- The app uses a single viewer window. It is not a multi-window comparison editor or a managed photo library.
- The image cache setting is a budget for cached full images, not a hard cap on process memory. Large/HDR/animated images can use substantially more memory during decoding and display. Lower preloading for large files.
- No frame-rate guarantee is made. Real mouse utilities, trackpads, ProMotion, cold disks, network volumes, very large RAWs, and prolonged browsing need field testing. The synthetic 3000-file scan is not a decode benchmark.
- English and Simplified Chinese only. Language changes require quitting and reopening.
- This beta is not notarized. Installation on managed Macs may be prohibited. Updates are manual.
- The app has no automatic crash reporting. Review and redact any report before sharing it.

## 简体中文

- 仅支持 Apple Silicon，最低 macOS 15。Build 30 在开发机的 macOS 27 测试版上进行了实际检查；macOS 15、26、其他 M 系列机型、外接显示器和输入设备仍需要测试者验证。部署目标正确不等于已经覆盖所有系统实机。
- 液态玻璃需要 macOS 26+；macOS 15 使用原生材质回退。HDR 取决于内容和显示器。
- 仅使用 ImageIO/AppKit 原生解码。旧版曾通过 Quick Look 显示的部分文件可能不再打开。RAW 支持取决于相机型号与系统；不可作为医学图像诊断工具。
- 采用单个看图窗口，不是多窗口比较编辑器或图库管理软件。
- 内存缓存设置只约束完整图片缓存预算，不是进程内存硬上限。大图、HDR 和动图在解码和显示时可能占用更多内存，可降低预载数量。
- 不承诺固定帧率。实体鼠标与平滑滚动工具、触控板、ProMotion、冷盘、网络目录、大 RAW 和长时间使用还需实际覆盖。3000 文件扫描不代表解码性能。
- 仅英文与简体中文，切换语言需要重启应用。
- 未公证，受管理电脑可能禁止安装；更新为手动替换。
- 不自动上传崩溃信息；分享反馈前请自行脱敏。


## Folder access during beta testing

In this macOS 27 beta test environment, opening one image inside Documents could leave the initial folder load waiting. Choosing its containing folder with File → Open Folder (⇧⌘O) completed loading the same 24 images. Folder authorization may be involved; the system-level cause has not been confirmed. If this happens, explicitly choose the folder and report the macOS version and location type.

本轮 macOS 27 测试环境中，从文稿目录打开单张图片曾持续等待；使用“文件 → 打开文件夹”（⇧⌘O）选择所在目录后正常加载。可能涉及文件夹访问授权，系统层根因尚未确认。如遇到此情况，请直接选择文件夹，并反馈系统版本与目录类型。
