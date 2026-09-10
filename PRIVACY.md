# Privacy / 隐私说明

Applies to Piclune 0.7.0 Public Beta 2 (Build 30). Updated 2026-09-09.

## English

Piclune processes images and metadata on your Mac. The application does not upload images, filenames, metadata, usage events, or crash reports. There are no accounts, advertisements, analytics SDKs, remote image URLs, cloud decoding, or automatic network update checks. Image decoding uses macOS ImageIO/AppKit. Third-party Quick Look thumbnail providers are not invoked.

**Local access:** Opening a file enumerates its parent folder to find neighboring images. Selecting a folder reads that folder. Preferences are stored in the app's UserDefaults domain. Image and thumbnail caches are held in memory; there is no app-managed cloud library or on-disk image cache. macOS may independently retain recent items, system caches, swap, and diagnostic information.

**User-initiated changes:** Rotate and flip affect the viewing state, not the source image. Copy Image writes image data to the system clipboard. Move to Trash moves the selected original file after confirmation by default. Changing default image formats updates macOS file associations only when requested. Showing a file in Finder delegates that action to Finder.

**System boundaries:** iCloud Drive, network volumes, third-party file providers, Universal Clipboard, and system diagnostics follow your macOS/provider settings. Opening an online-only file may cause its provider to download it. Piclune does not control or initiate cloud synchronization itself. Its no-upload promise describes Piclune's application behavior, not a firewall guarantee covering all software on the Mac.

**Permissions:** The GitHub build is not App Sandbox restricted because it browses neighboring files. It runs with the user's ordinary file access, subject to macOS privacy protections. It does not request camera, microphone, contacts, screen recording, accessibility control, or Full Disk Access. If macOS asks for a protected folder, you may decline and choose another folder. No permission is needed to send data to a Piclune service because no such service is used.

**Feedback:** GitHub Issues are a separate online service. Anything you choose to post there may be public. Do not post private images or identifying metadata. There is no automatic in-app feedback upload.

## 简体中文

Piclune 在你的 Mac 上处理图片和元数据，不上传图片、文件名、元数据、使用行为或崩溃报告。应用没有账户、广告、分析 SDK、远程图片 URL、云端解码或自动联网更新检查。图片由 macOS ImageIO/AppKit 解码，不调用第三方 Quick Look 缩略图提供程序。

**本地访问：** 打开一张图片会读取其父文件夹以查找相邻图片；打开文件夹会读取该文件夹。偏好保存在应用的 UserDefaults 中。图片和缩略图缓存位于内存中，没有由应用管理的云图库或磁盘图片缓存。macOS 可能独立保存最近项目、系统缓存、交换文件和诊断信息。

**主动文件操作：** 旋转和翻转只改变查看状态，不改写原图。“复制图像”将图像写入系统剪贴板；“移到废纸篓”会移动当前原文件，默认先确认。只有主动设置默认格式时才修改系统文件关联。“在访达中显示”交给访达执行。

**系统边界：** iCloud、网络磁盘、第三方文件提供程序、通用剪贴板和系统诊断遵循相应的系统或服务设置。打开仅在线保存的文件可能触发提供程序下载。Piclune 本身不控制或执行云同步。“不上传”描述应用行为，不是对整台 Mac 所有软件的防火墙承诺。

**权限：** GitHub 版本为了浏览同目录文件，没有启用 App Sandbox；它使用当前用户普通文件权限，同时受 macOS 隐私保护限制。不会申请摄像头、麦克风、通讯录、录屏、辅助功能控制或完全磁盘访问。系统询问受保护文件夹权限时，可以拒绝并选择其他文件夹。

**反馈：** GitHub Issues 是独立在线服务，主动提交的内容可能公开。请勿上传私人照片或可识别身份的元数据。应用不会自动上传反馈。
