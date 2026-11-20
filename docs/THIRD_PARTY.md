# 第三方组件

PomiPlayer 使用以下第三方组件。各组件保留原作者的版权和许可证；播放器自有代码的权利说明不改变这些许可。

## 0.1.0 Preview

安装目录的 `licenses` 保存许可原文、Qt SBOM 和来源索引。[Releases](https://github.com/Pumnn1ayLee/PomiPlayer/releases/tag/v0.1.0-preview) 另外提供同一版本的许可资料包，便于在下载播放器前查阅。

| 组件 | 版本与用途 | 上游 |
| --- | --- | --- |
| Qt | 6.10.0，界面和网络，以动态库使用 | [Qt LGPL 义务](https://www.qt.io/licensing/open-source-lgpl-obligations)、[版本源码](https://download.qt.io/archive/qt/6.10/6.10.0/submodules/) |
| libmpv | 0.42.0，官方 Windows x64 LGPL 构建，播放与解码 | [发行版及构建说明](https://github.com/mpv-player/mpv/releases/tag/v0.42.0)、[对应构建脚本](https://github.com/mpv-player/mpv/blob/v0.42.0/ci/build-mingw64.sh) |
| FFmpeg | 8.1.2 Gyan full build，独立的取帧与音轨提取程序，所用 full build 启用 GPL 组件 | [构建来源](https://www.gyan.dev/ffmpeg/builds/)、[许可说明](https://ffmpeg.org/legal.html) |
| whisper.cpp | v1.9.5 CPU 语音转写，MIT | [项目与版本源码](https://github.com/ggml-org/whisper.cpp/tree/v1.9.5) |
| Microsoft Visual C++ runtime | 应用本地运行库 | [再分发说明](https://learn.microsoft.com/en-us/visualstudio/releases/2022/redistribution) |
| NSIS | 安装器生成工具 | [项目及许可](https://nsis.sourceforge.io/License) |

标准包不含模型权重、CUDA 或本地语言模型运行库。表格不列举各运行库内部的全部依赖，具体文件以安装包清单及随附通知为准。

## 尚待补齐的材料

**目前还没有提供完整的第三方对应源码和构建材料套件。** 现有来源索引不等于对应源码本身，尤其还需核对 libmpv 的链接依赖、FFmpeg full build 的依赖和构建细节。此预览版不应被理解为已经完成全部第三方分发要求的确认。

LGPL 组件适用的调试、重新链接及兼容动态库替换权利不受 PomiPlayer 自有代码保护措施限制。自有代码暂不公开，不代表第三方组件也可免除其源码和通知义务。

The installer contains third-party license texts, Qt SBOM files and source references. A separate notices archive is available with the release. **A complete corresponding-source and build-materials bundle has not yet been supplied**, including the remaining checks for libmpv's linked dependencies and the FFmpeg full build. Source references are not claimed to be that bundle. Rights granted by third-party licenses remain unaffected.
