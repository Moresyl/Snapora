# Third-Party Notices

**English** | [简体中文](#第三方组件声明)

Every file in the Snapora installer other than `Snapora.exe` is a third-party component distributed under its own license. The table below reflects the files in the installation folder; the installed files are authoritative.

| Component | Files in the installation folder | License | Source |
|---|---|---|---|
| Qt 5.15 (Core, Gui, Widgets, Network, PrintSupport, Svg, plus the platforms / styles / iconengines / imageformats / printsupport plugins) | `Qt5*_conda.dll`, `platforms\qwindows.dll`, `styles\*.dll`, `iconengines\*.dll`, `imageformats\*.dll`, `printsupport\*.dll` | GNU LGPL v3 | https://www.qt.io/ |
| ICU | `icudt78.dll`, `icuin78.dll`, `icuuc78.dll` | Unicode License | https://icu.unicode.org/ |
| libpng | `libpng16.dll` | PNG Reference Library License | http://www.libpng.org/ |
| libjpeg-turbo | `jpeg8.dll` | IJG License / BSD-3-Clause / zlib License | https://libjpeg-turbo.org/ |
| PCRE2 | `pcre2-16.dll` | BSD-3-Clause | https://www.pcre.org/ |
| zlib | `zlib.dll` | zlib License | https://zlib.net/ |
| Zstandard | `zstd.dll` | BSD-3-Clause | https://github.com/facebook/zstd |
| Microsoft Visual C++ Runtime | `MSVCP140*.dll`, `VCRUNTIME140*.dll` | Microsoft Software License Terms (redistributable with applications) | https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist |
| Inno Setup 6 | The installer itself | Inno Setup License | https://jrsoftware.org/isinfo.php |
| Inno Setup Simplified Chinese translation | Installer UI text | Maintained by Zhenghan Yang (Kira) | https://github.com/kira-96/Inno-Setup-Chinese-Simplified-Translation |

## Qt (LGPL v3)

Snapora links Qt 5.15 dynamically and ships the conda-forge build of Qt, which is why the library names carry the `_conda` suffix. Under the GNU LGPL v3:

- The Qt 5.15 source code is available at https://download.qt.io/archive/qt/5.15/ ; the patches and build scripts used by the conda-forge build are at https://github.com/conda-forge/qt-feedstock .
- You may replace the `Qt5*_conda.dll` files and plugins in the installation folder with your own interface-compatible build of Qt 5.15 using the same file names, and Snapora will load them.
- The full text of the LGPL v3 is at https://www.gnu.org/licenses/lgpl-3.0.html .

## Other notes

- Windows API sets (`api-ms-win-*.dll`) are provided by the operating system and are not part of the installer.
- This file only describes third-party licenses. It does not change what the Snapora Privacy Notice and Terms of Use says about Snapora's own behavior.

---

# 第三方组件声明

[English](#third-party-notices) | **简体中文**

Snapora 安装包中除 `Snapora.exe` 以外的文件都是第三方组件，按各自的许可证随软件一起分发。下表以安装目录中的实际文件为准。

| 组件 | 安装目录中的文件 | 许可证 | 来源 |
|---|---|---|---|
| Qt 5.15（Core、Gui、Widgets、Network、PrintSupport、Svg，以及 platforms / styles / iconengines / imageformats / printsupport 插件） | `Qt5*_conda.dll`、`platforms\qwindows.dll`、`styles\*.dll`、`iconengines\*.dll`、`imageformats\*.dll`、`printsupport\*.dll` | GNU LGPL v3 | https://www.qt.io/ |
| ICU | `icudt78.dll`、`icuin78.dll`、`icuuc78.dll` | Unicode License | https://icu.unicode.org/ |
| libpng | `libpng16.dll` | PNG Reference Library License | http://www.libpng.org/ |
| libjpeg-turbo | `jpeg8.dll` | IJG License / BSD-3-Clause / zlib License | https://libjpeg-turbo.org/ |
| PCRE2 | `pcre2-16.dll` | BSD-3-Clause | https://www.pcre.org/ |
| zlib | `zlib.dll` | zlib License | https://zlib.net/ |
| Zstandard | `zstd.dll` | BSD-3-Clause | https://github.com/facebook/zstd |
| Microsoft Visual C++ 运行库 | `MSVCP140*.dll`、`VCRUNTIME140*.dll` | Microsoft Software License Terms（允许随应用再分发） | https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist |
| Inno Setup 6 | 安装程序本身 | Inno Setup License | https://jrsoftware.org/isinfo.php |
| Inno Setup 简体中文翻译 | 安装程序界面文本 | 维护者 Zhenghan Yang (Kira) | https://github.com/kira-96/Inno-Setup-Chinese-Simplified-Translation |

## Qt（LGPL v3）

Snapora 以动态链接方式使用 Qt 5.15，使用的是 conda-forge 发布的构建版本，因此动态库文件名带有 `_conda` 后缀。根据 GNU LGPL v3：

- Qt 5.15 的源代码可以从 https://download.qt.io/archive/qt/5.15/ 获取，conda-forge 构建所用的补丁和构建脚本见 https://github.com/conda-forge/qt-feedstock 。
- 你可以用自行编译的、接口兼容的 Qt 5.15 动态库替换安装目录中的同名 `Qt5*_conda.dll` 和插件文件，Snapora 会继续加载它们。
- LGPL v3 全文见 https://www.gnu.org/licenses/lgpl-3.0.html 。

## 其他说明

- Windows API 集（`api-ms-win-*.dll`）由操作系统提供，安装包不包含这些文件。
- 本文件只说明第三方组件的许可证，不改变《Snapora 隐私说明与使用协议》对 Snapora 自身行为的描述。
