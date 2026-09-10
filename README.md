<p align="center"><img src="media/piclune-icon.png" width="112" alt="Piclune icon"></p>
<h1 align="center">Piclune</h1>
<p align="center">Open one image. Browse the whole folder.</p>
<p align="center">A native, local image viewer for Apple Silicon Macs.</p>

[简体中文](README.zh-CN.md) · [Privacy](PRIVACY.md) · [Installation](INSTALL.md) · [Known limitations](KNOWN-ISSUES.md)

Piclune is a free image viewer for people who organize pictures in folders. Open an image from Finder and browse its neighbors without importing a photo library. A quiet interface, fluid transitions, and configurable controls keep the focus on your pictures.

**0.7.0 Public Beta 2 · Apple Silicon only · macOS 15 or later**

Get the app from this repository's **Releases** section. Download the `Piclune-0.7.0-beta.2-arm64.zip` asset, not GitHub's automatically generated “Source code” archive.

> This beta is ad-hoc signed and is **not Apple-notarized**. macOS may block the first launch. Read the [installation notes](INSTALL.md) before downloading. This is an early public test, not a claim of compatibility with every file or device.

![Piclune — folder browsing with bottom thumbnails](media/viewer.png)

[Download for Apple Silicon](https://github.com/Nastasy4/Piclune/releases/tag/v0.7.0-beta.2)

## A focused way to browse

- Open an image and navigate its folder with the keyboard, mouse, or trackpad.
- Zoom around the pointer, fit to the window, width, or height, and inspect at actual size.
- Keep thumbnails along the bottom or left; pin them, reveal them at the edge, or hide them.
- Switch between square, original-aspect, and waterfall folder overviews.
- View image dimensions, file information, and available EXIF metadata.
- Choose Liquid Glass or Classic styling, light or dark appearance, and your preferred transitions.
- English and Simplified Chinese, with an automatic system-language default and an in-app override.

Liquid Glass requires macOS 26 or later. Earlier supported systems use native fallback materials. HDR requires compatible content and display hardware. Image format support follows the native decoders available on your Mac.

## See the whole folder

A waterfall overview keeps each photo’s proportions, so you can scan the folder visually.

![Piclune waterfall folder overview](media/overview.png)

## Look closer

Keep image dimensions, format, color information, and available metadata beside the picture.

![Piclune image viewer with the information inspector](media/inspector.png)

Photos shown in these screenshots are from Unsplash. [Image credits](SCREENSHOT-CREDITS.md).

## Your pictures stay with you

Piclune does not upload images, filenames, or metadata. No account, ads, analytics, cloud processing, or automatic online update checks. It uses local macOS image decoders and does not invoke third-party Quick Look thumbnail extensions. See [Privacy](PRIVACY.md) for clipboard, cloud-drive, file-access, and system-service boundaries.

## Free to use

The app is free. There is currently no donation prompt or payment system. Optional support may be added later without interrupting image viewing.

This repository is initially prepared as a distribution and feedback repository. Free app distribution does not imply an open-source license for the source code. See [Distribution terms](DISTRIBUTION.md).

## Help improve the beta

Use **Issues** for reproducible bugs and suggestions. Include your macOS version, Mac chip, input device, display, and steps to reproduce. Please do not post private photos, location metadata, full personal file paths, or unredacted crash reports. A synthetic sample is ideal.

Start with the in-app **Help → Piclune Guide**, or read [Getting started](GETTING-STARTED.md).
