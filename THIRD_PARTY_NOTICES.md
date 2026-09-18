# 第三方组件声明 / Third-Party Notices

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
