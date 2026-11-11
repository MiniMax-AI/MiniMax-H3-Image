<div align="center">
  <img width="100%" src="assets/minimax-h3-image.jpg" alt="MiniMax H3 Image，开放权重">
</div>

<p align="center">
  <a href="https://hailuoai.video" target="_blank"><img src="https://img.shields.io/badge/Hailuo%20AI-FF6C37?logo=minimax&logoColor=white" alt="Hailuo AI"></a>
  <a href="https://platform.minimax.io" target="_blank"><img src="https://img.shields.io/badge/API-FF6C37?logo=minimax&logoColor=white" alt="API"></a>
  <a href="https://www.minimax.io" target="_blank"><img src="https://img.shields.io/badge/MiniMax%20Website-FF6C37?logo=minimax&logoColor=white" alt="MiniMax Website"></a>
  <a href="https://github.com/MiniMax-AI/MiniMax-H3-Image" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white" alt="GitHub"></a>
  <a href="https://huggingface.co/MiniMaxAI/MiniMax-H3-Image" target="_blank"><img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?logo=huggingface&logoColor=black" alt="Hugging Face"></a>
  <br>
  <a href="https://modelscope.cn/models/MiniMax/MiniMax-H3-Image" target="_blank" rel="noopener noreferrer"><img alt="ModelScope MiniMax AI" src="https://img.shields.io/badge/ModelScope-MiniMax%20AI-white?labelColor=%23EF3D5D"></a>
  <a href="https://platform.minimax.cn/docs/faq/contact-us" target="_blank"><img src="https://img.shields.io/badge/WeChat-07C160?logo=wechat&logoColor=white" alt="WeChat"></a>
  <a href="https://discord.com/invite/dbMxutw7tP" target="_blank"><img src="https://img.shields.io/badge/Discord-5865F2?logo=discord&logoColor=white" alt="Discord"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/LICENSE-4CAF50?logo=creativecommons&logoColor=white" alt="LICENSE"></a>
</p>

<p align="center">
  <a href="README.md">English</a> |
  <a href="README.zh-CN.md"><strong>简体中文</strong></a> |
  <a href="README.ko.md">한국어</a> |
  <a href="README.ja.md">日本語</a>
</p>

# MiniMax-H3-Image

## 提示词编写技能

MiniMax-H3-Image 在输入详细描述整张图像的英文文字时效果最好。`h3-image-prompt-writing` 技能可以让你自己的智能体根据一个简短的想法、一份需求说明、一条已有的提示词或一组参考图，写出这样的描述。使用 [skills CLI](https://github.com/vercel-labs/skills) 安装：

```bash
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --skill h3-image-prompt-writing
```

该技能在 [`skills/h3-image-prompt-writing/references/`](skills/h3-image-prompt-writing/references/) 下提供两份提示词指南：[`t2i-en.txt`](skills/h3-image-prompt-writing/references/t2i-en.txt) 用于文生图，[`edit-en.txt`](skills/h3-image-prompt-writing/references/edit-en.txt) 用于基于一张或多张参考图的图像编辑。

**智能体兼容性**：`h3-image-prompt-writing` 是一个纯 Markdown + 参考文件技能，不调用任何外部 API，因此可在 Claude Code、Claude Agent SDK、Cursor、Windsurf、基于 OpenAI 的智能体/Codex、LangChain，以及任何能够读取 `SKILL.md` 和本地文件的运行环境中使用。内置的 `skills/h3-image-prompt-writing/agents/openai.yaml` 只为 ChatGPT/Codex 的技能界面提供可选的界面元数据（显示名称、描述、默认提示词），并不会把该技能限制为仅适用于 OpenAI 智能体。

该技能只写提示词，不生成图像。把它的输出作为 `prompt` 传给你自己的部署即可（参见[本地运行](#本地运行)）。如果调用 MiniMax 文生图 API，还要设置 `disable_prompt_enhanced: true`，并传入技能给出的 `aspect_ratio`，否则 API 会把提示词再扩写一遍；图像编辑请求总会被扩写。如果想手写提示词，请参阅[提示词技巧](#提示词技巧)。所有技能的说明见 [`skills/README.md`](skills/README.md)。

## 在线使用

无需部署，可以直接在 MiniMax 应用里使用 MiniMax-H3-Image，也可以通过 MiniMax API 调用。

### 应用

- WebApp Global: [hailuoai.video](https://hailuoai.video/) | CN: [hailuoai.com](https://hailuoai.com/)
- Desktop Global: [agent.minimax.io](https://agent.minimax.io/) | CN: [agent.minimax.cn](https://agent.minimax.cn)

### API

- Global: [platform.minimax.io](https://platform.minimax.io/docs/guides/image-generation) | CN: [platform.minimax.cn](https://platform.minimax.cn/docs/guides/image-generation)

API 文档：
- 文生图：[EN-docs](https://platform.minimax.io/docs/api-reference/image-generation-h3-generations)，[CN-docs](https://platform.minimax.cn/docs/api-reference/image-generation-h3-generations)
- 图像编辑：[EN-docs](https://platform.minimax.io/docs/api-reference/image-generation-h3-edits)，[CN-docs](https://platform.minimax.cn/docs/api-reference/image-generation-h3-edits)
- 提示词扩写：[EN-docs](https://platform.minimax.io/docs/api-reference/image-generation-h3-context-ir)，[CN-docs](https://platform.minimax.cn/docs/api-reference/image-generation-h3-context-ir)

## 概览

MiniMax-H3-Image 是 [MiniMax H3](https://huggingface.co/MiniMaxAI/MiniMax-H3) 系列的开源 SOTA 图像生成与编辑模型，兼具高智能创作理解与视觉世界构建能力。模型以精准的指令遵循能力，将创意概念展开为具体的角色、场景与视觉氛围，集生成与编辑于一体，为创作者和开发者提供灵活、可控的出色图像创作体验。

它在各种宽高比下都能直接生成约 1600 万像素的图像，从 4096x4096（1:1）到 6272x2688（21:9），无需借助超分模型（参见[尺寸](#尺寸)）。该 checkpoint 经过蒸馏，只需 6 个采样步（6 次 NFE），且不使用 classifier-free guidance。它的扩散 Transformer（DiT）采用 H3 架构，但去掉了音频层；文本编码器直接沿用 MiniMax-H3 的文本编码器，未做改动。

![十五张 MiniMax-H3-Image 文生图结果，有横版也有竖版：3D 奇幻战斗场面、青绿山水画、树蛙、蓝染兔子、3D 白发女孩、花丛中的人像、科幻城市、饺子、高地牛、镜中人像、3D 水獭和绵羊、像素风猫咪、吉丁虫、巨型樱桃和鱼眼自拍](assets/showcase_hero.jpg)

### 亮点

MiniMax-H3-Image 兼具三项核心优势：速度、画质和指令遵循。

1. **以实用的计算成本生成 1600 万像素图像**。与目前常见的 100 万到 400 万像素输出相比，1600 万像素（4096 × 4096）的图像细节要丰富得多，但通常也需要多得多的计算量。MiniMax-H3-Image 把这部分计算成本控制在可承受的范围内，让 1600 万像素生成可以用于日常创作。
2. **细节丰富，真实感出众**。MiniMax-H3-Image 摆脱了常见的“AI 感”，生成的图像细节精细、真实逼真，为创意和专业用途带来更多可能。它让生成的图像更接近真实视觉世界的丰富与细腻。
3. **指令遵循更强**，创作更可控。出色的图像生成不只是画面好看，更要帮助创作者把想法变成作品。MiniMax-H3-Image 的指令遵循能力在开源模型中最强，最多支持 16 张参考图，让创作者能更好地掌控最终效果。

### 模型列表

| 模型 | 用途 | 精度 | 大小 | Hugging Face |
| --- | --- | --- | --- | --- |
| **MiniMax-H3-Image** | 文生图和图像编辑 | BF16 (DiT) | 68.65 GB | [MiniMaxAI/MiniMax-H3-Image](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image) |
| **MiniMax-H3-Image-PE**（可选） | 文生图提示词扩写模型 | NVFP4 | 17.9 GB | [MiniMaxAI/MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE) |

### 模型架构

MiniMax-H3-Image 沿用 H3-Base 的设计，但去掉了音频分支。文本提示词和参考图由 H3 文本编码器编码；参考图还会经过图像 VAE 编码。所有 token 组成一个打包序列，输入单流 Transformer，由它预测目标图像的 latent。VAE 再把这个 latent 解码成图像。

- **文本编码器**：MiniMax-H3 的完整 Qwen3-VL 文本编码器，未做改动。DiT 读取它第 50 层的隐藏状态。
- **图像 VAE**：一个 CNN 编码器加一个 2D ViT 解码器（24 层），空间下采样 16 倍，latent 通道数为 24。DiT 以 2x2 的 patch 对 latent 做 patchify，因此每个 Transformer token 覆盖 32x32 像素。
- **扩散 Transformer**：33.1B 参数的稠密单流 Transformer，共 50 层（隐藏维度 5376，56 个注意力头，FFN 维度 14336），使用 3D 多模态 RoPE，与 H3-Omni-Transformer 相同。权重为 BF16；embedding 层、timestep 层和输出层为 FP32。

## 效果展示

以下是文生图和图像编辑的结果，图片经过缩小。展开图片下方的**提示词**，可以看到当时输入的内容。这些是用户直接写下的需求，不是模型实际收到的扩写后提示词：MiniMax API 会在生成前用 H3-Image-Context-IR 扩写它们（文生图默认扩写，图像编辑总是扩写），所以可以原样发送。如果是本地部署，请先按[完整工作流](#完整工作流)中的方法扩写。这里展示的都是原始提示词，大多用中文写成，少数原本用英文写成，保留原样。

### 文生图

<p align="center">
<img src="assets/showcase/photo.jpg" alt="三张写实照片：黄昏的满月下，一个穿白衬衫的人在屋顶上收晾衣绳上的白床单；一位卷发年轻男子捧着深色杯子喝茶的侧脸特写；几只火烈鸟在浅水中行走" width="100%"/>
</p>
<p align="center"><em>写实摄影</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<p><b>黄昏屋顶</b></p>
<blockquote>夏末黄昏的旧城市屋顶，几根晾衣绳横跨前景，白床单被风吹起形成柔软的波浪，床单间隙露出远处密集的屋顶、天线和一轮低悬的淡金色月亮；逆光中一位穿白衬衫的人站在右侧收衣服，只保留清晰的侧面轮廓，屋顶水泥表面有暖灰纹理和浅浅积水，天空从玫瑰粉过渡到烟紫，夕阳边缘光穿过织物，画面有生活纪录片的真实和电影静帧的构图诗意，35mm镜头、自然风、轻微胶片颗粒，不要浪漫滤镜过重。<br>
真实摄影与电影静帧质感，优先自然光和可信的物理反射，构图有明确视觉重心与呼吸空间，色彩克制但有一到两个叙事性点色，材质细腻真实，人物动作自然，保留适度35mm胶片颗粒、柔和高光晕染和真实景深；画面高级、耐看、具有叙事瞬间，不要廉价CG感，不要塑料皮肤，不要过度锐化，不要HDR光晕，不要随机添加物件，不要水印、边框、logo或多余文字。</blockquote>

<p><b>喝茶前的停顿</b></p>
<blockquote>拍摄一位卷发人物喝茶前停顿的真实肖像，头部、肩膀、上胸和双手捧着的深色陶杯入镜，人物略微侧脸。画面右后方的暖色灯光掠过头发，背景是较暗的室内墙面。松散卷发外缘和几根翘起的碎发被照得透亮，发丝之间仍能看见暗背景；浓密发束的内部保持深色，亮边随着发束遮挡自然中断。脸部由相机左前方很弱的柔光照亮，能看清眼睛、面颊和手指。耳廓与肩部只在朝向后侧灯光的边缘受光，陶杯呈宽而弱的表面亮部，杯沿和手指交接处保留接触阴影。焦点覆盖眼睛、外缘发丝与杯口。</blockquote>

<p><b>清晨火烈鸟</b></p>
<blockquote>清晨盐湖浅水区，五只火烈鸟分散在宽阔的镜面水面上，最前景一只低头觅食，第二只单腿站立，远处三只形成柔和的粉色节奏，湖面倒映淡粉天空和远处白色盐壳；采用长焦平视构图，水面几乎占据整个画面，鸟群之间留出足够呼吸空间，羽毛粉色从灰粉到珊瑚粉有细腻层次，水纹、倒影、盐壳和鸟腿真实，优雅自然摄影，不要拥挤鸟群，不要高饱和卡通色。<br>
真实摄影与电影静帧质感，优先自然光和可信的物理反射，构图有明确视觉重心与呼吸空间，色彩克制但有一到两个叙事性点色，材质细腻真实，人物动作自然，保留适度35mm胶片颗粒、柔和高光晕染和真实景深；画面高级、耐看、具有叙事瞬间，不要廉价CG感，不要塑料皮肤，不要过度锐化，不要HDR光晕，不要随机添加物件，不要水印、边框、logo或多余文字。</blockquote>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/surreal.jpg" alt="三张超现实时尚大片：理发师为坐在理发椅上的一朵云修剪造型；夜晚的草地上有人在切月亮；一位模特从一只巨大的梨中走出" width="100%"/>
</p>
<p align="center"><em>超现实时尚大片</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<p><b>理发椅上的云</b></p>
<blockquote>一张复古、俏皮又高级的超现实时尚摄影。鲜绿色的山丘上摆着一张樱桃红色理发椅，一团巨大的白云坐在椅子里，蓬松的云体被薄荷绿色理发围布围住。一位成年女模特穿淡紫色短袖衬衫、深紫色铅笔裙和白色长靴，站在椅子旁，认真地用一把银色剪刀修剪白云，另一只手托起云朵的一角。剪下的小团云絮散落在草坪上，像刚剪落的头发。模特留利落的复古短发，神情专注。低机位广角构图，蓝天占据大半画面，布景简洁而色彩鲜明。真人时装大片质感，云朵有柔软半透明的细节与可信的体积阴影，轻微直闪补光，胶片颗粒，无卡通感。横向16:9，无文字。</blockquote>

<p><b>切月亮</b></p>
<blockquote>一张具有复古电影布景质感的超现实时尚摄影。钴蓝色暮光天空下，绿色山丘上摆着一张铺白色桌布的长餐桌。一位成年女模特穿番茄红色丝绒长裙和白色长手套，神情冷静地站在桌子一侧，用银色餐刀从餐盘里的巨大满月上切下一小块楔形月亮。满月如圆形蛋糕般立在盘中，表面保留真实的陨石坑，切口内部散发柔和的乳白色光芒，切下的月亮块稳稳落在旁边的小瓷盘上。月光照亮她的手套与下颌，桌上玻璃杯投下细长阴影。空中的天空没有第二个月亮，远处只有一棵孤独的小树。优雅、荒诞、略带冷幽默，真实人物和实体道具摄影质感，细腻胶片颗粒，横向16:9，无文字。</blockquote>

<p><b>梨子更衣室</b></p>
<blockquote>一张2000年代先锋时尚杂志的超现实摄影。浅粉色摄影棚里，一颗三米高的黄绿色梨子被改造成更衣室，梨皮上开出一道圆角小门，门板仍保留厚实的果皮与乳白色果肉切面。一位成年女模特正从梨子里迈出一只脚，穿巧克力棕色缎面连衣裙、浅蓝色连裤袜与尖头鞋，一只手扶着门边，另一只手整理耳环，表情漫不经心。梨子内部铺着酒红色丝绒软垫，挂着两件精致衣服。旁边一把小巧的银色椅子上放着普通大小的梨，形成明确的尺度对照。构图偏心，留出干净空间，柔和棚灯配合轻微正面闪光。果皮毛孔、水分充足的果肉、丝绒与缎面均有可触摸的真实质感，精心搭建的实体布景观感。横向16:9，无文字。</blockquote>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/scene.jpg" alt="四张场景概念图：森林中一座古代露天剧场的遗迹，标题为 ENVIRONMENT CONCEPT: THE ANCIENT THEATER；红色岩石悬崖上的驭龙者；挂着 ARRIVALS 指示牌的废弃火车站；冰封海面上的沉船" width="100%"/>
</p>
<p align="center"><em>场景概念图</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<p><b>森林中的古剧场（左上）</b></p>
<blockquote>画面比例16:9，4K。做一张面向3A游戏的环境概念成图，先读出地形、地标和聚落用途，再看到细节。采用可信写实3D空间，建筑顺应气候与地势，保留前中后景。具体内容：被森林吞没的圆形剧场，树根沿裂缝进入座席。不使用现有作品的名称、角色或品牌标志，不添加水印。</blockquote>

<p><b>废弃车站（左下）</b></p>
<blockquote>Aspect ratio 16:9, 4K. Generate a photorealistic AAA image with a high-end real-time engine look. Emphasize indirect illumination, varied roughness, contact shadows and depth separation. Show only the rendered scene, without an editor or performance counters. Scene: Sunlight enters an abandoned station through a glass roof and reflects its steel frame in wet tiles. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

<p><b>冰封沉船（右下）</b></p>
<blockquote>极寒冰封海湾中的废弃船舶遗址，2.2:1超宽全景，24mm广角微俯视。左侧倾斜船骸覆满积雪与冰柱，锈蚀集装箱散落甲板。中央碎冰裂隙延伸至蓝水道，青绿冰壁透光，浮冰与残片漂流。右侧白灰拖船搁浅，远处红色货轮倾覆于冰川之间。背景雪山、冰崖与稀疏针叶林隐入寒雾。冰蓝青灰主调，暗红船体点缀，冷冽日光形成近暗远亮层次，寂静荒凉。电影级写实，真实冰雪金属材质与水面反射，深景深、体积雾、8K，无人、无字、无水印。</blockquote>

<p><em>右上角驭龙者的提示词未收录。</em></p>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/char.jpg" alt="角色、生物与道具：戴装甲头盔的战斗驾驶员；森林中长着红色鳍的龙；红色荒原上一顶落满灰尘的宇航员头盔；一张极地服装设定板，含正面、背面和局部特写" width="100%"/>
</p>
<p align="center"><em>角色、生物与道具</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<p><b>战斗驾驶员</b></p>
<blockquote>画幅比例 1:1。写实未来战斗驾驶员的近距离半身肖像，年轻男性脸部冷峻、眼睛微向右看，面颊有细小擦伤，头发藏在复杂的开放式装甲头盔内。头盔为橄榄绿与旧白色工业壳体，顶部有红白斜纹徽记，面部两侧排列传感器、黑色光学镜头、通讯盒和铰接支架，下颌装有护颈框架。白灰色胸甲厚重，有深色胸带、软管、编号“003”、贴纸和细小警示标记，表面有划痕、积尘和边缘掉漆。主体靠近镜头，纯黑背景，冷色左上软光勾勒脸部与设备轮廓，强调复杂机械装配、皮肤真实感和军用硬表面材质。 输出单张完整作品画面，不添加网站边框、作者署名或水印。</blockquote>

<p><b>森林中的龙</b></p>
<blockquote>写实幻想电影生物立于幽暗森林的岩石上，正方形全身构图。主体是一只高颈、细长身体的龙，灰蓝与墨绿色细鳞皮肤，腹部偏米灰色，背部从肩膀到尾部竖起扇形暗红色鳍膜；头部张嘴嘶吼，额头与脸颊生出许多向后飘卷的粉红色长须和角状肉质冠，须丝形成优雅复杂的轮廓。四肢为有锐爪的爬行动物结构，长尾绕身体向左弯曲，脚踩湿润石块和苔藓。森林柔和自然光穿透部分须冠，材质细腻可信，无文字或水印。</blockquote>

<p><b>红色荒原上的宇航员头盔</b></p>
<blockquote>画面比例3:4，4K。绘制原创3A游戏的竖版封面主视觉，写实3D、强烈而克制的电影光影。让单一主角或核心物占据明确焦点，顶部约四分之一保持安静用于后续排字，当前图不生成标题、标志或文字。具体内容：蒙尘宇航头盔躺在红色荒原上，镜面反射远处基地。不使用现有作品的名称、角色或品牌标志，不添加水印。</blockquote>

<p><b>极地服装设定板</b></p>
<blockquote>Aspect ratio 3:2, 4K. Create an original AAA costume board: full front view on the left, full rear view in the center and one construction close-up on the right, using the same adult model and outfit. Show realistic 3D drape, seams and fastening structures against pale gray without text. Scene: An insulated polar communicator outfit with fur collar, sealed cuffs and gaiters. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/art.jpg" alt="四幅绘画与插画：古典大师油画风格的荷叶间鸳鸯；印象派油画风格的晨雾苏州园林；中世纪泥金手抄本风格的 XVIII THE MOON 页面，玉兔在石臼里捣月亮；一幅中国工笔画，画中鹈鹕照着镜子，配有四个书法字" width="100%"/>
</p>
<p align="center"><em>绘画与插画风格</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<p><b>鸳鸯，古典大师油画</b></p>
<blockquote>一幅17世纪欧洲古典大师风格的布面油画，题材是中国的鸳鸯与荷塘。画面中央，一对鸳鸯在幽暗的荷塘水面上相依而游：雄鸳鸯羽色华丽，橙红色帆状饰羽、带紫绿金属光泽的头冠、白色眉纹、红色的喙；雌鸳鸯灰褐素雅，眼后一道白纹。两只鸳鸯头颈微微相靠，神态安静深情。四周是夏末初秋的荷叶，有的饱满墨绿，有的边缘焦枯卷曲，右上方一枝半开的粉白荷花和一个低垂的莲蓬。伦勃朗式明暗对照光，一束温暖的侧光从左上方落在鸳鸯身上，其余部分沉入深橄榄绿与琥珀棕的暗部。水面像一面墨色的镜子，倒映着鸳鸯与荷花，泛起细小的涟漪。厚涂与薄罩染结合，羽毛高光处颜料堆起，能看到清晰的笔触和画布纹理，古旧清漆带来温暖的金色调和细微的龟裂。构图稳重，留有大片暗部的呼吸空间，诗意、静谧，博物馆级杰作。</blockquote>

<p><b>苏州园林，印象派油画</b></p>
<blockquote>一幅法国印象派布面油画的实物，竖幅构图，题材是苏州古典园林晨雾中的鸳鸯戏水，就像莫奈晚年在苏州园林的池塘边，用浓稠的油彩和粗猪鬃笔对着清晨的雾写生而成。气息接近《日出·印象》《睡莲》和《鲁昂大教堂》晨雾系列的原作：物象溶解在光和雾里，但整幅画每一寸都是看得见的笔触和颜料。这是西方油画，没有水墨，没有工笔线条，没有题字和印章。<br>
<br>
【画面内容】<br>
水面占画面下方约六成。中下部偏左，一对鸳鸯相向嬉戏，只用几笔概括，雄鸟那几笔厚重的橙红色是全画唯一温暖浓郁的一点，像《日出·印象》里的红日；雌鸟是一抹柔和的灰褐。周围松散地浮着粉色和蓝绿色的睡莲、荷叶色块。<br>
中景右侧，九曲石桥和岸边的太湖石化成几抹淡紫灰。<br>
远处（画面上方约四成），一道白粉墙、一扇圆形月洞门和一座飞檐高翘的亭子，在雾中融化成淡薰衣草色和奶油色的幽影，只隐约辨认出墙头的起伏、飞檐的弧线和一个淡淡的圆。左上方垂柳化成下垂的绿紫色笔触，右上方花树是粉色的笔触团块。所有建筑的倒影都在水面上溶解、颤动。<br>
<br>
【朦胧感】<br>
浓厚湿润的晨雾充满整个画面，空气本身是粉紫、淡金和灰蓝交融的光。没有轮廓线，水面、空气和远岸几乎没有分界，形体只靠色温的微弱差异浮现。整体高调柔和，色彩处在相近的明度上，阴影里只有淡紫和淡蓝，不用黑色。<br>
<br>
【笔触，最重要】<br>
朦胧完全来自相近明度的笔触彼此交错，绝不来自模糊。画面上没有任何柔焦、喷枪式渐变、光滑的过渡或数码模糊，雾气本身也是由一笔一笔可数的颜料构成的。<br>
全画布满清晰可见、奔放、大小不一的笔触：逗号状、短划状、断续的笔痕，宽约一指，每一笔都能看出起笔、收笔和猪鬃刷留下的细沟纹。<br>
笔触方向随物象变化：水面是横向短笔层层铺开；倒影是竖向颤动的笔触；垂柳是下垂的弧形长笔，飞快扫过；天空和雾气是斜向交错、松散编织的笔触；鸳鸯周围是环绕的弧形短笔，如涟漪般打开。<br>
颜料有真实的厚度：受光处、睡莲和雄鸳鸯的橙红处是明显的厚涂，颜料堆起，边缘带小脊，在侧光下呈浮雕感；较暗处干笔擦过，露出下层颜色和粗麻画布的织纹。<br>
笔触之间是未经调和的纯色并置：粉紫旁边是淡金，灰蓝旁边是淡玫瑰，湿画叠湿画，局部被下一笔拖带混合，但绝不抹平。<br>
<br>
近看全是奔放的笔触和颜料，退远看才聚拢成雾中园林。博物馆级印象派杰作，奥赛博物馆的藏品质感。</blockquote>

<p><b>玉兔，中世纪泥金手抄本</b></p>
<blockquote>A medieval illuminated manuscript illustration with gold leaf and a wide border of curling vines. Beneath an old osmanthus tree, the Jade Rabbit of Chinese folklore stands beside a blue-grey stone mortar. Wearing a simple red cloth sash, it grips a long jade pestle and carefully grinds a single ivory crescent moon into fine golden powder. Part of the crescent remains intact inside the mortar. Small osmanthus blossoms fall onto the stone rim, and several folded medicine packets lie nearby. The rabbit works with the solemn concentration of an old apothecary. The deep blue sky contains a few stars but no second moon.<br>
Flat perspective, dark ink outlines, opaque tempera on aged parchment. Rich red, ultramarine blue and antique gold. A broad blue border filled with curling gold lotus vines, small blossoms and Chinese cloud motifs. Worn gold leaf and slightly irregular hand-painted forms. A small numeral XVIII above, and THE MOON in a parchment cartouche below.</blockquote>

<p><b>照镜子的鹈鹕，工笔画</b></p>
<blockquote>中国工笔画风格，绢本设色。古代闺房的梳妆台上立着一面圆形铜镜，一只白色鹈鹕站在镜前，低头用长嘴整理胸前的羽毛。铜镜表面偏黄、有点模糊，映出鹈鹕的正脸和它身后的雕花木窗。左上角有竖排题字和一枚红色印章。</blockquote>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/text.jpg" alt="两块逻辑推理题板：一块是中文的候选人选拔题，列出五个条件和推出的答案；另一块是英文题板，标题为 CONFIDENTIAL FILE MISSING，有六名嫌疑人、真假印章和一张核对表" width="100%"/>
</p>
<p align="center"><em>带推理的文字渲染：中英文逻辑题，在题板上正确解出</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<p><b>人员选派推理题（左）</b></p>
<blockquote>请解答下面的人员选派推理题，并生成一张可视化解答图。16:9 横向，白底，规范清晰的中文排版。<br>
某单位要从甲、乙、丙、丁、戊、己六名工作人员中，恰好选派三人组成调研组，必须同时满足：<br>
如果甲入选，那么乙也必须入选。<br>
丙、丁两人中恰好有一人入选。<br>
乙和戊不能同时入选。<br>
如果己入选，那么丙也必须入选。<br>
已确定戊入选。<br>
请根据全部条件确定三人名单。<br>
图中上方呈现题目条件，下方分成“入选”和“未入选”两个区域，将六张工作人员卡片分别放入正确区域。每张卡片用人物图标和醒目的姓名标签表示，六人各出现一次，不得重复或遗漏。<br>
底部用简短批注展示关键排除依据。卡片所在区域、名单与批注必须一致，不得增加额外条件。仅输出完成后的解答图片。</blockquote>

<p><em>右侧侦探推理板的提示词未收录。</em></p>

</details>
<!-- END showcase-prompts -->

### 图像编辑

<p align="center">
<img src="assets/showcase/edit_render.jpg" alt="左：月球基地的无纹理灰色 3D 渲染图，有居住舱、月球车和一名宇航员。右：同一场景变成月面上的写实电影剧照" width="100%"/>
</p>
<p align="center"><em>图像编辑，一张参考图：无纹理 3D 渲染图（左）变成月球科研基地的电影剧照（右）</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<blockquote>把这张白模渲染成真实月面科考电影画面。补全灰色月壤、银白隔热层、涂层金属、玻璃与轮网材质，宇航服为米白色。使用强方向性太阳光和有限地面反射，远处天空纯黑，不加蓝天、云或地球式雾气。保持探测车六个车轮、人物和舱段布局，阴影方向统一，亮部保留材质细节。 保留原图构图、镜头角度、透视、几何结构与各主体的位置和比例；输出4K、16:9横版，呈现3A级写实CG与电影实拍融合的质感，不添加文字、品牌、界面或水印。</blockquote>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/edit_map.jpg" alt="左：插画风格的游戏地图，有河流、瀑布、桥梁、城堡、村庄、矿场和港口，南边湖面上有一个红色箭头。右：从湖面望向瀑布、吊桥、矿场和远处城堡的第一人称 3D 游戏画面，左上角是作为小地图的原地图" width="100%"/>
</p>
<p align="center"><em>图像编辑，一张参考图：游戏地图（左）变成从红色箭头位置看出去的第一人称 3D 游戏画面，原地图作为小地图（右）</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<blockquote>以提供的游戏地图为唯一空间依据，生成一张 16:9、写实 3D CG 风格的开放世界游戏实机画面。<br>
相机位置与朝向<br>
将红色箭头的尾端作为相机位置，箭头尖端所指方向作为镜头朝向。相机位于地图南部湖面上方约 1.7 米，以第一人称视角向北偏东看去，视野约 70°，保持自然透视。画面不出现玩家身体。<br>
空间还原<br>
严格按照地图还原地形高差、建筑位置、河流走向、桥梁连接和道路关系。<br>
根据真实视线决定两岸聚落、矿区、山体和远处城堡的可见范围。保留合理遮挡与远近比例，不要为了展示所有地标而移动建筑、拉平地形或扩大视野。<br>
画面风格<br>
高品质写实游戏引擎渲染，真实尺度的建筑与山体，细致的岩石、木材、植被和水面材质，自然日光、全局光照、水面反射与适度空气透视。呈现玩家真正置身于这个世界中的感觉。避免手绘地图质感、微缩沙盘、等距视角和鸟瞰构图。<br>
左上角小地图<br>
在画面左上角加入清晰的游戏 HUD 小地图，宽度约占画面的 15%。使用参考图的地表地图作为缩略底图，保持原始比例与北向朝上，保留主要地形和道路，去掉地下层插图。<br>
小地图上以一个小型方向箭头标出玩家位置，位置对应原图红色箭头的尾端，朝向与主画面镜头完全一致，并用淡色扇形表示视野范围。采用简洁细边框，保持地图清楚可读。<br>
最终只输出一张完整游戏画面。主场景中不要出现原图的红色箭头、地名标签、海拔数字或地图边框；除左上角小地图外，不添加其他界面元素。</blockquote>

</details>
<!-- END showcase-prompts -->

<p align="center">
<img src="assets/showcase/edit_multi.jpg" alt="上：十张参考图，一间洒满阳光的空房间和九件家具。下：空房间摆上这九件家具后成了一间客厅" width="100%"/>
</p>
<p align="center"><em>图像编辑，十张参考图：一间空房间和九件家具（上）组合成一间客厅（下）</em></p>

<!-- BEGIN showcase-prompts -->
<details>
<summary>提示词</summary>

<blockquote>为「向阳家居」拍一张春季家具目录的客厅氛围图。第一张是空房实景，后面九张是本期在售家具白底图。沿用空房的机位、墙面、门窗和木地板，把九件原款家具各摆入一次，布置成一间平时可以两三个人聊天、也可以靠窗读写的客厅。皮带扶手休闲椅是主推款，给它一个看得清木框、皮带扶手和坐垫的角度。其他家具按真实尺寸和用途安排，坐下能用到桌面，书椅能拉开，从门口进屋有连续的通道。<br>
保留每件商品的颜色、材质、结构和比例，让右侧窗光自然落在布面、皮革和木头上，桌腿椅脚有可信的接触阴影。允许少量书或一枝绿植，保持陈列清爽。室内实景摄影，不加文字。</blockquote>

</details>
<!-- END showcase-prompts -->

## 本地运行

要在自己的 GPU 上运行 MiniMax-H3-Image，先下载权重，再用 SGLang 或 vLLM-Omni 启动服务，然后按下面的参数和尺寸发送请求。[完整工作流](#完整工作流)把这些步骤和提示词扩写串起来，在本地复现 MiniMax API 的出图效果。

### 模型文件

| 组件 | 内容 | 大小 |
| --- | --- | --- |
| `transformer/` | DiT：BF16，其中 embedding 层、timestep 层和输出层为 FP32。 | 66.28 GB |
| `pdd_fused_heads.safetensors`、`pdd_config.json` | 每个采样步专用的输出头（替代 Transformer 原有的输出层），以及采样调度。 | 12 MB |
| `vae/` | 图像 VAE，FP32。 | 2.34 GB |
| `tokenizer/`、`processor/` | Qwen3-VL 的 tokenizer 和 processor，与 MiniMax-H3 相同。 | 23 MB |
| 文本编码器 | 不包含在原始 checkpoint 中。`model_index.json` 会从 [`MiniMaxAI/MiniMax-H3`](https://huggingface.co/MiniMaxAI/MiniMax-H3) 的 `text_encoder/` 文件夹加载它。如果你已经有 MiniMax-H3，就不会再次下载。 | 66.7 GB |

```text
MiniMax-H3-Image/
├── model_index.json
├── pdd_config.json
├── pdd_fused_heads.safetensors
├── processor/
├── tokenizer/
├── transformer/
└── vae/
```

Hugging Face 仓库同时托管这份原始 checkpoint 和 diffusers 格式，总共约 204 GB，因此请按你的框架需求限定下载范围。SGLang 和 vLLM-Omni 加载原始 checkpoint 和 MiniMax-H3 文本编码器，两者合计约 135 GB：

```bash
# Original checkpoint (SGLang, vLLM-Omni)
hf download MiniMaxAI/MiniMax-H3-Image model_index.json "pdd_*" "processor/*" "tokenizer/*" "transformer/*" "vae/*"
hf download MiniMaxAI/MiniMax-H3 --include "text_encoder/*"
# optional prompt expander
hf download MiniMaxAI/MiniMax-H3-Image-PE
```

diffusers 用户无需手动下载：`ModularPipeline.from_pretrained("MiniMaxAI/MiniMax-H3-Image")` 会读取 `modular_model_index.json`，并拉取 diffusers 格式的文件夹（`transformer_diffusers/`、`vae_diffusers/`，以及本仓库自带的一份 `text_encoder/`）。加载和 offloading 的用法请参阅 [diffusers 文档](https://huggingface.co/docs/diffusers/main/en/api/pipelines/minimax_h3_image)。

### 部署

我们推荐使用以下推理框架部署模型：

- [SGLang](https://docs.sglang.io/)：参见 [cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3-Image)
- [vLLM-Omni](https://github.com/vllm-project/vllm-omni)：参见 [vllm-omni recipe](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image)
- [diffusers](https://github.com/huggingface/diffusers)：参见 [diffusers 文档](https://huggingface.co/docs/diffusers/main/en/api/pipelines/minimax_h3_image)
- [ComfyUI](https://github.com/Comfy-Org/ComfyUI)：参见 [Comfy 教程](https://docs.comfy.org/tutorials/image/minimax/minimax-h3-image)；使用 [T2I 模板](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/image_minimax_h3_image_t2i.json) / [Edit 模板](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/image_minimax_h3_image_edit.json)

#### SGLang

下面的[完整工作流](#完整工作流)使用 SGLang。从 main 分支安装 SGLang 及其扩散模型依赖（参见[扩散模型安装指南](https://docs.sglang.io/docs/sglang-diffusion/installation)）：

```bash
git clone https://github.com/sgl-project/sglang.git
cd sglang
python3 -m pip install -e 'python[diffusion]'
```

在单张 GPU 上启动服务：

```bash
sglang serve --model-path MiniMaxAI/MiniMax-H3-Image --host 0.0.0.0 --port 30000 --warmup-mode off
```

显存较小的 GPU 也用同一条命令：GPU 可用显存不足 130 GiB 时，SGLang 会自动卸载（offload）部分模型组件来适应显存。如果要使用本地的 MiniMax-H3 `text_encoder/` 文件夹，而不是 Hugging Face 缓存，请添加 `--text-encoder-path <path to text_encoder>`。

如需更低延迟，可以用序列并行（Ulysses）把每个请求拆到多张 GPU 上，例如使用 4 张 GPU：

```bash
sglang serve --model-path MiniMaxAI/MiniMax-H3-Image --host 0.0.0.0 --port 30000 --warmup-mode off \
  --num-gpus 4 --ulysses-degree 4
```

[SGLang cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3-Image) 按 GPU 类型给出了从 B300 到 24 GB 显卡的部署方案和实测延迟。

#### vLLM-Omni

安装 vLLM 0.33.0，并从源码安装 vLLM-Omni：

```bash
uv venv --python 3.12 --seed && source .venv/bin/activate
uv pip install vllm==0.33.0 --torch-backend=cu130
git clone https://github.com/vllm-project/vllm-omni.git && cd vllm-omni && uv pip install -e .
```

默认配置（在 H200 上实测）用序列并行（Ulysses）把每个请求拆到 4 张 GPU 上：

```bash
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 \
  --num-gpus 4 --usp 4 --text-encoder-tp-size 4
```

单张 GPU 要放下整个模型，约需 135 GiB 显存（B200、B300）：

```bash
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 --num-gpus 1
```

单张 H200 上，把文本编码器卸载出去：

```bash
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 --num-gpus 1 \
  --diffusion-offload-config '{"mode":"layer","components":["text_encoder"]}'
```

在 AMD Instinct MI325X 和 MI350X 上，使用 `vllm/vllm-omni:minimax-h3-image-rocm` 镜像，并在默认命令后加上 `--no-enable-cuda-graph-decode`。H100、RTX PRO 6000 等其他 GPU 的配置和实测延迟见 [vLLM-Omni recipe](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image)。

### 请求参数与尺寸

#### 请求参数

使用 SGLang 时，文生图请求以 JSON 格式发送到 `/v1/images/generations`。图像编辑请求以 multipart 表单数据的形式把参考图发送到 `/v1/images/edits`；参考图的顺序决定它们在提示词中分别对应 `<Picture 1>`、`<Picture 2>` 等。两种请求都在 `data[0].b64_json` 中返回 PNG。可运行的示例见[完整工作流](#完整工作流)。vLLM-Omni 使用的字段略有不同，例如 `min_generation_area` 要放在 `extra_args` 中；参见 [vLLM-Omni recipe](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image)。

| 字段 | 文生图 | 图像编辑 | 说明 |
| --- | --- | --- | --- |
| `prompt` | 必填 | 必填 | 按原样使用，超过 4096 个 token 的部分会被截断。参见[完整工作流](#完整工作流) |
| `size` | 必填 | 必填 | `WIDTHxHEIGHT`。返回图像的尺寸与它完全一致；参见[尺寸](#尺寸) |
| `image` | — | 一个或多个文件 | 按上传顺序，在提示词中依次对应 `<Picture 1>`、`<Picture 2>` 等 |
| `seed` | 推荐 | 推荐 | 整数 |
| `generator_device` | 推荐 `cpu` | 推荐 `cpu` | 相同的 seed 在任何机器上都得到相同的初始噪声 |
| `response_format` | `b64_json` | `b64_json` | |
| `min_generation_area` | 可选 | 可选 | 最小生成面积（像素），取值 1024-16777216，默认 4194304（2048x2048）。较小的 `size` 会先在同宽高比的更大画布上生成，再用 LANCZOS 缩放回原尺寸；传入 1024 可关闭这一行为。下表中的所有尺寸都大于默认值 |
| `num_inference_steps` | 不填或填 6 | 不填或填 6 | 其他值返回 HTTP 400 |
| `guidance_scale` | 不填或填 1 | 不填或填 1 | 其他值返回 HTTP 400 |
| `negative_prompt` | 不支持 | 不支持 | 会被拒绝 |

#### 尺寸

MiniMax-H3-Image 的有效工作范围约为 400 万到 2000 万像素，一般在 1600 万像素左右效果最好。常用的 1600 万像素尺寸如下：

| 宽高比 | 尺寸（宽 x 高） |
| --- | --- |
| 1:1 | 4096x4096 |
| 4:3 / 3:4 | 4736x3552 / 3552x4736 |
| 3:2 / 2:3 | 5024x3360 / 3360x5024 |
| 16:9 / 9:16 | 5472x3072 / 3072x5472 |
| 21:9 | 6272x2688 |

其他宽高比保持约 1600 万像素、宽高都取 32 的倍数即可。[`examples/context_ir.py`](examples/context_ir.py) 里的 `size_for()` 可以直接算出尺寸：

```bash
cd examples
python3 -c "from context_ir import size_for; print(size_for('5:4'))"   # 4576x3648
```

### 完整工作流

MiniMax-H3-Image 的输入应是一段详细描述整张图像的英文文字。MiniMax API 会在生成前用 **H3-Image-Context-IR** 把任意语言的简短提示词改写成这样的描述。我们还提供可在本地部署的 [MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE)。

本节介绍如何用本地部署的 SGLang 服务，复现直接通过 MiniMax API 生成的图像质量。脚本位于 [`examples/`](examples)，只依赖 Python 标准库；克隆本仓库后在该文件夹中运行：

```bash
git clone https://github.com/MiniMax-AI/MiniMax-H3-Image.git
cd MiniMax-H3-Image/examples
```

`t2i.py` 和 `edit.py` 会把请求发到上面启动的 SGLang 服务 `http://127.0.0.1:30000`；用 `--url` 可以换成其他地址。

运行示例之前，请先设置 MiniMax API 的地址和密钥，用于调用 H3-Image-Context-IR API 和运行 API 参考脚本。脚本会从环境变量中读取它们：

```bash
# MiniMax API endpoint (choose one)
# CN
export MINIMAX_API_BASE="https://api.minimax.cn"
# Global
# export MINIMAX_API_BASE="https://api.minimax.io"

# API key obtained from the MiniMax platform
export MINIMAX_API_KEY="<api-key>"
```

API 文档：
- H3-Image-Context-IR：使用 /v1/h3_image_context_ir [EN-docs](https://platform.minimax.io/docs/api-reference/image-generation-h3-context-ir)，[CN-docs](https://platform.minimax.cn/docs/api-reference/image-generation-h3-context-ir)
- 文生图：使用 /v1/images/generations [EN-docs](https://platform.minimax.io/docs/api-reference/image-generation-h3-generations)，[CN-docs](https://platform.minimax.cn/docs/api-reference/image-generation-h3-generations)
- 图像编辑：使用 /v1/images/edits [EN-docs](https://platform.minimax.io/docs/api-reference/image-generation-h3-edits)，[CN-docs](https://platform.minimax.cn/docs/api-reference/image-generation-h3-edits)

#### case-T2I

[`instruction.t2i.txt`](examples/instruction.t2i.txt)。

<table>
<thead>
<tr><th colspan="2">阶段</th><th>请求</th><th>结果</th></tr>
</thead>
<tbody>
<tr><td rowspan="3">提示词增强</td><td>H3-Image-Context-IR（MiniMax API）</td><td><code>python3 context_ir.py t2i</code>（<a href="examples/context_ir.py">脚本</a>）</td><td><code>revised_prompt.txt</code>、<code>revised_size.txt</code>；我们的运行结果：<a href="examples/revised_prompt.t2i.txt"><code>revised_prompt.t2i.txt</code></a>、<a href="examples/revised_size.t2i.txt"><code>revised_size.t2i.txt</code></a>（4736x3552）</td></tr>
<tr><td>本地替代方案：<a href="https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE">MiniMax-H3-Image-PE</a></td><td>PE 仓库中的 <code>scripts/expand_prompt.py</code></td><td>将 <code>expanded_caption</code> 保存为 <code>revised_prompt.txt</code>，将 <code>aspect_ratio</code> 对应的尺寸保存为 <code>revised_size.txt</code></td></tr>
<tr><td>智能体替代方案：<a href="#提示词编写技能">h3-image-prompt-writing</a></td><td>让你的智能体使用该技能，为 <code>instruction.t2i.txt</code> 写一条提示词和宽高比</td><td>将提示词保存为 <code>revised_prompt.txt</code>，将该宽高比对应的<a href="#尺寸">尺寸</a>保存为 <code>revised_size.txt</code></td></tr>
<tr><td colspan="2">MiniMax-H3-Image 生成：本地 SGLang</td><td><code>python3 t2i.py --prompt revised_prompt.txt --size $(cat revised_size.txt)</code>（<a href="examples/t2i.py">脚本</a>）</td><td><code>t2i.png</code></td></tr>
<tr><td colspan="2">端到端 API 参考：直接调用 MiniMax API 进行文生图</td><td><code>python3 api_generate.py t2i</code>（<a href="examples/api_generate.py">脚本</a>）</td><td><code>api_t2i.png</code></td></tr>
</tbody>
</table>

<p align="center">
<img src="assets/workflow_t2i.jpg" alt="左：本地 SGLang 使用增强后的提示词生成的 t2i.png。右：MiniMax API 生成的 api_t2i.png。两张图都是俯拍的农家宴席，旧木桌上摆着面包、蔬菜和奶酪" width="100%"/>
</p>
<p align="center"><em>本地 SGLang 生成的 t2i.png（左）和 MiniMax API 生成的 api_t2i.png（右），4736x3552（宽高比 4:3 由 H3-Image-Context-IR 选定）</em></p>

#### case-Edit

[`instruction.edit.txt`](examples/instruction.edit.txt)，参考图为 [`reference1.png`](examples/reference1.png)，作为 `<Picture 1>`。

| 阶段 | 请求 | 结果 |
| --- | --- | --- |
| 提示词增强：H3-Image-Context-IR（MiniMax API） | `python3 context_ir.py edit`（[脚本](examples/context_ir.py)） | `revised_prompt.txt`、`revised_size.txt`；我们的运行结果：[`revised_prompt.edit.txt`](examples/revised_prompt.edit.txt)、[`revised_size.edit.txt`](examples/revised_size.edit.txt)（4096x4096） |
| 提示词增强，智能体替代方案：[h3-image-prompt-writing](#提示词编写技能) | 让你的智能体使用该技能，针对 `reference1.png` 改写 `instruction.edit.txt` | 将提示词保存为 `revised_prompt.txt`，将 `4096x4096` 保存为 `revised_size.txt` |
| MiniMax-H3-Image 生成：本地 SGLang | `python3 edit.py --prompt revised_prompt.txt --size $(cat revised_size.txt)`（[脚本](examples/edit.py)） | `edit.png` |
| 端到端 API 参考：直接调用 MiniMax API 进行图像编辑 | `python3 api_generate.py edit`（[脚本](examples/api_generate.py)） | `api_edit.png` |

<p align="center">
<img src="assets/workflow_edit.jpg" alt="左：参考图 reference1.png，两位播客主持人，男主持人戴着耳机。中：本地 SGLang 使用增强后的提示词生成的 edit.png。右：MiniMax API 生成的 api_edit.png。两张结果图中耳机都已去掉，两位主持人在 MONEY TALKS 标牌上方碰拳" width="100%"/>
</p>
<p align="center"><em>参考图 reference1.png（左）、本地 SGLang 生成的 edit.png（中）和 MiniMax API 生成的 api_edit.png（右），4096x4096（宽高比 1:1 由 H3-Image-Context-IR 选定）</em></p>

## 提示词技巧

以下技巧来自 MiniMax-H3-Image 官方使用手册，既适用于发给 MiniMax API 的简短需求，也适用于发给你自己部署的模型的完整提示词。

### 基础描述

- **先写任务，再写风格**：先说明任务目的、图片用途、主要人物或物体，以及状态或动作，再补充风格要求。
- **先定整体布局，再补局部细节**：写清主体数量、位置、观看角度与留白。内容较多时，先说明整体分区，再描述各部分及其关系，例如：“上方标题，下方左图右文。”
- **用可见细节表达风格**：通过色彩、材质、光线与质感描述效果，用“柔和侧光、金属反光、简洁留白”代替笼统的“高级感”。优先写清关键细节，避免堆叠相互矛盾的要求。

### 文字与信息

- **具体文字逐字给全**：可用引号标出需要显示的完整文字，说明位置、层级与分行。需要模型创作文案时，明确说明。
- **不需要文字时，明确说明**：在提示词中写明“画面中不添加任何文字、字母或数字”，减少模型自行添加标题、标签或装饰文字的情况。
- **知识与数据给准、关系写清**：图表、论文配图和科普内容，应提供准确的信息、数值、单位及对应关系；涉及时间变化时，注明时间范围。使用示例数据时明确说明，避免与真实数据混淆。

### 多图参考与编辑

- **多图参考先分工**：说明每张图提供什么，以及哪些需要一致、哪些可以自由变化。例如：“图1保留产品，图2参考配色，图3参考布局。”只借用颜色时，也应说明不采用其形状或材质。
- **编辑分清“变化”与“保留”**：用位置或特征指出修改对象，说明改成什么、修改范围，以及关键保留项。例如：“左侧杯身改为蓝色，形状、材质、位置和大小保持一致。”
- **给出完整的修改结果**：区分移动、复制、替换与删除，删除时说明原位置如何补全。修改文字或数据时，提供完整的新内容，并说明原排版、图表结构及其他信息是否保留。
- **多轮编辑，每轮明确目标**：说明本轮使用哪张图、修改什么、哪些内容继续保留，减少“上一轮那个”“和之前一样”等模糊指代。
- **网格和分格写清几行几列**：九宫格、分镜、拼图类需求写成“2行3列”或“3×3（行×列）”，避免只写“2×3”造成行列颠倒；排列不规则时直接描述，例如“上排3格、下排2格”；修改其中一格时，说明是“第2行第1列”。

### 本地部署时的提示词

本地部署会原样使用你给出的提示词，最长 4096 个 token，最适合使用一段描述整张图像的长篇英文文字。在这样的提示词中，按上传顺序用 `<Picture 1>`、`<Picture 2>` 等指代参考图。[提示词编写技能](#提示词编写技能)自带的两份指南 [`t2i-en.txt`](skills/h3-image-prompt-writing/references/t2i-en.txt) 和 [`edit-en.txt`](skills/h3-image-prompt-writing/references/edit-en.txt) 详细说明了这种格式；[`examples/`](examples) 中有真实的扩写后提示词，分别对应[文生图](examples/revised_prompt.t2i.txt)和[图像编辑](examples/revised_prompt.edit.txt)。

## 许可证

- MiniMax-H3-Image 基于 [MiniMax-H3-Image Community License Agreement](LICENSE) 发布。
- 文生图 PE 模型（[MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE)）是 MiniMax-H3-Image 的一部分，因此同样受 [MiniMax-H3-Image Community License Agreement](LICENSE) 约束。
- 许可证第 IV 节所述的单独书面授权，请通过[申请表](https://platform.minimax.io/console/license)申请。

## 联系我们

请通过 [model@minimax.io](mailto:model@minimax.io) 联系我们。
