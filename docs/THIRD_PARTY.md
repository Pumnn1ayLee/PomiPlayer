# 第三方组件 / Third-party components

PomiPlayer 的自有程序代码不在本仓库公开。第三方组件由各自项目维护，其许可证与 PomiPlayer 的权利说明分别适用。

## 首个公开版本的准备状态

0.1.0 安装包目前只作为维护者的 Release 草稿保存，**尚未对公众提供下载**。现有验证包保留了许可证、Qt SBOM 和来源索引，但来源链接清单本身不等于完整的对应源码材料。公开二进制前，需按实际包内文件核对相符源码、构建资料及必要通知。

| 组件 | 当前验证版本与用途 | 上游 |
| --- | --- | --- |
| Qt | 6.10.0，界面和网络，以动态库使用 | [Qt LGPL 义务](https://www.qt.io/licensing/open-source-lgpl-obligations)、[版本源码](https://download.qt.io/archive/qt/6.10/6.10.0/submodules/) |
| libmpv | 0.42.0，官方 Windows x64 LGPL 构建，播放与解码 | [发行版及构建说明](https://github.com/mpv-player/mpv/releases/tag/v0.42.0)、[对应构建脚本](https://github.com/mpv-player/mpv/blob/v0.42.0/ci/build-mingw64.sh) |
| FFmpeg | 8.1.2 Gyan full build，独立的取帧与音轨提取程序，所用 full build 启用 GPL 组件 | [构建来源](https://www.gyan.dev/ffmpeg/builds/)、[许可说明](https://ffmpeg.org/legal.html) |
| whisper.cpp | v1.9.5 CPU 语音转写，MIT | [项目与版本源码](https://github.com/ggml-org/whisper.cpp/tree/v1.9.5) |
| Microsoft Visual C++ runtime | 应用本地运行库 | [再分发说明](https://learn.microsoft.com/en-us/visualstudio/releases/2022/redistribution) |
| NSIS | 安装器生成工具 | [项目及许可](https://nsis.sourceforge.io/License) |

上述列表是面向用户的摘要，不替代实际分发所附的完整第三方通知及依赖清单。标准包不附带语言、视觉或语音模型权重；可选本地 AI 组件及其依赖另行处理，不在当前公开仓库中提供。

## 源码与权利边界

在满足全部适用 LGPL 条件时，使用 LGPL Qt 可以保留应用源码不公开；这不免除第三方源码、通知、调试及动态库替换等相应要求。不得以保护 PomiPlayer 自有代码为由限制第三方许可证允许的权利。

当前核对还包括 libmpv 的链接依赖和独立 FFmpeg full build。普通上游首页、缺少版本对应的链接或自有程序“闭源”说明，不能替代需要提供的材料。

PomiPlayer does not publish its proprietary source in this repository. Third-party components retain their own licenses. The 0.1.0 installer is currently held in a maintainer-only draft release, not offered as a public download. Matching source and build materials must be checked against the actual bundled components before public binary distribution. Existing source references are not presented as a complete corresponding-source bundle.
