# Piclune 0.7.0 Public Beta 2 — Build 30

A free native image viewer for folder-based workflows on Apple Silicon Macs.

## Changes

- A pure white app icon with flat, layered photo panes. No letter monogram.
- Mouse-wheel zoom uses a larger 20% step for non-precise wheel events. Precise/smoothed wheel input remains integrated and rate-limited.
- Reversing the wheel discards the previous pending destination immediately. Zoom responds quickly and eases into its destination.
- Zooming out across Fit to Window snaps and recenters, with a short detent before further zooming out. Respect the zoom snapping preference and Reduce Motion.
- Image and thumbnail navigation share a fixed 0.38-second transition. Removed the duration setting.
- Preload count sits beside its stepper. Clearer distinction between full-image preload and the image cache budget.
- Thumbnail generation and background aspect-ratio reading have separate queues. Strip and overview reuse the largest cached thumbnail, showing an existing preview before a higher-resolution version arrives.
- Resolve symbolic paths before folder scanning and selection.
- Overview metadata arrives in growing batches instead of waiting for the entire folder.

Download `Piclune-0.7.0-beta.2-arm64.zip` and `SHA256SUMS.txt`.

**Apple Silicon only; macOS 15+. Liquid Glass UI requires macOS 26+. This beta is ad-hoc signed, without Developer ID signing or Apple notarization.** [Installation](https://github.com/Nastasy4/Piclune/blob/main/INSTALL.md) · [Known limitations](https://github.com/Nastasy4/Piclune/blob/main/KNOWN-ISSUES.md)

## 中文

- 新白底图标，以叠放照片表达产品用途，扁平主体配少量玻璃层次。
- 鼠标普通滚轮每步调整为 20%；平滑滚轮继续积分与限速，避免一次滚动膨胀数倍。
- 反向滚动立即丢弃旧目标；缩放快速响应后缓缓收尾。缩小经过适合窗口时吸附并居中，短暂停留后可继续缩小。
- 切图与缩略图导航统一 0.38 秒，移除动画时长设置；精简缓存说明，数量紧邻增减箭头。
- 修正符号链接路径的选择匹配，并补充回归测试。
- 缩略图与后台尺寸读取分离；总览和缩略图栏复用缓存，已有小预览可先显示；瀑布流尺寸分批到达。

没有新增联网能力，图片仍在本机处理。预载入上限仍为每侧 8 张；加大原图预载入不能直接加快缩略图，可能加重解码与内存压力。首次读取超大图片或慢速磁盘仍可能等待。

99 项自动化测试通过。其他 macOS 版本、实际鼠标／平滑滚动工具和不同刷新率屏幕仍需用户测试。
