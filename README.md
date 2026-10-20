# ctdlb 的 Dalamud 插件仓库

个人维护的卫月（Dalamud）第三方插件源，主要放自己汉化/重构的插件。

## 添加方式

在游戏里输入 `/xlplugins` → 设置 → 自定义插件仓库 → 添加，粘贴：

```
https://raw.githubusercontent.com/ctdlb/DalamudPlugins/main/pluginmaster.json
```

如果直连 GitHub 打不开，用系统代理或加速器，不要用 jsDelivr 镜像——它的分支缓存最长 12 小时，新版本会迟迟不出现。

保存后回到「全部插件」，搜索插件名即可安装/更新。

## 插件列表

| 插件 | 说明 | 源码 |
| --- | --- | --- |
| TextToTalkCN | 聊天与剧情对话朗读（TTS）简体中文汉化版，适配国服 XIVLauncherCN | [ctdlb/TextToTalkCN](https://github.com/ctdlb/TextToTalkCN) |
| Price Insight CN | 悬停物品显示市场价格（Universalis，缓存 90 分钟） | [ctdlb/PriceInsight-CN](https://github.com/ctdlb/PriceInsight-CN) |

## 说明

- `pluginmaster.json` 是 Dalamud 的插件仓库清单格式，数组里每一项对应一个插件。
- 新增插件时，在数组里追加一条 `PluginMasterEntry`，把 `DownloadLinkInstall` / `DownloadLinkUpdate` 指向该插件 Release 里的 zip 即可。
- 本仓库只存放清单，插件本体放在各自的代码仓库里发布。