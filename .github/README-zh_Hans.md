# Moonlit Echoes Theme

[English](https://github.com/MeesuMaes/SillyTavern-MoonlitEchoesTheme) | **简体中文** | [繁體中文](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/README-zh_Hant.md)

![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_screen_demo_preview.jpg)

**Moonlit Echoes 月下回声** 是一款为 SillyTavern 设计的 UI 主题。它基于我的个人偏好进行了定制和优化，旨在打造一个更加现代、优雅且简约的界面，同时提升桌面端和移动端的用户体验。

Moonlit Echoes 于 2024 年 11 月 25 日首次在 SillyTavern 的 Discord 服务器上发布，并通过社区的宝贵反馈和支持不断更新。最终，为了提高可维护性和更新便利性——同时也为了满足我对精美主题设计的执着追求——我将其开发为 SillyTavern 的扩展程序，并在 GitHub 上开源。

| UI 界面预览 | 视觉小说模式 |
|----------------------|-------------------|
| ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/ui_overview_preview.jpg)     | ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/visual_novel_mode_preview.jpg)    |

## 功能特性

### 核心功能
- 完全兼容 SillyTavern 默认主题，并确保与其他 SillyTavern 扩展无缝集成。
- 针对桌面端和移动端设备进行了优化，提供更宽的输入框和布局调整，以提供更好的体验，特别是为那些对 UI 美学有高要求的用户。
- 包含多种聊天样式，超越了 SillyTavern 内置的“Flat（平面）”、“Bubble（气泡）”和“Document（文档）”样式。可用样式包括“Echo（回声）”、“Whisper（低语）”、“Hush（静谧）”以及新增的“Ripple（涟漪）”。
- 提供丰富的自定义选项，使用户能够根据自己的喜好调整界面。

### Moonlit Echoes 主题预设
用户现在可以轻松分享基于 Moonlit Echoes 主题的配色方案和主题。这些预设可以与 SillyTavern 内置的 UI 主题同步，实现无缝切换。

<img src="https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/Moonlit%20Echoes%20Theme%20Presets.png" width="500">

## 截图
以下截图来自 **版本 1.0.0**，展示于 MacBook（Chrome）。更多 iPhone（Safari PWA）上的截图，请查看项目 [.github 文件夹](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/tree/main/.github)。

| **Flat（平面）** | **Bubble（气泡）** | **Document（文档）** |
|:------:|:--------:|:----------:|
| ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_style_flat_preview.jpg) | ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_style_bubble_preview.jpg) | ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_style_document_preview.jpg) |
| **Echo（回声）** | **Whisper（低语）** | **Hush（静谧）** |
| ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_style_echo_preview.jpg) | ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_style_whisper_preview.jpg) | ![](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme/blob/main/.github/chat_style_hush_preview.jpg) |

## 安装
### 前置条件
建议使用 **最新版本** 的 SillyTavern（Release 或 Staging 版本），并搭配 Google Chrome 浏览器。

### 安装步骤
1. **安装 Moonlit Echoes 主题**：在 **SillyTavern 扩展管理器** 中，使用“从 URL 安装”功能，并粘贴以下 Git 地址：
   ```
   https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme
   ```
2. **禁用缩略图缩放（推荐，以获得更清晰的头像）**：某些消息样式会在背景中显示角色头像。由于 SillyTavern 默认启用了缩略图缩放，这可能会导致模糊。要禁用此功能，请修改 `config.yaml` 文件（位于 `/SillyTavern/config.yaml`），并将 `thumbnails.enabled` 设置为 `false`：
   ```
   thumbnails:
     enabled: false
   ```
3. **下载并启用主题（可选）**：安装完成后，Moonlit Echoes 主题扩展即可使用。然而，如果您希望使用预览图片中展示的样式，请下载并导入 `Moonlit Echoes - by Rivelle.json` 文件到用户设置中，并将其设置为 UI 主题。请勿重命名文件，否则可能导致扩展无法正常工作。

### 针对通过 Termux 使用 SillyTavern 的用户 📱
如果您是通过 Termux 使用 SillyTavern，以下是修改 `config.yaml` 的方法。

> [!警告]
> 我没有 Android 设备或 Termux 的使用经验，因此无法回答相关问题、测试步骤或保证结果。以下方法由其他用户提供。

> [!注意]
> 您可能会在 SillyTavern 文件夹中找到两个 `config.yaml` 文件。请确保编辑根目录下的文件：`/SillyTavern/config.yaml`。**不要修改** `/SillyTavern/default/config.yaml` 或 default 文件夹中的任何内容。

### 方法 1：通过 Termux 编辑
1. 打开 Termux 并输入：`cd SillyTavern`
2. 然后运行：`nano config.yaml` 以编辑文件。

### 方法 2：使用 Material Files（Android 文件管理器）
1. **打开 Material Files** > **添加存储** > **导航到 Termux** > **SillyTavern**
2. 在 SillyTavern 目录中，直接编辑 `config.yaml`

## 使用指南

### 如何使用 Moonlit Echoes 主题预设？
Moonlit Echoes 主题预设部分与 SillyTavern 的 UI 主题同步。如果菜单中有匹配的选项，切换任意一方都会相应同步设置。

然而，Moonlit Echoes 主题预设从根本上独立于 SillyTavern 的 UI 主题。Moonlit Echoes 主题不会创建或修改任何 SillyTavern UI 主题。

### 导入与导出
- Moonlit Echoes 主题预设文件遵循 `[Moonlit] 预设名称.json` 格式（例如 `[Moonlit] Honey Cream.json`）。在 `[Moonlit]` 后有一个半角空格。
- 这不会影响功能。您无需在导入前删除 `[Moonlit]`，直接导入文件即可。
- 如果导入的预设未与 SillyTavern UI 主题同步，请尝试**刷新页面**或**选择其他主题**以应用更改。

## 反馈与建议
如果您遇到任何问题或有功能需求，请在 Issues 部分提交问题，并使用提供的模板。

欢迎您在 Discussions 部分分享您的配色方案！<br>
无论是 SillyTavern UI 主题还是 Moonlit Echoes 主题预设，我都非常期待看到您的创意设计。

## 特别感谢

衷心感谢所有支持和为本项目做出贡献的人。

- 非常感谢 ceruleandeep 在 SillyTavern Discord 中的早期支持——这一切都因您而起。
- 非常感谢 IceFog72 鼓励我创建 SillyTavern 主题，并开发了 [SillyTavern-CustomThemeStyleInputs](https://github.com/RivelleDays/SillyTavern-MoonlitEchoesTheme)，这为我在早期阶段省去了许多麻烦。
- 非常感谢 Bronya-Rand 的开源工作——我从您的 SillyTavern 扩展中学到了很多，并从中汲取了功能布局的灵感。
- 感谢 vesper——我在设计 Ripple 消息样式时参考了您的自定义主题。

最后，向 Wolfsblvt 和 Cohee 表达无尽的感激之情，感谢他们在 SillyTavern 中为第三方扩展添加了 i18n 支持。这极大地改善了非英语用户的体验，我对此深表感谢！

## 许可证
AGPLv3
