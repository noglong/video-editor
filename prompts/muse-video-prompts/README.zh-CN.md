# Muse Video 提示词：X 上收集的 205 条真实提示词

[English](README.md) · 简体中文 · [在 apimodels.app 上看带视频的版本](https://apimodels.app/zh/muse-video-prompts) · [在 GitHub Pages 上搜索、一键复制](https://apimodels.github.io/muse-video-prompts/)

这里收的是 68 位创作者在 Meta 的 Muse 里跑过、再在 2026-09-17 到 2026-11-04 之间发到 X 上的 205 条视频提示词，每条都逐字全文收录、注明作者，并附上原帖链接。

说明：这个合集由 [apimodels.app](https://apimodels.app) 整理，我在这个 API 平台工作。apimodels.app 是多模型 API 平台，也提供 [Muse Video 的 API](https://apimodels.app/zh/models/muse-video)。API 有哪些限制，写在下面「[用 API 跑这些提示词](#用-api-跑这些提示词)」里，因为有些提示词只能在 Muse 应用里用。带作者成片、可以直接播放的在线版在 [apimodels.app 的 Muse Video 提示词库](https://apimodels.app/zh/muse-video-prompts)。

提示词以中文为主，也有英文和日文。作者把提示词拆在主帖和自己的回复里发的，已经拼回一条；别的账号转发的同一条提示词，合并到一条里，记在「同一提示词也被发布于」。

## 目录

- [多镜头卡点（参考图模板）](#多镜头卡点参考图模板)（31）
- [男友 POV](#男友-pov)（39）
- [自拍 / Vlog](#自拍--vlog)（28）
- [舞蹈](#舞蹈)（14）
- [时尚人像](#时尚人像)（12）
- [转场 / 变装](#转场--变装)（5）
- [古风 / 历史](#古风--历史)（23）
- [奇幻 / 动画 CG](#奇幻--动画-cg)（14）
- [纪实 / 风光](#纪实--风光)（9）
- [ASMR](#asmr)（2）
- [电影感 / 剧情](#电影感--剧情)（5）
- [长视频 / 多段脚本](#长视频--多段脚本)（11）
- [一句话 / 对话式](#一句话--对话式)（12）
- [这些提示词是怎么写的](#这些提示词是怎么写的)
- [用 API 跑这些提示词](#用-api-跑这些提示词)
- [怎么收集的](#怎么收集的)
- [出处、版权与许可](#出处版权与许可)

每条提示词在 [prompts/](prompts) 下有单独一页，写明作者、原帖、日期，提示词里写了的时长和画幅，要不要参考图，原帖有视频的附成片链接。每一页都是全文。全部 205 条也在 [data/prompts.json](data/prompts.json)，[index.html](index.html) 是可以搜索、筛选、一键复制的浏览页。

## 这些提示词是怎么写的

- **参考图模板**：这里被转得最多的写法（31 条）。先做一张拼图当参考图，左边是人物大头照，右边是服装三视图。正文按「人物 / 道具 / 场景 / 光线 / 机位 / 分镜 / 风格 / 音频 / 参数 / 负面提示词」写，分镜按 0.3 秒一步写身体动作，切镜点都对准音乐重拍。
- **男友 POV**：一个连载系列（39 条），「镜头就是男友的眼睛」。竖屏 9:16、10 秒一镜到底，男友不入镜、最多露手或前臂，动作按 0-2 / 2-5 / 5-8 / 8-10 秒写，配一句台词。后面几集用一张角色参考图把女主固定下来。
- **Format lock、Master、Clip**：英文长提示词的写法。开头锁定画幅和源分辨率；然后是 Master 块，把人物和服装一字不改地写死，每段都重复带上；再按 Clip 分段写镜头，每段都有 Avoid 清单。舞蹈类另加 TEMPO LOCK，写明 BPM 和每个重拍的时间点。最长的有 6 段、约 1 分钟。
- **手机真实感**：自拍、vlog 和 POV 会故意要手机镜头的毛病：手持晃动、对焦呼吸、降噪涂抹、平台压缩、720p，并且明确禁止 HDR、影棚精修和全程锐利的脸。
- **系列连续性**：古风甜宠和仙侠双姝两个系列，用参考图加一段从不改动的人物描述固定角色，每集只换剧情或场景。
- **一句话指令**：Muse 是聊天式 agent，有些作者只说想要什么，分镜让它自己写，比如「把这条推特里的图片作为参考图，生成视频」「根据这个抖音视频的风格和分镜内容，复刻 10 个同样风格的视频」。这类指令要靠 Muse 自己打开链接、自己写提示词，只能在 Muse 应用里用，视频 API 做不到。

## 多镜头卡点（参考图模板）

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV001 | [午后居家·落地镜与黑猫](prompts/multi-shot-reference/MV001.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2113504588393566336) | [视频](https://video.twimg.com/amplify_video/2113504472098127872/vid/avc1/1280x720/-6axLaR11INug1B_.mp4?tag=29) |
| MV002 | [高架桥下广场·黄金时刻](prompts/multi-shot-reference/MV002.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2113823150815453207) | [视频](https://video.twimg.com/amplify_video/2113823115369410560/vid/avc1/720x1280/exPhlK_YIWKWiH36.mp4?tag=29) |
| MV003 | [公寓客厅·沙发区 A](prompts/multi-shot-reference/MV003.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2113939986546327674) | [视频](https://video.twimg.com/amplify_video/2113939958985834496/vid/avc1/1280x720/fxHJ0yihibAqeXws.mp4?tag=29) |
| MV004 | [高档小区户外广场](prompts/multi-shot-reference/MV004.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2114116645396598985) | [视频](https://video.twimg.com/amplify_video/2114116591222923264/vid/avc1/720x1280/EtLSHbu4wLACFOnP.mp4?tag=29) |
| MV005 | [居家厨房走到客厅](prompts/multi-shot-reference/MV005.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2114281614973010122) | [视频](https://video.twimg.com/amplify_video/2114281583586983936/vid/avc1/1152x768/LGjWF_fGdhVHnUBN.mp4?tag=29) |
| MV006 | [公寓客厅·沙发区 B](prompts/multi-shot-reference/MV006.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2114525481945153921) | [视频](https://video.twimg.com/amplify_video/2114525450915745792/vid/avc1/1280x720/3AVjfn68Rl3VV2yP.mp4?tag=29) |
| MV007 | [地毯侧躺·贴地自拍](prompts/multi-shot-reference/MV007.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2114731091450097970) | [视频](https://video.twimg.com/amplify_video/2114731059170668546/vid/avc1/1280x720/inxHr0husruFV6Um.mp4?tag=29) |
| MV008 | [小区步道·午后树影](prompts/multi-shot-reference/MV008.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2114963539811303572) | [视频](https://video.twimg.com/amplify_video/2114963510044282880/vid/avc1/720x1280/kpDG4QS_8UGat603.mp4?tag=29) |
| MV009 | [法式甜品店·下午茶](prompts/multi-shot-reference/MV009.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2114990404622008734) | — |
| MV010 | [欧式客厅·壁炉夜](prompts/multi-shot-reference/MV010.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2115034789447438791) | [视频](https://video.twimg.com/amplify_video/2115034734447525888/vid/avc1/1920x1080/_kIajZN3LI-5kS1R.mp4?tag=29) |
| MV011 | [苏州园林·月洞门](prompts/multi-shot-reference/MV011.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2115116836211847374) | — |
| MV012 | [地铁车厢](prompts/multi-shot-reference/MV012.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2115301628387655983) | [视频](https://video.twimg.com/amplify_video/2115301606828986368/vid/avc1/576x1024/PPo44AquQDrW30fb.mp4?tag=29) |
| MV013 | [参考视频换人·卧室自拍](prompts/multi-shot-reference/MV013.md) | [@sinvlo233](https://x.com/sinvlo233) | 10.11 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2115343148625105289) | — |
| MV014 | [地下通道·站立展示一镜到底](prompts/multi-shot-reference/MV014.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2115396536498815192) | [视频](https://video.twimg.com/amplify_video/2115396484493651969/vid/avc1/1080x1920/rDUzOj06Ua-7c8Do.mp4?tag=29) |
| MV015 | [工业风建筑·黑色连体衣 8 镜](prompts/multi-shot-reference/MV015.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2115498819223973934) | [视频](https://video.twimg.com/amplify_video/2115498763859193856/vid/avc1/1920x1080/iigIoe7QSK33tO7J.mp4?tag=29) |
| MV016 | [草地到黄金时刻人行道](prompts/multi-shot-reference/MV016.md) | [@sinvlo233](https://x.com/sinvlo233) | 8.01 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2115629982953427208) | — |
| MV017 | [白瓷砖通道·冷色调](prompts/multi-shot-reference/MV017.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2115632014300966950) | [视频](https://video.twimg.com/amplify_video/2115631965869367296/vid/avc1/720x1280/9v70MF7SPhNBQps7.mp4?tag=29) |
| MV018 | [地下停车场·冷光](prompts/multi-shot-reference/MV018.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 4:3 | [X](https://x.com/beizhi606/status/2115743677985542411) | [视频](https://video.twimg.com/amplify_video/2115743648315052032/vid/avc1/1152x768/-o91WCpTcHXipdFa.mp4?tag=29) |
| MV019 | [夜晚停车场·UNO +2 卡牌](prompts/multi-shot-reference/MV019.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2115886145427108239) | [视频](https://video.twimg.com/amplify_video/2115886117132337152/vid/avc1/1280x720/NgBTAnPaX-8ogwFw.mp4?tag=29) |
| MV020 | [老楼道与阳台·仰拍](prompts/multi-shot-reference/MV020.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2116083343238513062) | [视频](https://video.twimg.com/amplify_video/2116083313144397824/vid/avc1/720x1280/jTm_Ns9GMZxAo3vB.mp4?tag=29) |
| MV021 | [红墙宫门·红大衣卡点](prompts/multi-shot-reference/MV021.md) | [@sinvlo233](https://x.com/sinvlo233) | 8 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2116130531507335651) | — |
| MV022 | [枕边自拍·新视角](prompts/multi-shot-reference/MV022.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 9:16 | [X](https://x.com/beizhi606/status/2116160485544567010) | [视频](https://video.twimg.com/amplify_video/2116160442037141504/vid/avc1/720x1280/zgm2KgOC93lYHeaN.mp4?tag=29) |
| MV023 | [蓝调时刻·闪光灯人像](prompts/multi-shot-reference/MV023.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2116335801433002267) | [视频](https://video.twimg.com/amplify_video/2116335702011211776/vid/avc1/1152x768/WFg2gPwGAqqmkVDN.mp4?tag=29) |
| MV024 | [夜晚酒吧·鸡尾酒](prompts/multi-shot-reference/MV024.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2116373490811163022) | [视频](https://video.twimg.com/amplify_video/2116373330622328832/vid/avc1/1280x720/Ldz7duqnc_csmFTr.mp4?tag=29) |
| MV025 | [西部牛仔·傍晚营地](prompts/multi-shot-reference/MV025.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2116546724382789884) | [视频](https://video.twimg.com/amplify_video/2116546670997786625/vid/avc1/1280x720/IFc18BYRK2rGwloY.mp4?tag=29) |
| MV026 | [黑白天鹅·派对入场](prompts/multi-shot-reference/MV026.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2116583181923291370) | — |
| MV027 | [高铁二等座车厢](prompts/multi-shot-reference/MV027.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2116594198405402737) | — |
| MV028 | [时尚模特电影短片](prompts/multi-shot-reference/MV028.md) | [@qingshuzuo](https://x.com/qingshuzuo) | 10 秒 | 9:16 | [X](https://x.com/qingshuzuo/status/2116862420400607716) | [视频](https://video.twimg.com/amplify_video/2116862376683405312/vid/avc1/720x1280/UneGPewqOKfnA24D.mp4?tag=29) |
| MV029 | [现代卧室·落地窗](prompts/multi-shot-reference/MV029.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2116906985291444667) | [视频](https://video.twimg.com/amplify_video/2116906952119009280/vid/avc1/1280x720/5RLTP7NUpvLynDe9.mp4?tag=29) |
| MV030 | [行驶中的火车·4 镜](prompts/multi-shot-reference/MV030.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2117139486895386744) | [视频](https://video.twimg.com/amplify_video/2117139438614810624/vid/avc1/1152x768/HW3DITeywHoK-DzT.mp4?tag=29) |
| MV031 | [山顶木栏杆·晴空广角](prompts/multi-shot-reference/MV031.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2117265988509155445) | [视频](https://video.twimg.com/amplify_video/2117265654009200640/vid/avc1/1080x1920/111GUkVGPZrwsbAD.mp4?tag=29) |

## 男友 POV

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV032 | [玄关等你回家](prompts/boyfriend-pov/MV032.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105677515444691177) | [视频](https://video.twimg.com/amplify_video/2105677164473671680/vid/avc1/1280x720/ybX1TYvx_zWgUYEj.mp4?tag=29) |
| MV033 | [深夜客厅·小龙虾之夜](prompts/boyfriend-pov/MV033.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105680036309483529) | [视频](https://video.twimg.com/amplify_video/2105679642275495936/vid/avc1/720x1280/FcZM23NI72_m16yr.mp4?tag=29) |
| MV034 | [夜宵后三局两胜](prompts/boyfriend-pov/MV034.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105684399866159339) | [视频](https://video.twimg.com/amplify_video/2105683937205116929/vid/avc1/720x1280/26H7AnRGCXLZeFO4.mp4?tag=29) |
| MV035 | [阳台夜风（第 4 集）](prompts/boyfriend-pov/MV035.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106035377148723204) | — |
| MV036 | [你的衬衫（第 5 集）](prompts/boyfriend-pov/MV036.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106052875604361550) | — |
| MV037 | [撒娇三连（第 13 集）](prompts/boyfriend-pov/MV037.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106184006035493208) | — |
| MV038 | [雨天共撑一把伞](prompts/boyfriend-pov/MV038.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106185393574203745) | [视频](https://video.twimg.com/amplify_video/2106184663991820288/vid/avc1/720x1280/NXRAhQy6sC6hxTU5.mp4?tag=29) |
| MV039 | [客厅舞会·踩脚背](prompts/boyfriend-pov/MV039.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106386425252073486) | [视频](https://video.twimg.com/amplify_video/2106386255403737088/vid/avc1/720x1280/y5S-Mvn8K3z7ekuL.mp4?tag=29) |
| MV040 | [白衬衫的早晨](prompts/boyfriend-pov/MV040.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106398601324978451) | [视频](https://video.twimg.com/amplify_video/2106398427294932993/vid/avc1/720x1280/yThq9V6wuv-EH9va.mp4?tag=29) |
| MV041 | [出门前帮她扣鞋](prompts/boyfriend-pov/MV041.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106557061454803234) | [视频](https://video.twimg.com/amplify_video/2106556785331224576/vid/avc1/720x1280/VZYLfliPCKrNQTP6.mp4?tag=29) |
| MV042 | [连狗的醋都吃](prompts/boyfriend-pov/MV042.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106643634095624466) | [视频](https://video.twimg.com/amplify_video/2106643480743456768/vid/avc1/720x1280/rkp0rMuHLfMs_0h6.mp4?tag=29) |
| MV043 | [热舞到翻车](prompts/boyfriend-pov/MV043.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106735739107258714) | [视频](https://video.twimg.com/amplify_video/2106735647520399360/vid/avc1/720x1280/HzaIqyRrErJ8SPeU.mp4?tag=29) |
| MV044 | [夜市灯火·糖葫芦](prompts/boyfriend-pov/MV044.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106764215289827588) | [视频](https://video.twimg.com/amplify_video/2106764088646963200/vid/avc1/720x1280/7pfGUOcQhYL8aSmu.mp4?tag=29) |
| MV045 | [江边晚风（第 94 集）](prompts/boyfriend-pov/MV045.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106801702729089505) | [视频](https://video.twimg.com/amplify_video/2106801359731507201/vid/avc1/720x1280/yx1REiwZpFWls9R7.mp4?tag=29) |
| MV046 | [海边湿透了（第 108 集）](prompts/boyfriend-pov/MV046.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106906698481115171) | [视频](https://video.twimg.com/amplify_video/2106906573918625792/vid/avc1/720x1280/I14sZ01yYOEmAr-z.mp4?tag=29) |
| MV047 | [梳妆台梳头](prompts/boyfriend-pov/MV047.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106925730206761191) | [视频](https://video.twimg.com/amplify_video/2106925694274183168/vid/avc1/720x1280/sFbPaweCfAJR2s9L.mp4?tag=29) |
| MV048 | [雪地红裙](prompts/boyfriend-pov/MV048.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106939471266726122) | [视频](https://video.twimg.com/amplify_video/2106939307051429888/vid/avc1/720x1280/sLYAzdAqp2nNj0Bg.mp4?tag=29) |
| MV049 | [天台落日](prompts/boyfriend-pov/MV049.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106978313550102814) | [视频](https://video.twimg.com/amplify_video/2106977752494817280/vid/avc1/720x1280/0qBiMmmW9fW4c8kl.mp4?tag=29) |
| MV050 | [早晨厨房递吐司](prompts/boyfriend-pov/MV050.md) | [@noahvisualsx](https://x.com/noahvisualsx) | — | 9:16 | [X](https://x.com/noahvisualsx/status/2106950799662489702) | [视频](https://video.twimg.com/amplify_video/2106950729290424321/vid/avc1/720x1280/NnCaJiEh28kGazQF.mp4?tag=29) |
| MV051 | [口红印](prompts/boyfriend-pov/MV051.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107277645419561412) | [视频](https://video.twimg.com/amplify_video/2107277602683817984/vid/avc1/720x1280/SmzAOYevSNRcrWhB.mp4?tag=29) |
| MV052 | [天台晚风](prompts/boyfriend-pov/MV052.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107296871043744175) | [视频](https://video.twimg.com/amplify_video/2107296646283575297/vid/avc1/720x1280/VZaJlMsuXSj-K4oW.mp4?tag=29) |
| MV053 | [萤火](prompts/boyfriend-pov/MV053.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107299500054462539) | [视频](https://video.twimg.com/amplify_video/2107299454399508480/vid/avc1/720x1280/gRJkCPKoqg1bNE4U.mp4?tag=29) |
| MV054 | [勾魂](prompts/boyfriend-pov/MV054.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107325807287058803) | [视频](https://video.twimg.com/amplify_video/2107325759341924352/vid/avc1/720x1280/MUCIiP4PGaoMCVXA.mp4?tag=29) |
| MV055 | [海边回头](prompts/boyfriend-pov/MV055.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107341007495037314) | [视频](https://video.twimg.com/amplify_video/2107340791198969856/vid/avc1/720x1280/DNN37-jrK4_vjSIr.mp4?tag=29) |
| MV056 | [艺术画像](prompts/boyfriend-pov/MV056.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107353193579462871) | [视频](https://video.twimg.com/amplify_video/2107353141691994112/vid/avc1/720x1280/pr7JsjFXfIoUYWsH.mp4?tag=29) |
| MV057 | [囍·新婚之夜](prompts/boyfriend-pov/MV057.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107370561999659063) | [视频](https://video.twimg.com/amplify_video/2107370520937381888/vid/avc1/720x1280/QNm4g_bR0U9bKVTm.mp4?tag=29) |
| MV058 | [簪花](prompts/boyfriend-pov/MV058.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2107469753006887039) | [视频](https://video.twimg.com/amplify_video/2107469685197537280/vid/avc1/720x1280/zythLTC0Wzp7xoU-.mp4?tag=29) |
| MV059 | [约会前涂口红](prompts/boyfriend-pov/MV059.md) | [@7998l201](https://x.com/7998l201) | — | 9:16 | [X](https://x.com/7998l201/status/2107696165991116816) | — |
| MV060 | [晚霞阳台](prompts/boyfriend-pov/MV060.md) | [@7998l201](https://x.com/7998l201) | — | 9:16 | [X](https://x.com/7998l201/status/2107817277811020213) | — |
| MV061 | [跨年倒数](prompts/boyfriend-pov/MV061.md) | [@7998l201](https://x.com/7998l201) | — | 9:16 | [X](https://x.com/7998l201/status/2108058117435212122) | — |
| MV062 | [第一场雪](prompts/boyfriend-pov/MV062.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2108166833950130381) | — |
| MV063 | [窗边听雨](prompts/boyfriend-pov/MV063.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2108423287961534885) | — |
| MV064 | [楼下看星星](prompts/boyfriend-pov/MV064.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2108511091999539314) | — |
| MV065 | [阳台看日落](prompts/boyfriend-pov/MV065.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2108785278030925999) | — |
| MV066 | [卧室晨间调侃](prompts/boyfriend-pov/MV066.md) | [@xiaocao](https://x.com/xiaocao) | 10 秒 | — | [X](https://x.com/xiaocao/status/2114612211515879653) | — |
| MV067 | [下班后的地铁女友](prompts/boyfriend-pov/MV067.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2114720512824025542) | — |
| MV068 | [夜晚公寓玄关·真实抓拍](prompts/boyfriend-pov/MV068.md) | [@chlovelyn](https://x.com/chlovelyn) | 10 秒 | 9:16 | [X](https://x.com/chlovelyn/status/2114828719395320085) | — |
| MV069 | [深夜进门·客厅沙发](prompts/boyfriend-pov/MV069.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2115716998923456961) | — |
| MV070 | [卧室亲吻镜头（日文）](prompts/boyfriend-pov/MV070.md) | [@kusaionara0303](https://x.com/kusaionara0303) | 10 秒 | 9:16 | [X](https://x.com/kusaionara0303/status/2116840351713649007) | [视频](https://video.twimg.com/amplify_video/2116840329869742080/vid/avc1/720x1280/j9veByfvKAM_JdDD.mp4?tag=29) |

## 自拍 / Vlog

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV071 | [北京老城周五早晨·家庭录像](prompts/selfie-vlog/MV071.md) | [@DangcingAI](https://x.com/DangcingAI) | 30 秒 | — | [X](https://x.com/DangcingAI/status/2103883325236818177) | — |
| MV072 | [湿发浴室门口](prompts/selfie-vlog/MV072.md) | [@goan999999](https://x.com/goan999999) | 10 秒 | 9:16 | [X](https://x.com/goan999999/status/2105911238127718457) | — |
| MV073 | [湿发粉裙温馨版](prompts/selfie-vlog/MV073.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105938619659849995) | — |
| MV074 | [夜晚卧室沙发近景](prompts/selfie-vlog/MV074.md) | [@HarriesSteele](https://x.com/HarriesSteele) | — | — | [X](https://x.com/HarriesSteele/status/2105950707300048974) | — |
| MV075 | [手机自拍通用模板](prompts/selfie-vlog/MV075.md) | [@NeonScribe07](https://x.com/NeonScribe07) | — | 9:16 | [X](https://x.com/NeonScribe07/status/2106018068619292924) | [视频](https://video.twimg.com/amplify_video/2106017528271245312/vid/avc1/768x1152/OE0VbH9ULvWnLQXi.mp4?tag=29) |
| MV076 | [客厅地毯·害羞捂脸](prompts/selfie-vlog/MV076.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106033360782885302) | — |
| MV077 | [湿发粉裙温馨版（改写）](prompts/selfie-vlog/MV077.md) | [@Tao\_Builds](https://x.com/Tao_Builds) | 10 秒 | 9:16 | [X](https://x.com/Tao_Builds/status/2106328218617946220) | — |
| MV078 | [白墙穿搭自拍 vlog](prompts/selfie-vlog/MV078.md) | [@SpringHaoAI](https://x.com/SpringHaoAI) | 10 秒 | 9:16 | [X](https://x.com/SpringHaoAI/status/2107206368604344818) | — |
| MV079 | [白墙前置自拍·怼脸两段](prompts/selfie-vlog/MV079.md) | [@BlockInsight214](https://x.com/BlockInsight214) | 20 秒 | 9:16 | [X](https://x.com/BlockInsight214/status/2107255023541616804) | — |
| MV080 | [开门迎接·手持自拍](prompts/selfie-vlog/MV080.md) | [@JasonLiuLabs](https://x.com/JasonLiuLabs) | 10 秒 | 3:4 | [X](https://x.com/JasonLiuLabs/status/2107858197264359871) | — |
| MV081 | [粉色少女卧室·说话卖萌](prompts/selfie-vlog/MV081.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2113329938350973222) | [视频](https://video.twimg.com/amplify_video/2113329883715891200/vid/avc1/1152x768/zc4lYOVpD7IPc_x7.mp4?tag=29) |
| MV082 | [推门进来·栗棕盘发](prompts/selfie-vlog/MV082.md) | [@0x95279527](https://x.com/0x95279527) | 10 秒 | 9:16 | [X](https://x.com/0x95279527/status/2113529267103637920) | — |
| MV083 | [日本女孩前置自拍（英文）](prompts/selfie-vlog/MV083.md) | [@hai\_vara](https://x.com/hai_vara) | 10 秒 | 9:16 | [X](https://x.com/hai_vara/status/2113847654602191191) | [视频](https://video.twimg.com/amplify_video/2113847264896851968/vid/avc1/1180x2556/OVNxwKfg0Fgk2R-1.mp4?tag=29) |
| MV084 | [参考图女孩·多场景（日文）](prompts/selfie-vlog/MV084.md) | [@REXTokyo2](https://x.com/REXTokyo2) | 10 秒 | 9:16 | [X](https://x.com/REXTokyo2/status/2114632321282515052) | — |
| MV085 | [列车车厢·眼镜女孩（图生视频）](prompts/selfie-vlog/MV085.md) | [@BaiSu\_M](https://x.com/BaiSu_M) | 10 秒 | — | [X](https://x.com/BaiSu_M/status/2115364993751466449) | — |
| MV086 | [图生视频·转头微笑（日文）](prompts/selfie-vlog/MV086.md) | [@gagarot200](https://x.com/gagarot200) | — | 9:16 | [X](https://x.com/gagarot200/status/2115339029348495858) | [视频](https://video.twimg.com/amplify_video/2115159478102618113/vid/avc1/1170x2064/ivKvTX2CdSg3fQAy.mp4?tag=29) |
| MV087 | [微醺女孩·出租车后座（一）](prompts/selfie-vlog/MV087.md) | [@real404world](https://x.com/real404world) | 10 秒 | 9:16 | [X](https://x.com/real404world/status/2115766888462766145) | — |
| MV088 | [每天定时发自拍视频（日文）](prompts/selfie-vlog/MV088.md) | [@Sadal\_Quari](https://x.com/Sadal_Quari) | — | 9:16 | [X](https://x.com/Sadal_Quari/status/2115774897775346041) | — |
| MV089 | [微醺女孩·出租车自拍（二）](prompts/selfie-vlog/MV089.md) | [@real404world](https://x.com/real404world) | 10 秒 | 9:16 | [X](https://x.com/real404world/status/2115808054176559379) | — |
| MV090 | [10 秒自拍四段模板（日文）](prompts/selfie-vlog/MV090.md) | [@rlu1598451](https://x.com/rlu1598451) | 3 秒 | — | [X](https://x.com/rlu1598451/status/2115955266516836377) | — |
| MV091 | [面包房外·冰咖啡俏皮眨眼](prompts/selfie-vlog/MV091.md) | [@DeepBlueX0](https://x.com/DeepBlueX0) | — | 9:16 | [X](https://x.com/DeepBlueX0/status/2116013694840983796) | [视频](https://video.twimg.com/amplify_video/2116013626809372672/vid/avc1/704x1248/qV6QjbcoCwxZuUeb.mp4?tag=29) |
| MV092 | [白墙前置自拍·怼脸卡点](prompts/selfie-vlog/MV092.md) | [@Crypto\_146827](https://x.com/Crypto_146827) | 10 秒 | 9:16 | [X](https://x.com/Crypto_146827/status/2116590227921998196) | — |
| MV093 | [失败自拍感·逆向提示词](prompts/selfie-vlog/MV093.md) | [@leaf\_sanren](https://x.com/leaf_sanren) | 10 秒 | 9:16 | [X](https://x.com/leaf_sanren/status/2116479544127300077) | [视频](https://video.twimg.com/amplify_video/2116468567508217856/vid/avc1/720x1280/cGAr3VC6-uZkDD0p.mp4?tag=29) |
| MV094 | [前置自拍 vlog 一镜到底](prompts/selfie-vlog/MV094.md) | [@superlewis88](https://x.com/superlewis88) | 10 秒 | 9:16 | [X](https://x.com/superlewis88/status/2116755225310793808) | — |
| MV095 | [杭州春日老街·DV 质感](prompts/selfie-vlog/MV095.md) | [@lucky46017](https://x.com/lucky46017) | 10 秒 | 16:9 | [X](https://x.com/lucky46017/status/2117386563793617155) | — |
| MV096 | [Vesper Vlog·多伦多秋日咖啡馆](prompts/selfie-vlog/MV096.md) | [@HuanAIart](https://x.com/HuanAIart) | 20 秒 | — | [X](https://x.com/HuanAIart/status/2117473374192468306) | — |
| MV097 | [Vesper Vlog 002·多伦多唐人街](prompts/selfie-vlog/MV097.md) | [@HuanAIart](https://x.com/HuanAIart) | 30 秒 | 9:16 | [X](https://x.com/HuanAIart/status/2117476520453115915) | — |
| MV098 | [唐长安 vlog 20 秒](prompts/selfie-vlog/MV098.md) | [@HuanAIart](https://x.com/HuanAIart) | 20 秒 | 9:16 | [X](https://x.com/HuanAIart/status/2117788326966997151) | — |

## 舞蹈

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV099 | [白墙前卡点手势舞（真人实拍）](prompts/dance/MV099.md) | [@li9292](https://x.com/li9292) | 10 秒 | 9:16 | [X](https://x.com/li9292/status/2105706754474639671) | [视频](https://video.twimg.com/amplify_video/2105706675432747009/vid/avc1/720x1280/8cK1iuCmczlbNvzT.mp4?tag=29) |
| MV100 | [珊瑚橙模特·影棚舞蹈](prompts/dance/MV100.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106227858750558701) | [视频](https://video.twimg.com/amplify_video/2106226999408857088/vid/avc1/720x1280/J4B_Gv0uREsQsQl9.mp4?tag=29) |
| MV101 | [古风纱裙·复刻参考舞](prompts/dance/MV101.md) | [@7998l201](https://x.com/7998l201) | 9 秒 | — | [X](https://x.com/7998l201/status/2106730824448217177) | [视频](https://video.twimg.com/amplify_video/2106730564250439680/vid/avc1/720x1280/raHhCePc7WlO_XSV.mp4?tag=29) |
| MV102 | [虚拟爱豆舞台直拍](prompts/dance/MV102.md) | [@mnmn94253156337](https://x.com/mnmn94253156337) | — | 9:16 | [X](https://x.com/mnmn94253156337/status/2108108576275480897) | — |
| MV103 | [衣帽间扭胯舞](prompts/dance/MV103.md) | [@beizhi606](https://x.com/beizhi606) | 10 秒 | 16:9 | [X](https://x.com/beizhi606/status/2113450998194934049) | [视频](https://video.twimg.com/amplify_video/2113450965714259968/vid/avc1/1248x704/9ZYBTTsZD9oc4w5L.mp4?tag=29) |
| MV104 | [旗袍捣年糕舞](prompts/dance/MV104.md) | [@sandmrk](https://x.com/sandmrk) | 12 秒 | 9:16 | [X](https://x.com/sandmrk/status/2115577558091833534) | — |
| MV105 | [中式内景旗袍慢摇](prompts/dance/MV105.md) | [@sandmrk](https://x.com/sandmrk) | 8 秒 | 9:16 | [X](https://x.com/sandmrk/status/2115666949975814639) | — |
| MV106 | [敦煌飞天群舞（两段）](prompts/dance/MV106.md) | [@sinvlo233](https://x.com/sinvlo233) | 20 秒 | 16:9 | [X](https://x.com/sinvlo233/status/2115688986886996394) | — |
| MV107 | [金殿猫爪三连舞](prompts/dance/MV107.md) | [@sandmrk](https://x.com/sandmrk) | 11 秒 | 9:16 | [X](https://x.com/sandmrk/status/2115834982996525446) | — |
| MV108 | [浅色墙前慢手势舞](prompts/dance/MV108.md) | [@sandmrk](https://x.com/sandmrk) | 9 秒 | 9:16 | [X](https://x.com/sandmrk/status/2115934345320145227) | — |
| MV109 | [卧室转圈裙摆舞](prompts/dance/MV109.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2115986332791324836) | — |
| MV110 | [白色影棚·手扶后脑慢摇](prompts/dance/MV110.md) | [@sandmrk](https://x.com/sandmrk) | 3 秒 | 9:16 | [X](https://x.com/sandmrk/status/2116038076002861245) | — |
| MV111 | [指尖点拍舞（126 BPM）](prompts/dance/MV111.md) | [@sandmrk](https://x.com/sandmrk) | 7.5 秒 | 9:16 | [X](https://x.com/sandmrk/status/2116104185481674891) | — |
| MV112 | [试衣间慢舞](prompts/dance/MV112.md) | [@sinvlo233](https://x.com/sinvlo233) | 10 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2116575902649966793) | — |

## 时尚人像

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV113 | [车展活动现场时尚人像](prompts/fashion-portrait/MV113.md) | [@leaf\_sanren](https://x.com/leaf_sanren) | 15 秒 | 9:16 | [X](https://x.com/leaf_sanren/status/2105645639703183753) | [视频](https://video.twimg.com/amplify_video/2105645218175557632/vid/avc1/720x1280/SoNR2QeeNHojNKIu.mp4?tag=29) |
| MV114 | [时尚人像短片 15 秒（两段拼接）](prompts/fashion-portrait/MV114.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105851302773497873) | — |
| MV115 | [珊瑚橙模特·影棚人像](prompts/fashion-portrait/MV115.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2106020052424351846) | [视频](https://video.twimg.com/amplify_video/2106019907884429312/vid/avc1/720x1280/-xzBC7tG2BbL_8kG.mp4?tag=29) |
| MV116 | [时尚人像短片·真实肤质](prompts/fashion-portrait/MV116.md) | [@fuji\_ai\_](https://x.com/fuji_ai_) | 15 秒 | 9:16 | [X](https://x.com/fuji_ai_/status/2107078481691783425) | — |
| MV117 | [日本街头清晨人像](prompts/fashion-portrait/MV117.md) | [@Pengchenop](https://x.com/Pengchenop) | — | — | [X](https://x.com/Pengchenop/status/2109467886905671897) | — |
| MV118 | [极近面部特写·电影肖像](prompts/fashion-portrait/MV118.md) | [@fly\_in\_X](https://x.com/fly_in_X) | 15 秒 | 9:16 | [X](https://x.com/fly_in_X/status/2111278110541058258) | — |
| MV119 | [日本小镇天桥·甜笑人像](prompts/fashion-portrait/MV119.md) | [@fly\_in\_X](https://x.com/fly_in_X) | 6 秒 | 9:16 | [X](https://x.com/fly_in_X/status/2111468463462220056) | — |
| MV120 | [渡轮上的米色风衣女孩](prompts/fashion-portrait/MV120.md) | [@supereasyit](https://x.com/supereasyit) | 10 秒 | — | [X](https://x.com/supereasyit/status/2115445302132175099) | — |
| MV121 | [银发旗袍魔女·姿态展示](prompts/fashion-portrait/MV121.md) | [@sandmrk](https://x.com/sandmrk) | 10 秒 | 9:16 | [X](https://x.com/sandmrk/status/2115469192854147255) | — |
| MV122 | [苗族少女·蓝蝶落鼻尖](prompts/fashion-portrait/MV122.md) | [@sandmrk](https://x.com/sandmrk) | 11 秒 | 16:9 | [X](https://x.com/sandmrk/status/2116024468053356887) | — |
| MV123 | [夜街手势人像](prompts/fashion-portrait/MV123.md) | [@hellsing00fl](https://x.com/hellsing00fl) | 10 秒 | 9:16 | [X](https://x.com/hellsing00fl/status/2117456100362686619) | [视频](https://video.twimg.com/amplify_video/2117455901280075776/vid/avc1/720x1280/Qme8LNq9oov8-0Wu.mp4?tag=29) |
| MV124 | [夜街人像·贴近抓拍](prompts/fashion-portrait/MV124.md) | [@hellsing00fl](https://x.com/hellsing00fl) | 10 秒 | 9:16 | [X](https://x.com/hellsing00fl/status/2117457287765950784) | [视频](https://video.twimg.com/amplify_video/2117457049038852096/vid/avc1/720x1280/t5LZX40920L9XOYD.mp4?tag=29) |

## 转场 / 变装

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV125 | [时尚造型图册 MV 15 秒](prompts/transitions/MV125.md) | [@li9292](https://x.com/li9292) | 15 秒 | 16:9 | [X](https://x.com/li9292/status/2105727318291341602) | [视频](https://video.twimg.com/amplify_video/2105727270090407936/vid/avc1/1280x720/e8SS8ThDLXIfUoQb.mp4?tag=29) |
| MV126 | [甩头变装·海边红裙](prompts/transitions/MV126.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105998485891977578) | — |
| MV127 | [手机变装转场（隐藏硬切）](prompts/transitions/MV127.md) | [@hellsing00fl](https://x.com/hellsing00fl) | 10 秒 | 9:16 | [X](https://x.com/hellsing00fl/status/2117459617051713837) | [视频](https://video.twimg.com/amplify_video/2117459154411622400/vid/avc1/720x1280/yXTrUE4UDtC2k8Bt.mp4?tag=29) |
| MV128 | [楼梯间硬切两镜](prompts/transitions/MV128.md) | [@hellsing00fl](https://x.com/hellsing00fl) | 10 秒 | 16:9 | [X](https://x.com/hellsing00fl/status/2117461986841915504) | [视频](https://video.twimg.com/amplify_video/2117461634658832384/vid/avc1/1280x720/lCku7zQomu_-OA2Q.mp4?tag=29) |
| MV129 | [商店街衣装切换（日文）](prompts/transitions/MV129.md) | [@TarouKim10504](https://x.com/TarouKim10504) | 10 秒 | 9:16 | [X](https://x.com/TarouKim10504/status/2117752544546222510) | [视频](https://video.twimg.com/amplify_video/2117750672238301184/vid/avc1/704x1248/ycJQYHleQdZQiGxd.mp4?tag=29) |

## 古风 / 历史

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV130 | [竹林石台·白衣剑舞](prompts/period-historical/MV130.md) | [@RealHanyaHu](https://x.com/RealHanyaHu) | — | — | [X](https://x.com/RealHanyaHu/status/2100835401552597309) | [视频](https://video.twimg.com/amplify_video/2100835218869653504/vid/avc1/1280x720/77ocR4MvSJszKMbt.mp4?tag=29) |
| MV131 | [咸阳城东楼·水墨诗词 5 段](prompts/period-historical/MV131.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | 9:16 | [X](https://x.com/7998l201/status/2105634195863457928) | [视频](https://video.twimg.com/amplify_video/2105633414774951936/vid/avc1/720x1280/_kBg3sQXNCiUjV8u.mp4?tag=29) |
| MV132 | [将进酒·唐朝宴会 45 秒](prompts/period-historical/MV132.md) | [@PixelAigc](https://x.com/PixelAigc) | 45 秒 | 16:9 | [X](https://x.com/PixelAigc/status/2106621355865133102) | [视频](https://video.twimg.com/amplify_video/2106621271597551616/vid/avc1/1280x720/g5kkIHlzTNeI9u2K.mp4?tag=29) |
| MV133 | [仙侠双姝·海底龙宫到云端天宫](prompts/period-historical/MV133.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106664982566031774) | — |
| MV134 | [仙侠双姝·悬崖飞檐](prompts/period-historical/MV134.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106680907532997015) | [视频](https://video.twimg.com/amplify_video/2106680638820814848/vid/avc1/1280x720/LvbgQ-L0lpodVKwT.mp4?tag=29) |
| MV135 | [仙侠双姝·金色云海](prompts/period-historical/MV135.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106721239498903809) | [视频](https://video.twimg.com/amplify_video/2106721076072116226/vid/avc1/1280x720/SLhqgVrcrufRx8td.mp4?tag=29) |
| MV136 | [仙侠双姝·雪山冰裂缝](prompts/period-historical/MV136.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106751168370377150) | — |
| MV137 | [仙侠双姝·竹海水乡](prompts/period-historical/MV137.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106751531328635125) | — |
| MV138 | [仙侠双姝·上元灯会](prompts/period-historical/MV138.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106921140065345662) | [视频](https://video.twimg.com/amplify_video/2106920877480960000/vid/avc1/1280x720/C8Fpm7Be1iw0bl2h.mp4?tag=29) |
| MV139 | [仙侠双姝·月夜桂花林](prompts/period-historical/MV139.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107035456772903259) | [视频](https://video.twimg.com/amplify_video/2107035051439648768/vid/avc1/1280x720/dyXVsIOkOgz11w5E.mp4?tag=29) |
| MV140 | [古风甜宠·夏夜灯下](prompts/period-historical/MV140.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107090279086076220) | [视频](https://video.twimg.com/amplify_video/2107089610753142784/vid/avc1/1152x720/nujKmwEHUz4DvHxT.mp4?tag=29) |
| MV141 | [古风甜宠·秋千（续集 3）](prompts/period-historical/MV141.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107093715059700140) | [视频](https://video.twimg.com/amplify_video/2107093650132140032/vid/avc1/1280x720/KLccJ48ZI5_KD0iv.mp4?tag=29) |
| MV142 | [古风甜宠·吃醋（续集 4）](prompts/period-historical/MV142.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107145726254059734) | [视频](https://video.twimg.com/amplify_video/2107145674085273601/vid/avc1/1152x720/6El17gWJhCbgb5lN.mp4?tag=29) |
| MV143 | [古风甜宠·量衣（续集 5）](prompts/period-historical/MV143.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107146150990250152) | [视频](https://video.twimg.com/amplify_video/2107146109831548930/vid/avc1/1152x720/r0gyJP-vAstOrCIU.mp4?tag=29) |
| MV144 | [古风甜宠·偷亲（续集 6）](prompts/period-historical/MV144.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107155598399980003) | [视频](https://video.twimg.com/amplify_video/2107155551675461632/vid/avc1/1152x720/tTOnM31HwV6l0MGc.mp4?tag=29) |
| MV145 | [古风甜宠·水袖（续集 7）](prompts/period-historical/MV145.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2107156702651121731) | [视频](https://video.twimg.com/amplify_video/2107156628852396032/vid/avc1/1280x720/tTmKMuNnlZZ8QB2T.mp4?tag=29) |
| MV146 | [清明上河图动态活化 43 秒](prompts/period-historical/MV146.md) | [@duange6099](https://x.com/duange6099) | 43 秒 | — | [X](https://x.com/duange6099/status/2108368549307994513) | [视频](https://video.twimg.com/amplify_video/2108368226505949184/vid/avc1/1280x720/pVRd9qnStuX-YGSL.mp4?tag=29) |
| MV147 | [古装片一镜到底·35mm](prompts/period-historical/MV147.md) | [@PixelAigc](https://x.com/PixelAigc) | 10 秒 | 16:9 | [X](https://x.com/PixelAigc/status/2109161374689726818) | — |
| MV148 | [穿越成皇后的第三天](prompts/period-historical/MV148.md) | [@sandmrk](https://x.com/sandmrk) | 55 秒 | 9:16 | [X](https://x.com/sandmrk/status/2116061912442261546) | — |
| MV149 | [北宋汴梁夜市 POV](prompts/period-historical/MV149.md) | [@zhu185178](https://x.com/zhu185178) | 1 分钟 | — | [X](https://x.com/zhu185178/status/2117098199752290657) | [视频](https://video.twimg.com/amplify_video/2117097901138874368/vid/avc1/1280x720/YCK_mtLHnGz36u2l.mp4?tag=29) |
| MV150 | [皇帝第一视角](prompts/period-historical/MV150.md) | [@sandmrk](https://x.com/sandmrk) | 49.6 秒 | 9:16 | [X](https://x.com/sandmrk/status/2117243590661562547) | — |
| MV151 | [古装剑客与紫裙女子·11 镜](prompts/period-historical/MV151.md) | [@ddny09](https://x.com/ddny09) | — | — | [X](https://x.com/ddny09/status/2117420842443587846) | — |
| MV205 | [竹海古装双姝高速穿行](prompts/period-historical/MV205.md) | [@7998l201](https://x.com/7998l201) | 10 秒 | — | [X](https://x.com/7998l201/status/2106699139908276470) | [视频](https://video.twimg.com/amplify_video/2106698860794138624/vid/avc1/1280x720/33Lil76P1RTDI6CG.mp4?tag=29) |

## 奇幻 / 动画 CG

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV152 | [梵高星月夜油画动态](prompts/fantasy-animation/MV152.md) | [@voidJan](https://x.com/voidJan) | — | — | [X](https://x.com/voidJan/status/2108198418728595864) | [视频](https://video.twimg.com/amplify_video/2108196805137883138/vid/avc1/1920x1080/FiyQPZQ8CSfOqj_2.mp4?tag=29) |
| MV153 | [海边坡道骑车·日常系动漫](prompts/fantasy-animation/MV153.md) | [@Polaksky](https://x.com/Polaksky) | — | — | [X](https://x.com/Polaksky/status/2112540091663155515) | — |
| MV154 | [云端白衣蒙眼仙子](prompts/fantasy-animation/MV154.md) | [@BaiSu\_M](https://x.com/BaiSu_M) | 10 秒 | 16:9 | [X](https://x.com/BaiSu_M/status/2115631959200223364) | [视频](https://video.twimg.com/amplify_video/2115620317389529088/vid/avc1/1216x640/pqEJj6B_wvlRrRXn.mp4?tag=29) |
| MV155 | [王城焚夜·白银女王](prompts/fantasy-animation/MV155.md) | [@sandmrk](https://x.com/sandmrk) | 34.6 秒 | 16:9 | [X](https://x.com/sandmrk/status/2115640170146071035) | — |
| MV156 | [火焰仪式·银甲红瞳](prompts/fantasy-animation/MV156.md) | [@sandmrk](https://x.com/sandmrk) | 10 秒 | 9:16 | [X](https://x.com/sandmrk/status/2115707898592694428) | — |
| MV157 | [翡翠洞窟·发光锦鲤泉](prompts/fantasy-animation/MV157.md) | [@hanagekkou](https://x.com/hanagekkou) | 10 秒 | 16:9 | [X](https://x.com/hanagekkou/status/2115708607497138599) | [视频](https://video.twimg.com/amplify_video/2115708502543097857/vid/avc1/1280x720/sSUSdBa0y2Wq5PJB.mp4?tag=29) |
| MV158 | [橘猫 3D 喜剧短片模板](prompts/fantasy-animation/MV158.md) | [@0xAIxiaobei](https://x.com/0xAIxiaobei) | 15 秒 | 9:16 | [X](https://x.com/0xAIxiaobei/status/2115667657924149557) | — |
| MV159 | [Q 版三姐妹说早安](prompts/fantasy-animation/MV159.md) | [@sinvlo233](https://x.com/sinvlo233) | 5 秒 | 9:16 | [X](https://x.com/sinvlo233/status/2115984127371485530) | [视频](https://video.twimg.com/amplify_video/2115984069242896384/vid/avc1/960x960/0YnD306ketKLV7yA.mp4?tag=29) |
| MV160 | [麻薯与海苔·故事板分镜](prompts/fantasy-animation/MV160.md) | [@Leviwoyun](https://x.com/Leviwoyun) | 30 秒 | — | [X](https://x.com/Leviwoyun/status/2116023791130386583) | — |
| MV161 | [涂鸦小人闯建筑实景](prompts/fantasy-animation/MV161.md) | [@sandmrk](https://x.com/sandmrk) | 15 秒 | 16:9 | [X](https://x.com/sandmrk/status/2116053439432237520) | — |
| MV162 | [水墨剑客·墨随剑舞](prompts/fantasy-animation/MV162.md) | [@sandmrk](https://x.com/sandmrk) | 28 秒 | 16:9 | [X](https://x.com/sandmrk/status/2116789171067174999) | — |
| MV163 | [骑行穿越画中风景](prompts/fantasy-animation/MV163.md) | [@sandmrk](https://x.com/sandmrk) | 7 秒 | 16:9 | [X](https://x.com/sandmrk/status/2116800255849288069) | — |
| MV164 | [冰龙驯龙师](prompts/fantasy-animation/MV164.md) | [@sandmrk](https://x.com/sandmrk) | 26.4 秒 | 16:9 | [X](https://x.com/sandmrk/status/2116859571301941453) | — |
| MV165 | [两个 Q 版小女孩](prompts/fantasy-animation/MV165.md) | [@sandmrk](https://x.com/sandmrk) | 15.1 秒 | 3:4 | [X](https://x.com/sandmrk/status/2117547331583410186) | — |

## 纪实 / 风光

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV166 | [南方乡村细雨田野](prompts/documentary-landscape/MV166.md) | [@yangleiocx3](https://x.com/yangleiocx3) | 15 秒 | — | [X](https://x.com/yangleiocx3/status/2106341712100532723) | [视频](https://video.twimg.com/amplify_video/2106341470475022336/vid/avc1/1280x720/XXCAw69-xqdx91dG.mp4?tag=29) |
| MV167 | [荒野建造类通用模板](prompts/documentary-landscape/MV167.md) | [@starkljm](https://x.com/starkljm) | 10 秒 | 9:16 | [X](https://x.com/starkljm/status/2115462631536689320) | [视频](https://video.twimg.com/amplify_video/2115462489035218944/vid/avc1/1080x1920/P8hEhHXC5qVyzODa.mp4?tag=29) |
| MV168 | [暴雨夜雪山垭口登山者](prompts/documentary-landscape/MV168.md) | [@Leviwoyun](https://x.com/Leviwoyun) | 15 秒 | — | [X](https://x.com/Leviwoyun/status/2115681567981080707) | — |
| MV169 | [藏区古镇与黑牦牛](prompts/documentary-landscape/MV169.md) | [@leaf\_sanren](https://x.com/leaf_sanren) | 10 秒 | 16:9 | [X](https://x.com/leaf_sanren/status/2115780679669858611) | [视频](https://video.twimg.com/amplify_video/2115779867879108609/vid/avc1/1280x720/bvDax5BkQei5GRNg.mp4?tag=29) |
| MV170 | [西北高原牧民赶羊](prompts/documentary-landscape/MV170.md) | [@leaf\_sanren](https://x.com/leaf_sanren) | 10 秒 | 16:9 | [X](https://x.com/leaf_sanren/status/2115780679669858611) | [视频](https://video.twimg.com/amplify_video/2115779867879108609/vid/avc1/1280x720/bvDax5BkQei5GRNg.mp4?tag=29) |
| MV171 | [南方老渔港·夏日傍晚](prompts/documentary-landscape/MV171.md) | [@RockTheWind](https://x.com/RockTheWind) | 10 秒 | 4:3 | [X](https://x.com/RockTheWind/status/2115990396207772036) | — |
| MV172 | [萨赫勒黎明·牧人](prompts/documentary-landscape/MV172.md) | [@LigtManTogo](https://x.com/LigtManTogo) | 10 秒 | 16:9 | [X](https://x.com/LigtManTogo/status/2116004346244796701) | [视频](https://video.twimg.com/amplify_video/2116003467093516288/vid/avc1/1280x720/cZ0cmRV-TbgidrLN.mp4?tag=29) |
| MV173 | [埃塞俄比亚老人人文特写](prompts/documentary-landscape/MV173.md) | [@leaf\_sanren](https://x.com/leaf_sanren) | 10 秒 | 16:9 | [X](https://x.com/leaf_sanren/status/2116033102573347229) | [视频](https://video.twimg.com/amplify_video/2116016983510839296/vid/avc1/1280x720/mmrprQ87XZAfp-ew.mp4?tag=29) |
| MV174 | [江南银杏大道·深秋](prompts/documentary-landscape/MV174.md) | [@RockTheWind](https://x.com/RockTheWind) | 10 秒 | 4:3 | [X](https://x.com/RockTheWind/status/2116498141826662402) | — |

## ASMR

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV175 | [河边野餐垫·石头 ASMR](prompts/asmr/MV175.md) | [@DeepBlueX0](https://x.com/DeepBlueX0) | 10 秒 | 9:16 | [X](https://x.com/DeepBlueX0/status/2115347819557261557) | [视频](https://video.twimg.com/amplify_video/2115347738091286529/vid/avc1/1080x1920/r7bH-kzkjDrhijPn.mp4?tag=29) |
| MV176 | [清宫夜雨荷塘 ASMR](prompts/asmr/MV176.md) | [@DeepBlueX0](https://x.com/DeepBlueX0) | 8 秒 | 9:16 | [X](https://x.com/DeepBlueX0/status/2116920472541536761) | [视频](https://video.twimg.com/amplify_video/2116920195797090304/vid/avc1/1080x1920/Zp-INBbaQed-K_JL.mp4?tag=29) |

## 电影感 / 剧情

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV177 | [喜极而泣·纯色背景特写](prompts/cinematic-story/MV177.md) | [@jarvis11x](https://x.com/jarvis11x) | — | — | [X](https://x.com/jarvis11x/status/2106617345418428515) | — |
| MV178 | [搞笑动物名场面复刻](prompts/cinematic-story/MV178.md) | [@liangzhu\_AI](https://x.com/liangzhu_AI) | 10 秒 | 9:16 | [X](https://x.com/liangzhu_AI/status/2109858384359100641) | — |
| MV179 | [大阪商业街·黄昏跟拍](prompts/cinematic-story/MV179.md) | [@Super\_Nius](https://x.com/Super_Nius) | — | — | [X](https://x.com/Super_Nius/status/2112961487107149929) | — |
| MV180 | [小剧场演唱会·民谣独唱](prompts/cinematic-story/MV180.md) | [@RohoQinAI](https://x.com/RohoQinAI) | 15 秒 | 9:16 | [X](https://x.com/RohoQinAI/status/2113586244538306739) | [视频](https://video.twimg.com/amplify_video/2113572916864471040/vid/avc1/720x1280/ySHWTz8Ui8-4Z0Cf.mp4?tag=29) |
| MV181 | [清晨咖啡店](prompts/cinematic-story/MV181.md) | [@0xPasswd](https://x.com/0xPasswd) | 5 秒 | 9:16 | [X](https://x.com/0xPasswd/status/2115025473969197399) | — |

## 长视频 / 多段脚本

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV182 | [万圣节 30 秒·三段](prompts/long-form/MV182.md) | [@NeonScribe07](https://x.com/NeonScribe07) | 30 秒 | 9:16 | [X](https://x.com/NeonScribe07/status/2105686412179951984) | [视频](https://video.twimg.com/amplify_video/2105686368483749888/vid/avc1/704x1248/yGlYwM2IWHyNXkzl.mp4?tag=29) |
| MV183 | [90 年代港片打戏 60 秒](prompts/long-form/MV183.md) | [@jarvis11x](https://x.com/jarvis11x) | 10 秒 | 16:9 | [X](https://x.com/jarvis11x/status/2105693376636952754) | — |
| MV184 | [iPhone 动态锁屏互动视频 29 秒](prompts/long-form/MV184.md) | [@7998l201](https://x.com/7998l201) | 29 秒 | 9:16 | [X](https://x.com/7998l201/status/2105882755435557370) | — |
| MV185 | [旗袍麻将 30 秒·8 镜](prompts/long-form/MV185.md) | [@jarvis11x](https://x.com/jarvis11x) | 30 秒 | 16:9 | [X](https://x.com/jarvis11x/status/2106034358821753092) | — |
| MV186 | [桃花源记·国风动画脚本](prompts/long-form/MV186.md) | [@linxiaobei888](https://x.com/linxiaobei888) | 6 分钟 | 16:9 | [X](https://x.com/linxiaobei888/status/2114605592140537901) | — |
| MV187 | [肉じゃが料理短片 60 秒（日文）](prompts/long-form/MV187.md) | [@old\_pgmrs\_will](https://x.com/old_pgmrs_will) | 1 分钟 | 16:9 | [X](https://x.com/old_pgmrs_will/status/2114714489174249503) | — |
| MV188 | [画皮·聊斋短片](prompts/long-form/MV188.md) | [@Lznnn1999](https://x.com/Lznnn1999) | 90 秒 | — | [X](https://x.com/Lznnn1999/status/2116207686471823399) | [视频](https://video.twimg.com/amplify_video/2116206928678531077/vid/avc1/720x1280/Spx76A_A6oAgn4qZ.mp4?tag=29) |
| MV189 | [2350 年醒来·科幻喜剧 POV](prompts/long-form/MV189.md) | [@sandmrk](https://x.com/sandmrk) | 59 秒 | 3:4 | [X](https://x.com/sandmrk/status/2116428925014339974) | — |
| MV190 | [长滑板下坡·10 秒叠接](prompts/long-form/MV190.md) | [@Kashiko\_AIart](https://x.com/Kashiko_AIart) | 10 秒 | — | [X](https://x.com/Kashiko_AIart/status/2116460269664670066) | [视频](https://video.twimg.com/amplify_video/2116460209388572672/vid/avc1/720x1278/lVqPZwXjywZLVVay.mp4?tag=29) |
| MV191 | [巨物治愈·夏日白日梦](prompts/long-form/MV191.md) | [@sandmrk](https://x.com/sandmrk) | 58 秒 | 16:9 | [X](https://x.com/sandmrk/status/2116493818677878793) | — |
| MV192 | [钟楼之城·白发女战士](prompts/long-form/MV192.md) | [@sandmrk](https://x.com/sandmrk) | 59.3 秒 | 16:9 | [X](https://x.com/sandmrk/status/2117490566892269752) | — |

## 一句话 / 对话式

| # | 提示词 | 作者 | 时长 | 画幅 | 原帖 | 成片 |
| --- | --- | --- | --- | --- | --- | --- |
| MV193 | [火星生存 180 秒短片](prompts/one-liners/MV193.md) | [@ksky](https://x.com/ksky) | 3 分钟 | — | [X](https://x.com/ksky/status/2100490906436858353) | [视频](https://video.twimg.com/amplify_video/2100490497865420800/vid/avc1/1920x1080/Oyv8IEv4338Vwtgo.mp4?tag=29) |
| MV194 | [斯里兰卡人说 Ayubowan（英文）](prompts/one-liners/MV194.md) | [@chenuka\_j](https://x.com/chenuka_j) | — | — | [X](https://x.com/chenuka_j/status/2102802573099143637) | [视频](https://video.twimg.com/amplify_video/2102801960847978496/vid/avc1/1280x720/x_hxkI6MnaV6o5b0.mp4?tag=14) |
| MV195 | [童话小镇骑自行车](prompts/one-liners/MV195.md) | [@EianLu](https://x.com/EianLu) | — | — | [X](https://x.com/EianLu/status/2103842716836872375) | [视频](https://video.twimg.com/amplify_video/2103842023598149632/vid/avc1/1152x768/-KHDOgzcCEKYxc3a.mp4?tag=29) |
| MV196 | [按帖子链接复刻天宫视频](prompts/one-liners/MV196.md) | [@jarvis11x](https://x.com/jarvis11x) | — | — | [X](https://x.com/jarvis11x/status/2105515798915694902) | — |
| MV197 | [替换视频里的人物](prompts/one-liners/MV197.md) | [@esrhengwu](https://x.com/esrhengwu) | — | — | [X](https://x.com/esrhengwu/status/2106285591465955449) | [视频](https://video.twimg.com/amplify_video/2106285066544730112/vid/avc1/720x1280/WokOBYdzEdyIADh1.mp4?tag=29) |
| MV198 | [女大怼脸撒娇自拍](prompts/one-liners/MV198.md) | [@loyu266934](https://x.com/loyu266934) | — | — | [X](https://x.com/loyu266934/status/2107376078893543543) | [视频](https://video.twimg.com/amplify_video/2107375576197775360/vid/avc1/720x1280/P_TmDahiDj2RnnES.mp4?tag=29) |
| MV199 | [推文配图一键转视频](prompts/one-liners/MV199.md) | [@jarvis11x](https://x.com/jarvis11x) | — | — | [X](https://x.com/jarvis11x/status/2108775744096604641) | [视频](https://video.twimg.com/amplify_video/2108772251633881088/vid/avc1/1080x1920/w0vyrZQP160sQ-ZV.mp4?tag=29) |
| MV200 | [宋词系列 60 秒](prompts/one-liners/MV200.md) | [@PixelAigc](https://x.com/PixelAigc) | 1 分钟 | — | [X](https://x.com/PixelAigc/status/2110023639806660635) | [视频](https://video.twimg.com/amplify_video/2110023452715565056/vid/avc1/1920x1080/47bPV2slVIHE5jNM.mp4?tag=29) |
| MV201 | [参考图生成 3 分钟先导片](prompts/one-liners/MV201.md) | [@jarvis11x](https://x.com/jarvis11x) | 3 分钟 | — | [X](https://x.com/jarvis11x/status/2113157755225669993) | [视频](https://video.twimg.com/amplify_video/2113155584228839424/vid/avc1/1280x720/wtKTL0D_Fg53NCh7.mp4?tag=29) |
| MV202 | [按抖音对标视频复刻 10 条](prompts/one-liners/MV202.md) | [@jarvis11x](https://x.com/jarvis11x) | — | — | [X](https://x.com/jarvis11x/status/2115247017999958150) | [视频](https://video.twimg.com/amplify_video/2115246948508712960/vid/avc1/1280x720/ub4t8lmG3bXLQSE7.mp4?tag=29) |
| MV203 | [宋代女子清晨劳作](prompts/one-liners/MV203.md) | [@PixelAigc](https://x.com/PixelAigc) | 10 秒 | — | [X](https://x.com/PixelAigc/status/2115605465040367620) | [视频](https://video.twimg.com/amplify_video/2115605255073542144/vid/avc1/1280x720/EoYtMJoYClQ9hl69.mp4?tag=29) |
| MV204 | [前所未有的摩托车（英文）](prompts/one-liners/MV204.md) | [@Preda2005](https://x.com/Preda2005) | — | — | [X](https://x.com/Preda2005/status/2117725540727861333) | [视频](https://video.twimg.com/amplify_video/2117725508733640704/vid/avc1/1660x720/nQkuMttknQaHFKQy.mp4?tag=29) |

## 用 API 跑这些提示词

这些提示词都是作者在 Meta 的 Muse 应用里跑的。[apimodels.app 上的 Muse Video](https://apimodels.app/zh/models/muse-video)（模型名 `muse-video`，[API 文档](https://apimodels.app/zh/docs/muse-video)）能做的事更少，有些提示词要改过才能用：

- 只有 720p，只有横屏 16:9（1280×720）或竖屏 9:16（720×1280）。
- 每次请求 4 到 20 秒。写给 30 秒或 1 分钟的提示词，要拆成几次请求再剪到一起。
- 提示词最长 4000 字。这里有 8 条超过了，要删短或按段拆开。
- 图片：要么 1 张首帧（视频从这张图开始），要么 1 到 4 张参考图（保持人物或主体，但不从参考图开始），两者不能同时用。参考图模板那种拼图，按参考图传。
- 让 Muse 打开链接、读帖子、每天定时做的指令，只能在 Muse 应用里用。
- 按请求秒数计费，每秒 $0.037：4 秒 $0.148，10 秒 $0.37，20 秒 $0.74。10 秒以内的片子一般 1 到 2 分钟出来。不保证每次都成功，失败的任务不扣费。

```bash
curl -X POST https://api.apimodels.app/v1/video/generations \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "muse-video",
    "prompt": "<one prompt from this collection, up to 4,000 characters>",
    "duration": 10,
    "aspect_ratio": "9:16"
  }'
# 10 秒：$0.37。返回里有 taskId，轮询到 state 为 "completed"：
curl "https://api.apimodels.app/v1/video/generations?task_id=TASK_ID" \
  -H "Authorization: Bearer YOUR_API_KEY"
```

参考图模板的提示词，再加一个 `"images": ["https://example.com/reference-sheet.jpg"]`（1 到 4 张）；要首帧就改传 `"image_url"`。两者不能同时传。

## 怎么收集的

用中文、英文、日文在 X 上搜 Muse Video 提示词相关的帖子，再把常发这类帖子的作者主页逐条看完。每条帖子都连同回复一起打开，因为很多作者把提示词放在第一条回复里。只收作者说明是用 Muse 做的、而且帖子里有提示词本身的。方法帖、心得、图片提示词，以及写给其他模型（Seedance、Grok、Veo、Gemini Omni 等）的提示词都没收。每一条都是原帖（或作者在原帖下自己的回复）里的全文。MV205 是 2026-11-20 第二轮补进来的，这一轮同时去掉了推广、色情内容、涉及未成年人的内容和真人肖像。时长、画幅和要不要参考图，都是从提示词原文里读出来的，「—」表示原文没写。标题是我们起的，每页另附英文标题。

## 出处、版权与许可

- **每条提示词的版权归作者**，视频和图片也归各自的作者。每条都写明作者、附原帖链接，媒体只链接到它原本所在的地方，没有任何文件拷进本仓库。
- **全文收录**：每条提示词都按原帖或原页面逐字全文收录。商用前请先看原帖。
- **我们自己写的内容**（写法说明、标题、分类表、数据文件和浏览页）按 [CC BY 4.0](LICENSE) 许可，引用请注明 apimodels.app 并附链接。
- 如果你是其中某条提示词的作者，想删除或更正署名，请开一个 issue，我们会尽快处理。
