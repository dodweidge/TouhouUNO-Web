# 素材来源与替换说明

记录日期：2026-10-24。此项目是基于东方 Project 的个人练习同人作品，与官方无关联。

## 角色立绘（本地临时素材）

| 项目路径 | 角色与原作 | 作者 / 权利人 | 原图尺寸 | 来源页面 |
| --- | --- | --- | --- | --- |
| `assets/characters/reimu.png` | 博丽灵梦，《东方永夜抄 ～ Imperishable Night.》 | ZUN / 上海爱丽丝幻乐团 | 256 × 512，透明 PNG | [THBWiki：博丽灵梦（永夜抄立绘）](https://thwiki.cc/index.php?curid=2623) |
| `assets/characters/marisa.png` | 雾雨魔理沙，《东方永夜抄 ～ Imperishable Night.》 | ZUN / 上海爱丽丝幻乐团 | 256 × 512，透明 PNG | [THBWiki：雾雨魔理沙（永夜抄立绘）](https://thwiki.cc/index.php?curid=9347) |

两张文件在 THBWiki 文件页均归类为「官方游戏立绘」「ZUN绘」「东方永夜抄」。下载后保留原始像素内容，仅在本项目中改名。没有使用同人图冒充官方图，也没有下载游戏安装包。

下载地址：

- [灵梦原图](https://upload.thbwiki.cc/1/18/%E5%8D%9A%E4%B8%BD%E7%81%B5%E6%A2%A6%EF%BC%88%E6%B0%B8%E5%A4%9C%E6%8A%84%E7%AB%8B%E7%BB%98%EF%BC%89.png)
- [魔理沙原图](https://upload.thbwiki.cc/b/bc/%E9%9B%BE%E9%9B%A8%E9%AD%94%E7%90%86%E6%B2%99%EF%BC%88%E6%B0%B8%E5%A4%9C%E6%8A%84%E7%AB%8B%E7%BB%98%EF%BC%89.png)

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

两段真人角色配音来自 **《东方弹幕神乐 / 東方ダンマクカグラ》官网存档角色页的 VOICE 3 公开试听**。这是东方 Project 衍生游戏的角色配音，并非 ZUN 原作游戏配音，也不是 AI 模仿声线。官网版权标示为 ©上海アリス幻樂団 / ©アンノウンX。

| 项目路径 | 角色 / 声优 | 官方试听来源 | 最终音频 |
| --- | --- | --- | --- |
| `assets/audio/voices/reimu_skill.wav` | 博丽灵梦 / 湯浅かえで（Kaede Yuasa） | [官网角色页：博麗霊夢，VOICE 3](https://danmaku.jp/archive/character/c001/)；[原始试听 M4A](https://danmaku.jp/import/character/c001_voice3.m4a) | 2.065 秒，44,100 Hz，单声道 PCM16 WAV，182,222 字节 |
| `assets/audio/voices/marisa_skill.wav` | 雾雨魔理沙 / 本多真梨子（Mariko Honda） | [官网角色页：霧雨魔理沙，VOICE 3](https://danmaku.jp/archive/character/c002/)；[原始试听 M4A](https://danmaku.jp/import/character/c002_voice3.m4a) | 4.062 秒，44,100 Hz，单声道 PCM16 WAV，358,350 字节 |

原始公开试听为 M4A。为兼容 Godot，将完整试听解码为 WAV，未裁切台词、变调、变速或拼接；解码时移除了原编码格式的填充时间。两条最终 WAV 均通过完整音频解码验证。

官网没有附逐字台词，游戏演出不显示未经人工确认的字幕。使用电脑已有离线转写模型得到的参考识别结果如下（仅用于辨认素材，不视为官方文字稿）：灵梦「さっさと次に行きましょ」；魔理沙「ほらー、さっさと来ないと置いてくぞー！」。两段均为推动行动的短句，不声称是「博丽结界」或「魔力重构」的官方技能台词。

官网允许访问试听不等于允许在其他作品中公开再分发，这些录音不是 CC0 或开源素材。本项目仅按个人练习需求作为本地临时配音保留，并在 `.gitignore` 中排除。公开仓库或发布游戏包前，应移除、换为自行录制或明确获授权的录音。临时下载文件与转写依赖存放在工程外的 `work/voice-source-v3/`，不随项目打包。

`audio_manager.gd` 使用独立语音播放器，默认增益 0.85；语音播放时将 BGM 临时降低 11 dB，结束或跳过演出后恢复用户设置的音乐音量。语音开关保存在原有 `user://audio_settings.cfg` 的 `[voice] enabled` 字段；缺失语音文件时安静跳过，不阻断技能演出。

## 后续替换

角色图保持透明 PNG，并沿用 `reimu.png`、`marisa.png` 文件名即可替换。卡面可沿用上述文件名。背景音乐可替换 `assets/audio/bgm.mp3`，技能语音可替换 `assets/audio/voices/reimu_skill.wav`、`marisa_skill.wav`。公开仓库前请先处理角色立绘、背景音乐与角色语音录音；代码、CC0 卡面与 OFL 字体可以分别保留各自许可和来源说明。

## 3D 牌桌与卡背

`scripts/table_3d.gd` 中的牌桌、纸张厚度、牌堆、桌布纹理与方向箭头由代码创建，使用项目已有卡面。`assets/card_back.svg` 为本项目绘制的阴阳玉矢量卡背；未使用参考截图中的商业背景、头像或卡背素材。
