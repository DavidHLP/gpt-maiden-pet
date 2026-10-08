# GPT娘 · GPT Maiden Pet

A white-and-lilac dragon-maiden animated pet, with **nine standard actions and sixteen look directions**.

白紫色龙娘主题动态宠物。此版本修复待机与鼠标注视切换时的头身比例差异；保留九种标准动作。

![Idle and look-direction transitions](previews/idle-look-switch.gif)

## Download / 下载

Use the [latest release](https://github.com/DavidHLP/gpt-maiden-pet/releases/latest), or download [GPT-maiden-pet-v2.zip](downloads/GPT-maiden-pet-v2.zip).

- [Sprite atlas](assets/spritesheet-extended.png)
- [MP4 preview](previews/idle-look-switch.mp4)
- [Editable Blender project](downloads/GPT-maiden-Blender-project.zip)

## Install / 使用

The ZIP contains `gpt-maiden-refined/pet.json` and `spritesheet.png`. It targets the v2 sprite-sheet format. Follow the custom-pet import workflow supported by your client; this repository does not install or activate a pet automatically.

For an existing compatible pet package, back up your current files, replace its `spritesheet.png` with the supplied atlas, and preserve your existing pet ID and other configuration. Reload the pet if your client caches the old image. If your client has no compatible import function, the PNG and previews remain usable as standalone assets; no universal install command is claimed.

安装包包含配置与精灵图。已有兼容宠物包请先备份，只替换同名 `spritesheet.png`，保留原宠物 ID 和其余配置；若显示旧图，请重新加载。具体导入方式取决于客户端提供的功能。

## Format / 格式

| Property | Value |
|---|---|
| Atlas | 1536 × 2288 RGBA PNG |
| Grid | 8 × 11 |
| Cell | 192 × 208 |
| Populated frames | 73 |
| Standard actions | 9 |
| Look directions | 16 |

The pet uses the format's fixed frame layout. The preview video's frame rate is not a claim of additional unique animation frames. Some diagonal look angles are deliberately subtle.

The v2 update was produced on October 4, 2026. Package artwork checks are summarized in [QA-summary.txt](assets/QA-summary.txt). Publication preparation preserves the atlas SHA-256:

`c307ed4e9415fb8797238f8343a7a863a1cb974f9496e22d7425136505011a68`

## Editable source / 可编辑工程

Open `GPT-Maiden-animation.blend` in Blender 4.3.2 or a compatible newer version. It is an editable **2D sprite timeline**, not a rigged 3D character. The atlas is packed into the project and also included next to it. `timeline.json` documents timing. A 100 fps authoring timeline provides timing granularity; it does not create new painted frames.

Blender 工程是可编辑的二维逐帧时间轴；内嵌图集，并附独立图集文件。发布副本已清理原工作路径。

## Provenance and rights

The character direction/reference was supplied by the repository owner. Refined artwork and assembly were AI-assisted. This is a community-created character and asset pack, not an official OpenAI product, character, or endorsement.

No open-source or open-content license is granted by this repository at this time. Contact the owner before redistribution or commercial use. Dependencies and third-party trademarks retain their respective rights.
