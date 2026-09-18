<p align="center">
  <img src="snapora.png" width="96" alt="Snapora">
</p>

<h1 align="center">Snapora</h1>

<p align="center">Windows 截图、标注与贴图工具。捕捉、标注、整理，一切都在本机完成。</p>

> 本仓库只发布 Snapora 的 Windows 安装包和版本说明，不包含源代码。

## 下载与安装

1. 打开 [Releases](https://github.com/Moresyl/Snapora/releases/latest)，下载 `Snapora-<版本>-Setup.exe`。
2. 每个安装包旁边都有同名的 `.sha256` 文件。下载后可以在 PowerShell 中校验：

   ```powershell
   Get-FileHash .\Snapora-1.0.0-Setup.exe -Algorithm SHA256
   ```

   输出的哈希值应与 `.sha256` 文件中的值一致。不一致时请不要安装。
3. 运行安装包。安装需要管理员权限，默认安装到 `C:\Program Files\Snapora`，可以在 Windows「应用」页面卸载。

## 系统要求

- Windows 10 或 Windows 11，64 位
- 不需要注册账号，核心功能不需要联网

## 功能

**截图**

- `F1` 开始截图，快捷键可以在首选项中修改
- 桌面框选、延时截图、截图历史（保留数量可设置）
- 结果可以复制到剪贴板、保存为文件，或直接贴到屏幕上

**标注**

- 画笔、直线、矩形、椭圆、箭头、文字、马赛克、模糊
- 颜色与线宽可调，支持撤销 / 重做
- 文字标注可以随时点回重新编辑，也可以拖动位置

**贴图**

- `F3` 把剪贴板中的图片、文本、HTML 或图片文件贴到屏幕上
- `Shift+F3` 隐藏 / 显示所有贴图
- 旋转、翻转、缩放、透明度；关闭后可以恢复，支持分组和贴图会话保存

**首选项**

- 快捷键、主题、截图历史数量、延时
- 检查更新，可以关闭「启动时自动检查更新」

## 隐私

- 截图、贴图、剪贴板历史、配置文件和运行日志默认只保存在本机。
- 当前版本不会主动上传截图、剪贴板内容、配置或日志。
- 客户端只在检查更新时访问 `snapora.9nn.cn` 获取版本信息，是否下载新版本由你决定。
- 完整说明见 [LICENSE.txt](LICENSE.txt)，内容与安装程序中显示的《隐私说明与使用协议》一致。

## 反馈

- 问题与建议：[GitHub Issues](https://github.com/Moresyl/Snapora/issues)
- 邮箱：hi@9nn.cn
- 博客：https://blog.biekanle.com/

## 第三方组件

Snapora 使用 Qt 等开源组件，各组件的许可证见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

## 版权

© 2026 Mores。保留所有权利。

---

## English

Snapora is a screenshot, annotation and pin-to-screen tool for Windows 10 / 11 (64-bit). This repository only distributes the Windows installer and release notes. The source code is not published here.

- Download `Snapora-<version>-Setup.exe` from [Releases](https://github.com/Moresyl/Snapora/releases/latest) and verify it against the `.sha256` file next to it before installing.
- Everything runs locally. The only network request is the update check against `snapora.9nn.cn`, which can be turned off in Preferences.
- Terms and privacy notice (Chinese): [LICENSE.txt](LICENSE.txt). Third-party licenses: [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
- Feedback: [Issues](https://github.com/Moresyl/Snapora/issues) or hi@9nn.cn.
