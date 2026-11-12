# 素材来源与替换说明

最后更新：2026-11-12。此项目是基于东方 Project 的个人练习同人作品，与官方无关联。

## 角色立绘（本地临时素材）

| 项目路径 | 角色与原作 | 作者 / 权利人 | 原图尺寸 | 来源页面 |
| --- | --- | --- | --- | --- |
| `assets/characters/reimu.png` | 博丽灵梦，《东方永夜抄 ～ Imperishable Night.》 | ZUN / 上海爱丽丝幻乐团 | 256 × 512，透明 PNG | [THBWiki：博丽灵梦（永夜抄立绘）](https://thwiki.cc/index.php?curid=2623) |
| `assets/characters/marisa.png` | 雾雨魔理沙，《东方永夜抄 ～ Imperishable Night.》 | ZUN / 上海爱丽丝幻乐团 | 256 × 512，透明 PNG | [THBWiki：雾雨魔理沙（永夜抄立绘）](https://thwiki.cc/index.php?curid=9347) |
| `assets/characters/flandre.png` | 芙兰朵露，全身与武器 | 用户提供图片，原作者未核实；角色原作上海爱丽丝幻乐团 | 1162 × 1353，透明 RGBA PNG | 本会话附件，经内置图像编辑去背景 |

以下为 H008 历史来源；芙兰已由 H020 全身图替换，旧文件备份保存在 builds/h020/assets/flandre-previous.png。原三张文件在 THBWiki 文件页均归类为「官方游戏立绘」「ZUN绘」；灵梦、魔理沙来自「东方永夜抄」，芙兰朵露来自「东方红魔乡」。下载后保留原始像素内容，仅在本项目中改名。没有使用同人图冒充官方图，也没有下载游戏安装包。

下载地址：

- [灵梦原图](https://upload.thbwiki.cc/1/18/%E5%8D%9A%E4%B8%BD%E7%81%B5%E6%A2%A6%EF%BC%88%E6%B0%B8%E5%A4%9C%E6%8A%84%E7%AB%8B%E7%BB%98%EF%BC%89.png)
- [魔理沙原图](https://upload.thbwiki.cc/b/bc/%E9%9B%BE%E9%9B%A8%E9%AD%94%E7%90%86%E6%B2%99%EF%BC%88%E6%B0%B8%E5%A4%9C%E6%8A%84%E7%AB%8B%E7%BB%98%EF%BC%89.png)
- [芙兰朵露原图](https://upload.thbwiki.cc/4/4d/%E8%8A%99%E5%85%B0%E6%9C%B5%E9%9C%B2%C2%B7%E6%96%AF%E5%8D%A1%E8%95%BE%E7%89%B9%EF%BC%88%E7%BA%A2%E9%AD%94%E4%B9%A1%E7%AB%8B%E7%BB%98%EF%BC%89.png)

芙兰朵露立绘下载于 2026-11-08，86,015 字节；SHA-256：`652df9efb93bc6201fb8232b1ad5bf5f38543c62f98c3300c0e38da664970b48`。已核对 PNG 编码、尺寸、透明通道并静态查看原图；未进行 Godot 导入或真实游戏画面检查。

这些立绘不是 CC0 或开源素材，网站可下载不代表获得公开分发许可。目前按个人练习需求作为本地临时素材保留。将来公开 GitHub 仓库、发布游戏包或分发项目之前，应替换为自绘或明确获授权的立绘，或移除这些文件。[东方 Project 官方二次创作指引](https://touhou-project.news/guidelines_en/) 列出不得在二创内容中使用从官方游戏提取的素材；仅注明非商业用途不能替代素材授权。

## 卡面（CC0）

- 本地目录：`assets/cards/`，55 张独立牌面，包含 1 张空白牌。
- 下载仓库：[celsiusnarhwal/uno](https://github.com/celsiusnarhwal/uno)。仓库说明牌面由 **lolkabash#7000** 从整套矢量图切分。
- 原始图稿：[Wikimedia Commons / UNO cards deck.svg](https://commons.wikimedia.org/wiki/File:UNO_cards_deck.svg)。作者 **Дмитрий Фомин（Dmitry Fomin）**，2013-11-10；原作页面明确标记 **CC0 1.0 Universal**。
- 完整许可随项目保存在 `assets/cards/LICENSE.md`；下载仓库说明保存在 `assets/cards/SOURCE_README.md`。
- 牌面原图约为 240 × 360 像素，部分切片宽或高多 1 像素，显示时应等比缩放。
- UNO 名称、商标与相关商业外观权益归 Mattel；CC0 仅适用于此处作者发布的图稿，不授予商标权，也不表示本项目获 Mattel 授权。

### 卡面文件映射

| 类别 | 文件名规则 | 示例 |
| --- | --- | --- |
| 颜色 | 红 `R`、黄 `Y`、绿 `G`、蓝 `B` | 蓝色前缀为 `B` |
| 数字牌 | 颜色前缀 + `0`～`9` + `.png` | `R7.png` = 红色 7 |
| 反转牌 | 颜色前缀 + `R.png` | `BR.png` = 蓝色反转 |
| 跳过牌 | 颜色前缀 + `S.png` | `YS.png` = 黄色跳过 |
| 加二牌 | 颜色前缀 + `A2.png` | `GA2.png` = 绿色 +2 |
| 万能换色 | `WC.png` | 无固定颜色 |
| 万能加四 | `W4.png` | 无固定颜色 |
| 空白 | `BLANK.png` | 不加入当前牌组 |

下载仓库中的 55 个 `.png` 文件有 53 个实际采用 GIF89a 编码，另外 2 个原本为 PNG。为兼容 Godot 的 PNG 导入器，本项目按原路径将所有卡面统一重新编码为真实 PNG，保留原图尺寸和画面，不作裁切、缩放或美术改动。所有输出均已检查 PNG 文件签名 `89 50 4E 47 0D 0A 1A 0A` 并重新解码验证尺寸。

## 字体（SIL OFL 1.1）

- 游戏完整字体：`assets/fonts/NotoSansSC.ttf`，真实字体名称 **Noto Sans SC**，简体中文黑体（无衬线）；原始文件名 `NotoSansSC[wght].ttf`，只改文件名，未修改字形。
- 来源：[Google Fonts 官方仓库 / ofl/notosanssc](https://github.com/google/fonts/tree/main/ofl/notosanssc)。
- [完整字体下载地址](https://raw.githubusercontent.com/google/fonts/main/ofl/notosanssc/NotoSansSC%5Bwght%5D.ttf)。下载日期 2026-11-08，文件大小 17,772,300 字节。
- `assets/fonts/ui_font.tres` 将游戏默认字重设为 400；所有普通控件及自绘界面文字使用同一内置黑体，不依赖用户设备安装字体。3D 加牌数字使用同源的 `assets/fonts/effect_numerals.ttf`：仅含 `+0123456789`，静态字重 800，合并重叠轮廓，衍生字体名 Touhou UNO Numerals ExtraBold。Windows/Web 使用完全相同的黑体字形与立体厚度，不依赖系统字体。该 4,260 字节子集由 fontTools 4.68.0 / skia-pathops 0.9.2 从上述 NotoSansSC.ttf 生成，沿用同一 OFL 许可；可用 `tools/build_effect_font.py` 及其注明的构建依赖重新生成。
- 浏览器加载页：`web/static/NotoSansSC-UI.woff2`，由 [Google Fonts 官方 CSS API](https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@400;500&display=swap) 按加载页文本与 ASCII 字符生成的 WOFF2 子集，文件大小 42,844 字节；随网页本地分发，运行时不请求外部字体服务。若新增加载页文案，应同步重新生成此子集。
- 许可：**SIL Open Font License 1.1**，完整原文及版权声明保存在 `assets/fonts/OFL.txt`。完整字体及网页子集分发时均保留该文件。

## 背景音乐与操作音效

- 背景音乐：**リーインカーネーション / Reincarnation（东方梦时空，魅魔主题）**，作曲及官网编曲录音：**ZUN / 上海爱丽丝幻乐团**。
- 来源：[上海爱丽丝幻乐团官方网站「东方幻想的音乐」旧曲页面](https://www16.big.or.jp/~zun/html/music_old.html)，页面 MP3 栏中的「リーインカーネーション」，公开日期 2001-10-30。
- [官网直接下载地址](https://www16.big.or.jp/~zun/data/mp3/th3_05.mp3)。下载后仅改文件名为 `assets/audio/bgm.mp3`，没有改编、裁切、变速或重新编码。
- 已验证：MP3、44,100 Hz、双声道、时长约 **4 分 20 秒**，文件大小 4,161,330 字节。SHA-256：`507ca5c5096ecc8b00b977237a16555a1c443b90615a1ba414108d6c637cf9cf`。
- 这是作者官网公开供下载聆听的录音，不是 CC0 或开源音乐；官网保留 ZUN 的著作权。本项目作为个人练习的本地 BGM 使用，没有声称获得公开再分发许可。未来公开 GitHub 仓库或发布游戏包前，须另行确认使用许可，或移除、替换此录音。
- `scripts/audio_manager.gd` 自动循环播放这首音乐，默认音量 -20 dB；音乐开关和音量保存在 Godot 的 `user://audio_settings.cfg`。
- 出牌、摸牌、UNO、技能、胜负及回合提示音由 `audio_manager.gd` 程序生成短音符，不截取或改编上述 BGM，不依赖其他声音素材。

## 角色技能语音（本地临时素材）

三段真人角色配音来自 **《东方弹幕神乐 / 東方ダンマクカグラ》官网存档角色页的 VOICE 3 公开试听**。这是东方 Project 衍生游戏的角色配音，并非 ZUN 原作游戏配音，也不是 AI 模仿声线。官网版权标示为 ©上海アリス幻樂団 / ©アンノウンX。

| 项目路径 | 角色 / 声优 | 官方试听来源 | 最终音频 |
| --- | --- | --- | --- |
| `assets/audio/voices/reimu_skill.wav` | 博丽灵梦 / 湯浅かえで（Kaede Yuasa） | [官网角色页：博麗霊夢，VOICE 3](https://danmaku.jp/archive/character/c001/)；[原始试听 M4A](https://danmaku.jp/import/character/c001_voice3.m4a) | 2.065 秒，44,100 Hz，单声道 PCM16 WAV，182,222 字节 |
| `assets/audio/voices/marisa_skill.wav` | 雾雨魔理沙 / 本多真梨子（Mariko Honda） | [官网角色页：霧雨魔理沙，VOICE 3](https://danmaku.jp/archive/character/c002/)；[原始试听 M4A](https://danmaku.jp/import/character/c002_voice3.m4a) | 4.062 秒，44,100 Hz，单声道 PCM16 WAV，358,350 字节 |
| `assets/audio/voices/flandre_skill.wav` | 芙兰朵露·斯卡蕾特 / 花守ゆみり（Yumiri Hanamori） | [官网角色页：フランドール・スカーレット，VOICE 3](https://danmaku.jp/archive/character/c013/)；[原始试听 M4A](https://danmaku.jp/import/character/c013_voice3.m4a) | 5.734 秒，44,100 Hz，单声道 PCM16 WAV，505,806 字节 |

原始公开试听为 M4A。为兼容 Godot，将完整试听解码为 WAV，未裁切台词、变调、变速或拼接；解码时移除了原编码格式的填充时间。三条最终 WAV 均通过完整音频解码验证。

芙兰朵露语音下载于 2026-11-08。官网角色页标示声优「花守ゆみり」与 VOICE 3；页面脚本的试听地址规则为 `/import/character/<角色编号>_voice3.m4a`，该角色编号为 `c013`。原始 M4A 为 44,380 字节，SHA-256：`eddba66409e73859d1b78aeee957c6d6312d3797f2abe0471f0c8097f8650d02`；完整解码后的 WAV SHA-256：`11b2a1fe002a207b8cca1775a5614254cf562ac16c3b80d49b934c474e0e6bcf`。本轮仅检查媒体格式与完整解码，未进行听感、Godot 导入或游戏播放测试；不添加未经确认的台词字幕。原始 M4A 暂存于收集工作目录的 `builds/h008-source/`，不随游戏打包。

官网没有附逐字台词，游戏演出不显示未经人工确认的字幕。使用电脑已有离线转写模型得到的参考识别结果如下（仅用于辨认素材，不视为官方文字稿）：灵梦「さっさと次に行きましょ」；魔理沙「ほらー、さっさと来ないと置いてくぞー！」。两段均为推动行动的短句，不声称是「博丽结界」或「魔力重构」的官方技能台词。

官网允许访问试听不等于允许在其他作品中公开再分发，这些录音不是 CC0 或开源素材。本项目仅按个人练习需求作为本地临时配音保留，并在 `.gitignore` 中排除。公开仓库或发布游戏包前，应移除、换为自行录制或明确获授权的录音。临时下载文件与转写依赖存放在工程外的 `work/voice-source-v3/`，不随项目打包。

`audio_manager.gd` 使用独立语音播放器，默认增益 0.85；语音播放时将 BGM 临时降低 11 dB，结束或跳过演出后恢复用户设置的音乐音量。语音开关保存在原有 `user://audio_settings.cfg` 的 `[voice] enabled` 字段；缺失语音文件时安静跳过，不阻断技能演出。

## 后续替换

角色图保持透明 PNG，并沿用 `reimu.png`、`marisa.png`、`flandre.png` 文件名即可替换。卡面可沿用上述文件名。背景音乐可替换 `assets/audio/bgm.mp3`，技能语音可替换 `assets/audio/voices/reimu_skill.wav`、`marisa_skill.wav`、`flandre_skill.wav`。公开仓库前请先处理角色立绘、背景音乐与角色语音录音；代码、CC0 卡面与 OFL 字体可以分别保留各自许可和来源说明。

## 3D 牌桌与卡背

`scripts/table_3d.gd` 中的牌桌、纸张厚度、牌堆、桌布纹理与方向箭头由代码创建，使用项目已有卡面。`assets/card_back.svg` 为本项目绘制的阴阳玉矢量卡背；未使用参考截图中的商业背景、头像或卡背素材。

## 新增幽幽子（H011，2026-11-09）

收集日期：2026-11-09（Asia/Shanghai）。来源文件已按下述路径接入当前主目录，沿用已有本地临时素材管理方式。

### 角色立绘

| 项目路径 | 角色与原作 | 作者 / 权利人 | 原图尺寸 | 来源页面 |
| --- | --- | --- | --- | --- |
| `assets/characters/yuyuko.png` | 西行寺幽幽子，《东方永夜抄 ～ Imperishable Night.》 | ZUN / 上海爱丽丝幻乐团 | 256 × 512，透明 RGBA PNG | [THBWiki：西行寺幽幽子（永夜抄立绘）](https://thwiki.cc/index.php?curid=2506) |

[原始 PNG 下载地址](https://upload.thbwiki.cc/3/3d/%E8%A5%BF%E8%A1%8C%E5%AF%BA%E5%B9%BD%E5%B9%BD%E5%AD%90%EF%BC%88%E6%B0%B8%E5%A4%9C%E6%8A%84%E7%AB%8B%E7%BB%98%EF%BC%89.png)。文件页归类为「官方游戏立绘」「ZUN绘」「东方永夜抄」，文件页编号为 2506。通过来源页读取原图地址后下载，保存为 `yuyuko.png`，只改文件名，没有裁切、缩放、重新编码或绘制；没有下载游戏安装包。

文件大小为 165,011 字节；SHA-256：`93c9a8a80622e3a196df9f014bbb18d53e64f06a4419f4a8128cc6cb45f906f9`。已核对 PNG 编码、256 × 512 尺寸、RGBA 像素格式，并静态查看原图；已按本轮用户选择增量导入 Godot，并由无界面加载专项确认 Texture2D 尺寸；实际游戏画面未验证。

沿用原项目约定：这是个人练习用的本地临时官方立绘，不是 CC0 或开源素材，能下载不代表获得公开分发许可。公开仓库或发布前的移除、替换及授权处理遵循现有素材说明，文件与导入元数据沿用 `.gitignore` 中 `assets/characters/*.png` 和 `*.png.import` 的排除。

### 技能语音

| 项目路径 | 角色 / 声优 | 官方试听来源 | 最终音频 |
| --- | --- | --- | --- |
| `assets/audio/voices/yuyuko_skill.wav` | 西行寺幽幽子 / 柏山奈々美（Nanami Kashiyama） | [弹幕神乐官网存档角色页：西行寺 幽々子，VOICE 3](https://danmaku.jp/archive/character/c047/)；[原始试听 M4A](https://danmaku.jp/import/character/c047_voice3.m4a) | 7.522 秒，44,100 Hz，单声道 PCM16 WAV，663,502 字节 |

官网角色页明确标示声优「柏山奈々美」并提供 VOICE 1／2／3；该角色编号为 `c047`。已核对官网页面脚本：此角色没有自定义语音数组，VOICE 3 按 `/import/character/<角色编号>_voice3.m4a` 加载，因此本次使用 `c047_voice3.m4a`。这是《东方弹幕神乐》的真人配音公开试听，不是 ZUN 原作游戏配音或 AI 声音；版权标示为 ©上海アリス幻樂団 / ©アンノウンX。

原始 M4A：AAC、44,100 Hz、单声道，编码流时长 7.569705 秒，60,934 字节；SHA-256：`cd73fd580b73ee32522733e38e759d2f9da315a6ee10f59417cf46d49a0c5eb8`。

转换后的 WAV：PCM signed 16-bit little-endian、44,100 Hz、单声道，实际时长 7.521814 秒，663,502 字节；SHA-256：`7cd1f99098e7224bf542d158e654735e7a6303c40843679ac3ad586c92d331bb`。

完整解码为 WAV 以兼容 Godot，没有截断、变速、变调、混音或拼接；前后时长差来自 AAC 编码填充的移除。未添加未经确认的台词字幕。转换工具为本机 FFmpeg `2025-02-24-git-6232f416b1-full_build-www.gyan.dev`，命令为：

```text
ffmpeg -v error -nostdin -i source/c047_voice3.m4a -map 0:a:0 -c:a pcm_s16le yuyuko_skill.wav
```

已用 FFprobe 核对格式，并执行完整解码检查 `ffmpeg -v error -nostdin -i yuyuko_skill.wav -f null NUL`，退出码为 0，无解码错误。已增量导入 Godot，加载专项确认完整 7.521814 秒 AudioStreamWAV 及演出时长；未进行听感或真实游戏播放测试。

收尾时另对 `yuyuko.png`、原始 `source/c047_voice3.m4a` 与 `yuyuko_skill.wav` 分别进行完整媒体解码，三次均退出 0；重新计算三份文件哈希，与 `yuyuko-assets.json` 一致。

沿用原项目约定：录音仅作为个人练习的本地临时配音，不是 CC0 或开源素材；官网可试听不等于公开再分发许可。继续由 `assets/audio/voices/*.wav` 和 `*.wav.import` 忽略，公开分发前按现有来源说明移除、替换或确认授权。

### 素材文件与来源证据

- 可接入文件：`yuyuko.png`、`yuyuko_skill.wav`。
- 原始语音：`source/c047_voice3.m4a`，不随游戏打包。
- 来源证据：`source/thbwiki-file-page.html`、`source/danmaku-character-page.html`、`source/danmaku-character-page-script.js`。THBWiki 文件页在搜索工具未命中缓存，实际 HTTPS 读取成功；上述页面保存了分类、原图地址和角色编号。
- 结构化记录：`yuyuko-assets.json`，包含来源、元数据、哈希、转换命令及未验证范围。


来源证据与元数据已归档到主目录忽略的 `builds/h011/assets/`；不随游戏打包。

## H020：蕾米莉亚与芙兰全身图（2026-11-12）

- 蕾米莉亚立绘：`assets/characters/remilia.png`，ZUN / 上海爱丽丝幻乐团《东方永夜抄》，256 × 512 RGBA PNG。[THBWiki 文件页](https://thwiki.cc/文件:蕾米莉亚·斯卡蕾特（永夜抄立绘）.png)；[原图](https://upload.thbwiki.cc/e/e0/%E8%95%BE%E7%B1%B3%E8%8E%89%E4%BA%9A%C2%B7%E6%96%AF%E5%8D%A1%E8%95%BE%E7%89%B9%EF%BC%88%E6%B0%B8%E5%A4%9C%E6%8A%84%E7%AB%8B%E7%BB%98%EF%BC%89.png)。原字节不变，仅改名；SHA-256 `f4b0377edd053402fe26d964598a1f9c110f9b4dda3d440915ccc5423b95e21b`。
- 芙兰全身立绘：`assets/characters/flandre.png`，采用[东方弹幕神乐官方角色页](https://danmaku.jp/archive/character/c013/)的 [c013_boss.png](https://danmaku.jp/import/character/c013_boss.png)，作者栗栖 歳；675 × 467 RGBA PNG，完整身体、双腿与翅膀。原字节不变；SHA-256 `17cd873d644c05ff53849c3a9ba77916155e755ade8b8504660b48d7756f61b8`。未采用先核对的刚欲异闻半身图。
- 蕾米莉亚语音：`assets/audio/voices/remilia_skill.wav`，声优山岡ゆり，来自[官方角色页 VOICE 3](https://danmaku.jp/archive/character/c007/)及[原始试听](https://danmaku.jp/import/character/c007_voice3.m4a)。完整转换为 44,100 Hz 单声道 PCM16 WAV，时长 5.594558 秒，未裁切或变速；SHA-256 `9010c2f16e18decac532588231b6762c157f5b1724431c3281e8d89870b7c891`。版权 ©上海アリス幻樂団 / ©アンノウンX。

来源页面、播放器脚本、原始语音、元数据和旧图备份在 `builds/h020/assets/`。这些本地练习素材沿用已有忽略规则，不纳入 Git；静态解码与图片查看、用户选择的 Godot 导入及无界面资源加载检查已通过；真实画面和听感未验证。

## H023：用户提供的芙兰全身持武器图

- 用户于 2026-11-12 提供 440 × 512 RGB 黑底图，要求换立绘、去背景并保留完整主体和武器。本轮未将其归为官方素材，原作者未核实。
- 使用内置图像编辑工具进行透明抠图，最终接入 assets/characters/flandre.png（1162 × 1353 RGBA）；并非声称原始像素逐点不变。检查帽子、双翼晶体、双脚、左侧弧形武器和腿间钩尾均保留；全身显示沿用 KEEP_ASPECT_CENTERED，头像另取头部区域。
- 最终 SHA-256：ed9761f259df8a9442037f8d5c3a228e59ace9bde848a97419032ab290d1dfe0。源图及旧立绘备份、透明通道信息在 builds/h023/assets；H020 图作为历史记录保留，不再代表当前芙兰立绘。
- 编辑提示：只提取原图角色、去除纯黑背景为透明；保留原造型和颜色，不裁切帽子、头发、所有翼晶体、两只鞋及整根黑色武器，清理背景边缘，保留透明边距。最终英文提示全文位于 builds/h023/assets/edit-prompt.txt。
- 原生导入及无界面资源加载检查通过；没有打开实际游戏、截图或检验实际屏幕效果。语音未改。
