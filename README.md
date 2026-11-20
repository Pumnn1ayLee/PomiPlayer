<p align="center">
  <img src="assets/pomiplayer.svg" width="72" height="72" alt="PomiPlayer">
</p>

<h1 align="center">PomiPlayer</h1>

<p align="center">Windows 视频播放器，带一个可以对话的视频助手。</p>

<p align="center">
  <a href="https://github.com/Pumnn1ayLee/PomiPlayer/releases/download/v0.1.0-preview/PomiPlayer-0.1.0-Setup-x64.exe">下载 Windows 版</a>　
  <a href="docs/USAGE.md">使用指南</a>　
  <a href="https://github.com/Pumnn1ayLee/PomiPlayer/issues/new/choose">反馈问题</a>　
  <a href="README.en.md">English</a>
</p>

## Assets

**0.1.0 Preview，Windows x64，约 121 MB。** 当前在 Windows 11 上测试。

[**PomiPlayer-0.1.0-Setup-x64.exe**](https://github.com/Pumnn1ayLee/PomiPlayer/releases/download/v0.1.0-preview/PomiPlayer-0.1.0-Setup-x64.exe)　
[更新说明](https://github.com/Pumnn1ayLee/PomiPlayer/releases/tag/v0.1.0-preview)

选择一个可写文件夹安装即可，不需要管理员权限。设置和缓存放在播放器目录里，卸载时保留。下载后直接运行安装程序；当前预览版尚未签名，Windows 可能显示发布者提醒。

![PomiPlayer 深色界面](docs/screenshots/pomiplayer-dolomites-dark.png)

PomiPlayer 的主要空间留给视频。右侧助手可以收起，播放时控制栏自动隐藏。支持深浅主题、字幕、音轨、倍速和快捷键，也可以直接用一句话查找片段。

## 看视频，也可以问视频

打开助手后，可以查台词、询问画面、概括内容，或直接聊其他话题。

```text
跳到 00:18
找到「信号」的片段
当前画面里有什么？
概括这个视频，按时间列出关键片段
```

视频概览会把内容按时间整理，每个片段都有时间按钮，点击就能跳过去。画面理解采用采样，可能漏掉短暂动作。

时间跳转和台词关键词检索不需要 AI。内容问答需要在设置中连接模型服务；使用本地模型时，需要自行准备运行库和模型。云端画面问答还需要模型支持图片，并单独允许发送采样画面。标准包不附带模型或 API 密钥。

## 字幕

在助手中输入“生成字幕”，选择 SRT 或 VTT，再选择保存位置。默认存到视频所在目录，生成后自动加载，也能继续用助手查找。转写需要另行准备兼容的 Whisper GGML 语音模型。

## 按习惯调整

右键可以调整倍速、画面比例、音轨和字幕，也能逐帧查看或保存截图。播放结束后，按空格或播放键即可从头重播。

设置里可以修改快捷键、字幕样式和助手参数。界面支持中文、英语、日语、韩语、法语、德语、西班牙语和巴西葡萄牙语，中文提供简体和繁体。切换语言无需重启，新回答会跟随所选语言。

![PomiPlayer 浅色界面](docs/screenshots/pomiplayer-dolomites-light.png)

完整操作见[使用指南](docs/USAGE.md)。截图中的山脉视频由 Zlatin Georgiev 拍摄，来自 Pexels，详见[素材署名](docs/MEDIA_CREDITS.md)。

## 问题反馈

这是早期预览版。遇到问题，请在 [Issues](https://github.com/Pumnn1ayLee/PomiPlayer/issues/new/choose) 留下版本、复现步骤和必要的环境信息。发送日志或截图前，请删掉密钥和私人内容。安全漏洞请通过[私密报告](https://github.com/Pumnn1ayLee/PomiPlayer/security/advisories/new)提交。

本仓库用于版本发布和反馈，播放器核心源码暂不公开。数据处理方式见[隐私政策](docs/PRIVACY.md)。第三方组件保留各自的许可证，见[第三方说明](docs/THIRD_PARTY.md)和[权利说明](NOTICE.md)。
