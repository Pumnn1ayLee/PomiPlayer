# User guide

Download the [0.1.0 Preview installer](https://github.com/Pumnn1ayLee/PomiPlayer/releases/tag/v0.1.0-preview). The preview is still being improved; check its release notes for installation details and known issues.

## Playback

Choose a writable installation folder. Settings, playback history, caches and models stay in the player folder. Ordinary playback needs no AI model, account or administrator access.

Open a local video with the toolbar, `Ctrl+O`, or drag and drop. Press Play or Space after the video ends to replay it. The context menu offers playback speed, frame stepping, looping, aspect ratio, audio and subtitle controls.

## Video assistant

Open the sidebar with its toolbar button or `Ctrl+L`. The sliders icon opens performance settings. The back arrow returns to the assistant home while preserving the conversation; the trash button clears it.

| Task | Requirement |
| --- | --- |
| Timestamp navigation and playback commands | No model needed. |
| Search a subtitle phrase | Load subtitles first. |
| Discuss dialogue or content | Configure a model service or compatible local model. |
| Ask about a frame or request an overview | Image-capable model; cloud frame sharing needs separate permission. |
| Generate SRT or VTT | Compatible Whisper GGML speech model. |

Follow-up questions and unrelated topics share one input box. Processing stages, elapsed time and short evidence summaries are shown; these are not the model's private internal reasoning. Overview timestamps let you choose a scene to visit.

## Cloud configuration

In Settings → Content model, enter a service URL, model name and API key. The service must support Chat Completions; visual questions also require image input support.

You choose the provider and pay any provider charges. PomiPlayer supplies no shared account, quota or built-in key. Saving a service does not prove connectivity or authorize frame sharing. Windows DPAPI protects credentials; they may not decrypt under another Windows account.

Questions send relevant conversation context. Video questions may send relevant subtitles. Sampled frames are sent only with separate permission. Review your provider's data handling policy before use.

## Local models and performance

The standard installer contains no language-model weights or GPU inference components. Local inference requires a compatible runtime and model. Vision models may need a matching projector. See release notes for component availability and hardware support.

Performance settings control context, GPU layers, batching, image budget, response length and idle release. Start with the resource-saving preset. A shorter context does not reduce model weights; moving work to the CPU can increase system RAM use.

Opening the assistant alone does not load a language model. Disabling a local model does not automatically switch to the cloud. Capabilities and resource use vary by model.

## Subtitles

Ask to generate subtitles, choose SRT or VTT, then choose the video folder or a custom destination. Default filenames are `video-name.pomiplayer.srt` or `video-name.pomiplayer.vtt`.

Select a compatible speech model before starting. Completed subtitles load automatically and become available to the assistant. Existing destination files are not silently overwritten. Errors or cancellation preserve the original subtitles. Test a short clip first to assess speed and quality.

## Default shortcuts

| Shortcut | Action |
| --- | --- |
| `Space` | Play, pause or replay |
| `Left` / `Right` | Seek backward or forward 5 seconds |
| `Up` / `Down` | Adjust volume |
| `M` | Toggle mute |
| `F11` | Toggle fullscreen |
| `Ctrl+O` | Open video |
| `Ctrl+L` | Open assistant |
| `Ctrl+,` | Settings |
| `Ctrl+S` | Save current frame |

Shortcuts are customizable. In the message box, Enter sends and Shift+Enter adds a new line. Confirming an IME candidate does not submit the message.

Change the interface language from the toolbar or Settings without restarting. New answers follow that language unless you explicitly request another one. Existing conversations and media quotations are not translated again.

The sun or moon button changes theme; the gear opens Settings. Uninstallation removes installed program files while preserving personal settings, caches and models. Back up your data before manually removing it.
