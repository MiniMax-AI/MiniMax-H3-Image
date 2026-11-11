<p align="center">
  <a href="instruction-following.md">English</a> |
  <a href="instruction-following.zh-CN.md"><strong>简体中文</strong></a> |
  <a href="instruction-following.ko.md">한국어</a> |
  <a href="instruction-following.ja.md">日本語</a>
</p>

# 精准指令遵循与理解

理解提示词中的知识、结构与表达要求，将内容组织成清晰的视觉画面。

← [最高 16 图参考](multi-reference.zh-CN.md) · [效果展示](README.zh-CN.md) · [复杂视觉挑战](visual-challenges.zh-CN.md) →

## 教育、科普、知识推理

### 论文页生成生物学科研配图

<table><tr><td width="28%" valign="top"><img src="../assets/showcase/bio-figure-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="72%" valign="top"><img src="../assets/showcase/bio-figure-output.jpg" alt="论文页生成生物学科研配图"><br><sub>输出</sub></td></tr></table>

<details>
<summary>提示词</summary>
<blockquote>根据上传的英文论文文字页，生成一张论文级生物学科研配图，16:9横版，4k。组织为3个逻辑连贯的面板：光照实验布置、幼苗初始与末态对比及角度定义、时间与弯角的数据图。幼苗和培养装置采用简洁可信的科研渲染或学术示意，数据图保持准确、清晰、克制。自行读取原文的观察方向、光源位置、形态变化、角度定义及数据，保持所有面板一致。白底、统一字体、英文短标签、a–c编号，具有正式论文配图的层次和留白。保留“synthetic study”标识，并标明示意或渲染性质；不增加原文没有的对照组、分子机制图、误差线或统计结论。</blockquote>
</details>

### 小熊猫科普图

<p align="center"><img src="../assets/showcase/red-panda-infographic.jpg" alt="小熊猫科普图" width="520"></p>

<details>
<summary>提示词</summary>
<blockquote>制作2:3中文竖版信息图，标题“读懂小熊猫”，副标题“山地森林里的树栖生活家”。高密度动物图鉴风，扁平矢量插画，浅青柠底、深松绿文字、赤陶橙身体与奶白面纹。顶部深色圆角标题条，下接档案、标尺、分布图和行为图标；中央小熊猫占约四分之一，侧身站在树枝上回望，环纹尾巴自然垂向右下，比例准确。两侧排列局部图与注释，底部以连续资料带衔接，整板视觉统一。<br>
完整包含14组知识，每组配标题、3—5条短知识及插图：<br>
01 身份：哺乳纲、食肉目、小熊猫科；以剪影区分大熊猫幼崽与浣熊。<br>
02 体型：头体长约56—62.5厘米，不含尾；尾长约37—47厘米，双标尺注明个体差异。<br>
03 面部：圆头短吻、尖耳、浅脸深泪纹，腿腹深色，配局部窗口。<br>
04 毛发：长护毛、浓密底绒、足底毛；配苔藓地衣环境色对照。<br>
05 抓握：每足五趾、爪部分收回；假拇指为特化腕骨，帮助握竹。<br>
06 尾巴：环纹、平衡、围身保暖，不能卷枝承重。<br>
07 攀树：树上休息避险、爪抓树干、灵活踝关节辅助头朝下下树。<br>
08 食谱：竹叶嫩笋为主，也吃果实昆虫，不编摄食比例。<br>
09 吃竹：前足握枝、嘴择嫩叶、臼齿咀嚼，配三步图。<br>
10 栖息地：尼泊尔、印度、不丹、中国、缅甸适宜山区；配局部分布及森林、竹丛、水源图。<br>
11 节奏：晨昏活跃、炎热时树上休息，冷时蜷缩、暖时伸展，不编精确作息。<br>
12 交流：多独居，通过气味、叫声和姿态交流。<br>
13 成长：隐蔽处营巢、新生未睁眼、母兽哺乳、逐渐探索，配四阶段图。<br>
14 保护：森林丧失与破碎化、偷猎贸易、游荡犬，对应栖息地保护、巡护监测、社区参与。<br>
至少40条有效信息、约25幅辅助图。统一造型线宽，以编号、对齐和细分隔线组织，避免同质卡片、大块空白及交叉引线。中文层级清晰，无乱码、重复填充或虚构数据。页脚来源：Smithsonian National Zoo、San Diego Zoo Wildlife Alliance、Red Panda Network。输出完整平面展板，无样机。</blockquote>
</details>

### 人员选派推理题

<p align="center"><img src="../assets/showcase/staffing-logic-puzzle.jpg" alt="人员选派推理题" width="100%"></p>

<details>
<summary>提示词</summary>
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
</details>

## 工业与产品设计

### 电动摩托爆炸图

<table><tr><td width="50%" valign="top"><img src="../assets/showcase/e-motorcycle-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="../assets/showcase/e-motorcycle-exploded.jpg" alt="电动摩托爆炸图"><br><sub>输出</sub></td></tr></table>

<details>
<summary>提示词</summary>
<blockquote>把图1这辆概念电动摩托车拆成一张非常细致的零件爆炸图，造型、白色几何车壳、金属灰电机、无轮毂车轮和橙红色灯条都与图1一致。<br>
<br>
拆解方式：等轴测视角，以电机单元为中心，所有零件沿各自装配方向向四周放射状展开，彼此留出清楚的间距、互不重叠：<br>
- 前部：前整流罩拆成上下两片，车头灯条、风挡、前叉、前轮无轮毂轮圈、轮胎、轮圈内的环形轴承和刹车盘分别分离；<br>
- 中部：白色几何车架外壳拆成左右多块切面板，露出内部管状主车架；电机单元拆出外壳、散热鳍片、定子、转子和电机控制器；电池包单独抽出，旁边是电池模组和线束；<br>
- 后部：座椅总成拆成坐垫和底座，后摇臂、后减震器、后轮轮圈、轮胎、尾灯条依次分离；<br>
- 小零件：螺栓、垫片、卡扣、轴承、接插件按所属位置成组排列在对应部件旁，用细虚线连回安装点；<br>
- 加两个圆形放大框，分别放大无轮毂轮圈的轴承结构和电机内部的定子绕组。<br>
<br>
文字标注：每个主要部件用细白色引线（末端带小圆点）连接全大写英文标签，文字清晰、拼写准确，标签沿画面边缘整齐排布。<br>
<br>
深灰色背景，带淡淡的等距网格线，柔和均匀的光线，零件边缘有干净的高光。画面饱满、层次分明、排布有序，像专业工业设计公司的结构拆解图。</blockquote>
</details>

### 喷气发动机爆炸图

<table><tr><td width="50%" valign="top"><img src="../assets/showcase/jet-engine-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="../assets/showcase/jet-engine-exploded.jpg" alt="喷气发动机爆炸图"><br><sub>输出</sub></td></tr></table>

<details>
<summary>提示词</summary>
<blockquote>把图1这台喷气发动机做成高精度爆炸结构渲染图。纯深灰色背景，斜俯视等轴测视角，部件沿一条从右上到左下的对角轴线悬浮分开：进气罩、压气机叶片盘、燃烧室、涡轮盘、中心主轴、尾喷管依次排开，机匣外壳分成几块弧形板，悬在主轴周围；电子控制盒、燃油泵、齿轮附件、燃油管和铜色线束分布在主轴两侧。外壳和机匣是冷灰、银色和哑光白，涡轮核心和主轴是暖金色和古铜色。零件对齐、间距均匀，柔和影棚光，金属反光真实。主要部件用细白色引线连到画面两侧，标注部件名称：进气罩、压气机叶片盘、燃烧室、涡轮盘、中心主轴、尾喷管、机匣外壳、电子控制单元、燃油泵、附件齿轮箱、燃油管路。标注为简洁的白色无衬线小字，左右两列整齐排布，引线不交叉，不遮挡部件。竖版2:3，无品牌标识。</blockquote>
</details>

### 摩卡壶工程蓝图

<table><tr><td width="39%" valign="top"><img src="../assets/showcase/moka-pot-input.jpg" alt="图 1"><br><sub>图 1</sub><br><img src="../assets/showcase/moka-pot-parts-input.jpg" alt="图 2"><br><sub>图 2</sub></td><td width="61%" valign="top"><img src="../assets/showcase/moka-pot-blueprint.jpg" alt="摩卡壶工程蓝图"><br><sub>输出</sub></td></tr></table>

<details>
<summary>提示词</summary>
<blockquote>把图1这只八角摩卡壶做成经典工程蓝图海报，零件构成参照图2。深蓝色带浅色网格的背景，所有图形是带轻微做旧颗粒感的白色线稿。顶部居中是大写标题"MOKA POT"；左侧竖向排列各部件的爆炸分解图（顶盖与胶木小把手、带手柄的上壶身、不锈钢过滤网、橡胶密封圈、漏斗滤杯、带安全泄压阀的下壶底座）；右上方是较大的剖面图，展示内部水路与咖啡粉仓；右下方是较小的俯视图和侧立面图。各处带尺寸线、引线和字母标记。竖版3:4，技术图纸排版。</blockquote>
</details>

### 蚂蚁六足机甲线稿

<p align="center"><img src="../assets/showcase/ant-hexapod-mech-lineart.jpg" alt="蚂蚁六足机甲线稿" width="100%"></p>

<details>
<summary>提示词</summary>
<blockquote>科幻仿生六足重型机甲的手绘线稿工业概念设计展示板，横向宽幅构图，纯白背景，主体为参考蚂蚁身体结构设计的巨型机械步行平台，采用左前方四分之三视角，略微俯视。机甲头部朝向左下方，躯干与高耸的尾部舱体向右后方延伸，六条机械腿向两侧展开，形成稳定且富有压迫感的站姿。主体占据画面中下部，顶部与周围留白区域排布独立部件线稿、仿生结构草图、手写注释和弧形指示箭头，呈现完整的游戏机械设定稿布局。<br>
<br>
主体轮廓明确区分低矮头部、连接胸段和厚重腹部三个体块。头部为扁平楔形装甲，前端带狭窄的蓝青色光学观察窗，两侧设置小型传感器与圆形机械接口；背部覆盖两块芥末黄色模块箱体，表面具有加强筋、锁扣、分段盖板和深灰固定框。头部前下方并列悬挂两组细长的虚构科幻装备，深灰主体配橙黄色外露支架，方向斜指左下；弯曲的分节金属链带从上方箱体垂落并连接下方组件，形成清晰的弧线层次。中段略收窄，保留黑色软管、承重框架和内部连杆的可见空间。<br>
<br>
六条机械腿具有昆虫式多段关节与厚实工业装甲，粗大的上肢斜向伸展，细长的下肢支撑地面，末端为低矮、宽扁的分节机械足。每条腿都包含大型圆形转轴、分层护板、液压杆、活塞、关节限位件与外露线束；近景腿体较大，远景腿体部分被机身遮挡，透视和前后关系清晰。机身右上方的腹部舱体高大厚重，由倾斜的多边形装甲板组成，侧面带白色磨损编号“02”、矩形维护口、散热缝、螺栓及两只红色小型圆柱罐，腹下密集分布机械骨架与连接管路。<br>
<br>
腹部顶部安装多种虚构设备模块：一组横向长方形箱式组件，其左端排列四个暗红色圆形端盖；旁边有圆盘状探测器、细长天线、成对竖起的小型感应杆、青绿色指示灯，以及成簇倾斜排列的短筒部件。顶部前侧伸出一根粗短的水平圆柱形探测装置，前端由多枚方形彩色光学镜片组成。所有附属设备保持统一的军绿色工业外观，关节连接与支架造型丰富，但仅作为科幻外观设计展示，不表现发射、爆炸或战斗场景。<br>
<br>
画面左上方横向摆放一幅极细长的双轨式科幻装备黑白线稿，右端为复杂箱体、电缆与圆柱模块，左端延伸为平直狭长轨道；左侧中上区域另放一幅短粗多筒组件的透视线稿，中上部放置独立矩形储存箱线稿，并以自由弯曲的黑色箭头对应主体上的相关位置。右上角绘制一只蚂蚁侧面速写，以简洁黑线概括头、胸、腹三段，并标注浅红色数字“1、2、3”；底部偏右保留一张松散的黑色仿生六足结构草图，展示机甲与昆虫形态之间的联系。少量随手书写的小字作为辅助设计注释，避免大面积文字干扰主体。<br>
<br>
整体为纯手绘线稿设定板风格：以细而略有抖动的黑色墨线勾勒全部结构，线条疏密有别，保留少量复线、断线与不完全闭合的探索性笔触。除极小面积的淡彩点色外不填任何厚涂材质，不做写实渲染，不出现镜面高光、光斑、渐变体积感或照片式质感。主体机甲采用线稿加极轻灰阶平涂：装甲面大面积留白，仅在背光面与结构缝隙用浅灰、中灰块面与零星纯黑阴影交代转折，装甲分缝、螺栓、液压杆、活塞、外露线束、束状线缆等内部机械细节全部用细线精确描绘。芥末黄色模块箱体、橙黄色外露支架、两只红色小型圆柱罐、青绿色指示灯仅以极小面积的淡彩点色示意，不做大面积填色。装甲边缘以少量短促断线与飞白笔触暗示磨损，不涂抹材质纹理。机体下方几乎不画投影，仅用两三笔极淡的灰线交代足部落地关系，画布边缘保持干净利落。<br>
<br>
左上角的双轨式装备线稿、左侧多筒组件透视线稿、中上部矩形储存箱线稿、右下角仿生六足结构草图全部为未上色的纯线稿，与主体保持同一套线稿语言。右上角蚂蚁侧面速写同样以细黑线勾出头、胸、腹三段，仅在编号“1、2、3”处用淡红色标注。弧形指示箭头与手写注释为随手勾勒的黑色线条，笔迹自由、略不规整。少量随手书写的小字作为辅助设计注释，避免大面积文字干扰主体。<br>
<br>
参数：画幅比例约3:2，超高清，线稿清晰度极高，线条粗细变化明显，色彩饱和度极低，黑白对比中高，无阴影投影，无材质渲染，无环境场景，无人物，无多余装饰边框。</blockquote>
</details>

## 机器人与具身智能

### 四足机甲 CAD 图纸

<table><tr><td width="50%" valign="top"><img src="../assets/showcase/quadruped-mech-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="../assets/showcase/quadruped-mech-cad.jpg" alt="四足机甲 CAD 图纸"><br><sub>输出</sub></td></tr></table>

<details>
<summary>提示词</summary>
<blockquote>把图1这台四足机甲整理成一张规范的 CAD 多角度工程图纸。白色图纸背景，黑色细线绘制，可见轮廓用实线，被遮挡的结构用虚线，对称轴和关节中心用点划线。<br>
<br>
图纸包含五个视图，排布整齐：<br>
- 左上：正视图；<br>
- 右上：左侧视图；<br>
- 左中：俯视图，清楚表现两个武器舱的发射孔阵列和四条腿的展开角度；<br>
- 右中：后视图；<br>
- 下方：一个较大的等轴测线框图，表现整体立体结构。<br>
<br>
各视图之间比例统一，机身、武器舱、腿部关节和大腿装甲板的形状与图1一致。标注主要尺寸：总高、总长、总宽、腿部跨距、武器舱尺寸；关键部件用引线标注"武器舱""翻盖""机身""大腿装甲板""膝关节""足部"。右下角放标准标题栏"四足机甲 总装图 1:20"。线条干净准确，排版规整，像正式的机械设计图纸</blockquote>
</details>

### 机甲巨兽爆炸 CAD 图

<table><tr><td width="43%" valign="top"><img src="../assets/showcase/mech-monster-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="57%" valign="top"><img src="../assets/showcase/mech-monster-exploded-cad.jpg" alt="机甲巨兽爆炸 CAD 图"><br><sub>输出</sub></td></tr></table>

<details>
<summary>提示词</summary>
<blockquote>【左侧爆炸图：大距离展开、完全分离】<br>
<br>
左侧呈现一幅充分展开的机械装配爆炸图。中央只保留连续的内部承力骨架，头部外壳、胸背装甲、四肢护板、关节端盖、背部棘甲和尾部鳞甲大幅移离安装位置，在骨架周围形成宽阔、有序的零件阵列。<br>
<br>
中央骨架仅占左侧区域约 45% 的宽度、40% 的高度；完整爆炸组件群则覆盖左侧区域约 90% 的宽度、85% 的高度。 为拆出的零件预留足够空间，完整展示每块零件的轮廓、厚度、内侧加强筋和安装孔位。<br>
<br>
【明确的分离距离】<br>
<br>
至少 80% 的外部装甲完全脱离骨架。大型装甲与原安装位置之间的移动距离，约为该装甲自身宽度的 1—1.5 倍。主要零件之间形成肉眼明显的白色间隔，避免护板仍贴着身体、仅露出一条缝隙。<br>
<br>
采用三级展开距离：<br>
<br>
外层装甲移动最远，构成外围零件阵列；中层连接支架位于装甲与骨架之间；内部轴承、连接环、垫圈和紧固件沿对应轴线依次展开。每一层之间都留有明显空白，能够一眼辨认零件的装配先后关系。<br>
<br>
【分区展开方向】<br>
<br>
头部组件向左上方展开：额头护板、双角安装模块、两侧护颊、传感器模块与下颌组件分别沿自己的装配方向远离头骨。头部外壳与内部框架之间留出足够大的间隔，让原本藏在头颅内部的结构完整显露。<br>
<br>
胸背装甲向上展开：背部棘甲及鳞片装甲按照原来的前后顺序，在骨架上方排列成两至三层错开的悬浮组件带。每片装甲都有独立轮廓，片与片之间留出白色间隔。装甲内侧朝向能够被观察的位置，清楚呈现加强筋、连接座和螺孔。<br>
<br>
胸腔侧板向左右展开：外侧护甲移动到外围，肋状支架停留在中间层，中央动力模块与机械脊柱留在骨架中心。管线留在所属的组件上，拆开的接口清晰可见。<br>
<br>
四肢组件向外侧及下方展开：前肢装甲分布在左下区域，后肢装甲分布在右下区域；护板、支架与关节组件各有独立空间，避免围绕腿部密集堆叠。<br>
<br>
圆形关节沿轴向拉成长列：端盖、锁紧环、垫圈、轴承与连接法兰依次排列，相邻主要零件之间的间隔约为关节直径的 0.3—0.6 倍，所有圆环严格同轴，清楚展示各层厚度与安装顺序。<br>
<br>
尾部组件向右上方展开：中央骨节链保持连续，外部鳞甲分组向上和两侧移开，形成与尾部走向平行的组件带。尾端钩刃明显脱离连接座，保留清晰的装配轴线。<br>
<br>
【装配关系与可读性】<br>
<br>
所有拆出的零件保持原有比例与安装朝向，通过细长、清晰的虚线连接到对应位置。分离距离扩大后，仍能准确判断每块装甲属于哪个部位、每组关节如何装回。<br>
<br>
主零件之间避免互相遮挡，装配引导线尽量平行，减少交叉。螺钉与小型紧固件集中排列在所属组件附近，不填满主要零件之间的空白。<br>
<br>
最终画面应清楚呈现：中央是一套裸露的机械巨兽骨架，外围是大幅移开的多层装甲与机械组件，零件之间具有宽阔、明确、连续的白色间隔。 保持纯白背景、精密黑色 CAD 线稿，以及右侧装配完成的四视图。</blockquote>
</details>

### 吊轨配送机

<p align="center"><img src="../assets/showcase/ceiling-rail-courier.jpg" alt="吊轨配送机" width="100%"></p>

<details>
<summary>提示词</summary>
<blockquote>Create a 16:9 English engineering concept sheet titled "Ceiling Rail Courier," marked "Fictional indoor transport concept." Show a long side elevation across the upper half, a detailed suspended carriage at lower left, and a three-position storyboard at lower right. Use warm white paper and cobalt linework.<br>
A straight horizontal rail spans X = 0 to 2400 mm. Define three docking stations by carriage-center coordinates: A at X = 300, B at X = 1200, and C at X = 2100 mm. Adjacent station spacing is 900 mm. The carriage is 400 mm long along X, so its footprint at A is 100–500 mm and at C is 1900–2300 mm; all positions remain within the rail. The three storyboard panels show the same carriage at A, B, and C, not three simultaneous robots.<br>
At the illustrated extension, the vertical suspension comprises an 80 mm carriage housing, a 120 mm mounting bracket, a 300 mm telescoping stem, and a 60 mm gripper, measured as consecutive segments. Mark their total as 560 mm, measured from the housing top to the gripper bottom; rail, rollers and parcel are excluded from this dimension. The gripper holds one sealed parcel throughout all panels. Include two rail rollers, one linear drive unit, one downward camera, and one two-finger gripper in the component ledger. Maintain the same dimensions, parcel, roller count, and sensor position across all views. Clearly separate horizontal station dimensions from the vertical stack.</blockquote>
</details>

### 轮腿配送机器人

<p align="center"><img src="../assets/showcase/wheel-leg-robot.jpg" alt="轮腿配送机器人" width="100%"></p>

<details>
<summary>提示词</summary>
<blockquote>机甲CAD绘制16:9中文轮腿配送机器人概念图，包含同一机器人的站立、下蹲侧视图，三维图及动力轴表，注明“虚构结构研究”。车体长500、宽360、高180毫米；四个角各装一条二关节腿，每腿末端一个直径120毫米的主动轮。腿关节共8个，轮轴电机共4个，合计12个受控旋转轴。四条腿标FL、FR、RL、RR，各自的上、下关节编号1和2，轮轴编号W；缩写中的左右以机器人自身为准。站立姿态车体顶面离地560毫米，下蹲姿态为440毫米，用同一地平线画出降低120毫米的差值。两幅图只改变关节角度，车体、轮径和连杆长度保持一致。前面板只有一台深度相机，车体上方只有一个封闭货箱；货箱在两种姿态中保持水平。用对照表区分8个腿部关节与4个驱动轮轴，避免把12个受控轴误画成12条腿或12个轮子。</blockquote>
</details>

---

← [最高 16 图参考](multi-reference.zh-CN.md) · [效果展示](README.zh-CN.md) · [复杂视觉挑战](visual-challenges.zh-CN.md) →
