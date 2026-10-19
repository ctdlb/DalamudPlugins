# ctdlb 的 Dalamud 插件仓库

个人维护的卫月（Dalamud）第三方插件源，主要放自己汉化/重构的插件。

## 添加方式

在游戏里输入 `/xlplugins` → 设置 → 自定义插件仓库 → 添加，粘贴：

```
https://raw.githubusercontent.com/ctdlb/DalamudPlugins/main/pluginmaster.json
```

如果直连 GitHub 打不开，可以换成 CDN 地址（同一个文件）：

```
https://cdn.jsdelivr.net/gh/ctdlb/DalamudPlugins@main/pluginmaster.json
```

保存后回到「全部插件」，搜索插件名即可安装/更新。

## 插件列表

| 插件 | 说明 | 源码 |
| --- | --- | --- |
| TextToTalkCN | 聊天与剧情对话朗读（TTS）简体中文汉化版，适配国服 XIVLauncherCN | [ctdlb/TextToTalkCN](https://github.com/ctdlb/TextToTalkCN) |

## 说明

- `pluginmaster.json` 是 Dalamud 的插件仓库清单格式，数组里每一项对应一个插件。
- 新增插件时，在数组里追加一条 `PluginMasterEntry`，把 `DownloadLinkInstall` / `DownloadLinkUpdate` 指向该插件 Release 里的 zip 即可。
- 本仓库只存放清单，插件本体放在各自的代码仓库里发布。
