<p align="center">
  <a href="SHOWCASE.md">English</a> |
  <a href="SHOWCASE.zh-CN.md"><strong>简体中文</strong></a> |
  <a href="SHOWCASE.ko.md">한국어</a> |
  <a href="SHOWCASE.ja.md">日本語</a>
</p>

# MiniMax-H3-Image 效果展示

官方使用手册中的作品，附手册给出的提示词。MiniMax API 会先扩写这些提示词再生成；本地部署时，请先按[完整工作流](README.zh-CN.md#完整工作流)扩写。

![十五张 MiniMax-H3-Image 文生图作品，横版和竖版](assets/showcase_hero.jpg)

## 开源高智能

### 最高 16 图参考

#### 16 人群像，6 种场景

<p align="center"><img src="assets/showcase/multi-ref-group-a-output.gif" alt="16 人群像，6 种场景"></p>

以 16 张人物照片为参考，生成这 16 人在 6 种场景中的群像。

#### 多图服饰配色

<p align="center"><img src="assets/showcase/multi-ref-outfit-color-output.gif" alt="多图服饰配色" width="520"></p>

以 8 位模特和 8 个色块为参考，生成 6 张配色不同的群像。

#### 十张参考图组合成客厅

<table><tr><td width="30%" valign="top"><img src="assets/showcase/furniture-room-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="70%" valign="top"><img src="assets/showcase/furniture-room-output.gif" alt="十张参考图组合成客厅"><br><sub>输出</sub></td></tr></table>

<blockquote>为「向阳家居」拍一张春季家具目录的客厅氛围图。第一张是空房实景，后面九张是本期在售家具白底图。沿用空房的机位、墙面、门窗和木地板，把九件原款家具各摆入一次，布置成一间平时可以两三个人聊天、也可以靠窗读写的客厅。皮带扶手休闲椅是主推款，给它一个看得清木框、皮带扶手和坐垫的角度。其他家具按真实尺寸和用途安排，坐下能用到桌面，书椅能拉开，从门口进屋有连续的通道。<br>
保留每件商品的颜色、材质、结构和比例，让右侧窗光自然落在布面、皮革和木头上，桌腿椅脚有可信的接触阴影。允许少量书或一枝绿植，保持陈列清爽。室内实景摄影，不加文字。</blockquote>

### 教育、科普、知识推理

#### 论文页生成生物学科研配图

<table><tr><td width="28%" valign="top"><img src="assets/showcase/bio-figure-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="72%" valign="top"><img src="assets/showcase/bio-figure-output.jpg" alt="论文页生成生物学科研配图"><br><sub>输出</sub></td></tr></table>

<blockquote>根据上传的英文论文文字页，生成一张论文级生物学科研配图，16:9横版，4k。组织为3个逻辑连贯的面板：光照实验布置、幼苗初始与末态对比及角度定义、时间与弯角的数据图。幼苗和培养装置采用简洁可信的科研渲染或学术示意，数据图保持准确、清晰、克制。自行读取原文的观察方向、光源位置、形态变化、角度定义及数据，保持所有面板一致。白底、统一字体、英文短标签、a–c编号，具有正式论文配图的层次和留白。保留“synthetic study”标识，并标明示意或渲染性质；不增加原文没有的对照组、分子机制图、误差线或统计结论。</blockquote>

#### 小熊猫科普图

<p align="center"><img src="assets/showcase/red-panda-infographic.jpg" alt="小熊猫科普图" width="520"></p>

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

#### 人员选派推理题

<p align="center"><img src="assets/showcase/staffing-logic-puzzle.jpg" alt="人员选派推理题" width="100%"></p>

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

### 工业与产品设计

#### 电动摩托爆炸图

<table><tr><td width="50%" valign="top"><img src="assets/showcase/e-motorcycle-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="assets/showcase/e-motorcycle-exploded.jpg" alt="电动摩托爆炸图"><br><sub>输出</sub></td></tr></table>

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

#### 喷气发动机爆炸图

<table><tr><td width="50%" valign="top"><img src="assets/showcase/jet-engine-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="assets/showcase/jet-engine-exploded.jpg" alt="喷气发动机爆炸图"><br><sub>输出</sub></td></tr></table>

<blockquote>把图1这台喷气发动机做成高精度爆炸结构渲染图。纯深灰色背景，斜俯视等轴测视角，部件沿一条从右上到左下的对角轴线悬浮分开：进气罩、压气机叶片盘、燃烧室、涡轮盘、中心主轴、尾喷管依次排开，机匣外壳分成几块弧形板，悬在主轴周围；电子控制盒、燃油泵、齿轮附件、燃油管和铜色线束分布在主轴两侧。外壳和机匣是冷灰、银色和哑光白，涡轮核心和主轴是暖金色和古铜色。零件对齐、间距均匀，柔和影棚光，金属反光真实。主要部件用细白色引线连到画面两侧，标注部件名称：进气罩、压气机叶片盘、燃烧室、涡轮盘、中心主轴、尾喷管、机匣外壳、电子控制单元、燃油泵、附件齿轮箱、燃油管路。标注为简洁的白色无衬线小字，左右两列整齐排布，引线不交叉，不遮挡部件。竖版2:3，无品牌标识。</blockquote>

#### 摩卡壶工程蓝图

<table><tr><td width="39%" valign="top"><img src="assets/showcase/moka-pot-input.jpg" alt="图 1"><br><sub>图 1</sub><br><img src="assets/showcase/moka-pot-parts-input.jpg" alt="图 2"><br><sub>图 2</sub></td><td width="61%" valign="top"><img src="assets/showcase/moka-pot-blueprint.jpg" alt="摩卡壶工程蓝图"><br><sub>输出</sub></td></tr></table>

<blockquote>把图1这只八角摩卡壶做成经典工程蓝图海报，零件构成参照图2。深蓝色带浅色网格的背景，所有图形是带轻微做旧颗粒感的白色线稿。顶部居中是大写标题"MOKA POT"；左侧竖向排列各部件的爆炸分解图（顶盖与胶木小把手、带手柄的上壶身、不锈钢过滤网、橡胶密封圈、漏斗滤杯、带安全泄压阀的下壶底座）；右上方是较大的剖面图，展示内部水路与咖啡粉仓；右下方是较小的俯视图和侧立面图。各处带尺寸线、引线和字母标记。竖版3:4，技术图纸排版。</blockquote>

#### 蚂蚁六足机甲线稿

<p align="center"><img src="assets/showcase/ant-hexapod-mech-lineart.jpg" alt="蚂蚁六足机甲线稿" width="100%"></p>

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

### 机器人与具身智能

#### 四足机甲 CAD 图纸

<table><tr><td width="50%" valign="top"><img src="assets/showcase/quadruped-mech-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="assets/showcase/quadruped-mech-cad.jpg" alt="四足机甲 CAD 图纸"><br><sub>输出</sub></td></tr></table>

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

#### 机甲巨兽爆炸 CAD 图

<table><tr><td width="43%" valign="top"><img src="assets/showcase/mech-monster-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="57%" valign="top"><img src="assets/showcase/mech-monster-exploded-cad.jpg" alt="机甲巨兽爆炸 CAD 图"><br><sub>输出</sub></td></tr></table>

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

#### 吊轨配送机

<p align="center"><img src="assets/showcase/ceiling-rail-courier.jpg" alt="吊轨配送机" width="100%"></p>

<blockquote>Create a 16:9 English engineering concept sheet titled "Ceiling Rail Courier," marked "Fictional indoor transport concept." Show a long side elevation across the upper half, a detailed suspended carriage at lower left, and a three-position storyboard at lower right. Use warm white paper and cobalt linework.<br>
A straight horizontal rail spans X = 0 to 2400 mm. Define three docking stations by carriage-center coordinates: A at X = 300, B at X = 1200, and C at X = 2100 mm. Adjacent station spacing is 900 mm. The carriage is 400 mm long along X, so its footprint at A is 100–500 mm and at C is 1900–2300 mm; all positions remain within the rail. The three storyboard panels show the same carriage at A, B, and C, not three simultaneous robots.<br>
At the illustrated extension, the vertical suspension comprises an 80 mm carriage housing, a 120 mm mounting bracket, a 300 mm telescoping stem, and a 60 mm gripper, measured as consecutive segments. Mark their total as 560 mm, measured from the housing top to the gripper bottom; rail, rollers and parcel are excluded from this dimension. The gripper holds one sealed parcel throughout all panels. Include two rail rollers, one linear drive unit, one downward camera, and one two-finger gripper in the component ledger. Maintain the same dimensions, parcel, roller count, and sensor position across all views. Clearly separate horizontal station dimensions from the vertical stack.</blockquote>

#### 轮腿配送机器人

<p align="center"><img src="assets/showcase/wheel-leg-robot.jpg" alt="轮腿配送机器人" width="100%"></p>

<blockquote>机甲CAD绘制16:9中文轮腿配送机器人概念图，包含同一机器人的站立、下蹲侧视图，三维图及动力轴表，注明“虚构结构研究”。车体长500、宽360、高180毫米；四个角各装一条二关节腿，每腿末端一个直径120毫米的主动轮。腿关节共8个，轮轴电机共4个，合计12个受控旋转轴。四条腿标FL、FR、RL、RR，各自的上、下关节编号1和2，轮轴编号W；缩写中的左右以机器人自身为准。站立姿态车体顶面离地560毫米，下蹲姿态为440毫米，用同一地平线画出降低120毫米的差值。两幅图只改变关节角度，车体、轮径和连杆长度保持一致。前面板只有一台深度相机，车体上方只有一个封闭货箱；货箱在两种姿态中保持水平。用对照表区分8个腿部关节与4个驱动轮轴，避免把12个受控轴误画成12条腿或12个轮子。</blockquote>

### 复杂视觉挑战

#### 直角镜面

<p align="center"><img src="assets/showcase/mirror-reflection.jpg" alt="直角镜面" width="100%"></p>

<blockquote>真实摄影呈现一套桌面光学展示：两面竖直平面镜沿竖边相接，夹角为直角，镜面朝向夹角内部。相机从开口方向略偏一侧拍摄，完整纳入镜角前的实物和两面镜中的三组对应镜像。实物是一座小型车站模型：中央钟楼、只位于钟楼一侧的高水塔、另一侧的低候车棚，前方停着一辆带黄色车头和黑色尾部的小车；一根弯曲红线连接水塔底部与候车棚。模型前方竖着正面朝向镜角的标牌，文字为“R7”，实拍可见标牌背面。两侧各有一组经过一次反射的模型像，镜角深处还有一组经过两次反射的模型像；两侧标牌文字呈镜写，双次反射中的“R7”可以正常阅读。水塔、候车棚、车头和红线在三组镜像中随反射共同改变方向，保留各自与钟楼的位置关系。镜面接缝和装置底座清楚可辨，倒影之间留出足够空间识别每组模型。</blockquote>

#### 伸进投影的手

<p align="center"><img src="assets/showcase/projection-hand-shadow.jpg" alt="伸进投影的手" width="100%"></p>

<blockquote>一张真实的投影艺术装置现场照片：投影机把蓝白棋盘格投到白色石膏半身像上，格线随鼻梁、面颊和胸部曲面改变形状。操作者站在投射范围旁，将一只五指分开的手伸到雕像胸前的光路中，掌面朝向投影机。手掌本身接到一部分棋盘图案，后方雕像胸前则出现不含棋盘纹样的暗手影；亮格在影边被截断，指缝对应的位置仍有投射光通过。从侧前方取景，让实际手掌与胸前手影在画面中错开，能同时看到人物上半身、雕像和侧缘开启的投影机。</blockquote>

#### 游戏地图变 3D 游戏画面

<table><tr><td width="46%" valign="top"><img src="assets/showcase/game-map-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="54%" valign="top"><img src="assets/showcase/game-map-to-3d.jpg" alt="游戏地图变 3D 游戏画面"><br><sub>输出</sub></td></tr></table>

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

#### 鹈鹕毕业叠罗汉

<p align="center"><img src="assets/showcase/pelican-graduation-pyramid.jpg" alt="鹈鹕毕业叠罗汉" width="520"></p>

#### 鹈鹕圣诞树

<p align="center"><img src="assets/showcase/pelican-christmas-tree.jpg" alt="鹈鹕圣诞树" width="520"></p>

#### 鹈鹕平衡挑战

<p align="center"><img src="assets/showcase/pelican-challenge-3.jpg" alt="鹈鹕平衡挑战" width="520"></p>

## 创意生产

### 游戏世界

#### 边境骑手

<p align="center"><img src="assets/showcase/frontier-rider.jpg" alt="边境骑手" width="100%"></p>

<blockquote>Aspect ratio 16:9, 4K. Create original game key art that evokes the genre atmosphere of a major AAA production through mood, gameplay motifs and composition. Use realistic 3D materials and cinematic lighting, with original identities, costumes and symbols. Scene: An adult frontier rider waits at a waystation as a sandstorm approaches and the horse turns its head. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

#### 荒漠大集会

<p align="center"><img src="assets/showcase/desert-gathering.jpg" alt="荒漠大集会" width="100%"></p>

<blockquote>画幅比例 21:9。史诗感写实电影场面，从人物身后的高处岩台俯视巨大沙漠集会，一个披着深色长斗篷的人物站在近景中央偏左，背对镜头，轮廓几乎形成黑色剪影。下方密密麻麻的人群铺满宽阔的沙地与岩石围合的天然剧场，人群以极小尺度向远方延伸，排列不完全整齐，每个身影融成细密有序的纹理。两侧褐色岩壁、粗糙台阶和隆起岩台构成空间边界，暖米黄色空气中有轻微尘雾。高处自然日光照亮场地，前景保留深阴影，强调孤立的近景人物与庞大集体的尺度对照，真实电影调色。</blockquote>

#### 冷色矿物荒原航拍

<p align="center"><img src="assets/showcase/cold-mineral-aerial.jpg" alt="冷色矿物荒原航拍" width="100%"></p>

<blockquote>一幅游戏CG风格的超广角航拍画面，以略带倾斜的高空俯视视角呈现辽阔的矿物荒原。整体色调由红褐暖色转为深靛蓝、冷灰、青绿色与银白色，地表如天然玛瑙切片般铺展，层层矿物色带交织成不规则的环状沉积纹理与蜿蜒分支。画面没有天空和地平线，所有视觉信息集中于地表肌理，营造陌生、寂静而壮阔的异域地貌。<br>
<br>
一条较明亮的灰青色狭长通道从画面右下方进入，向中央偏左弯折，再沿柔缓的S形曲线延伸至左上方远处，取代笔直的对角线布局，成为引导视线深入画面的主要动线。通道位于画面偏左区域，右侧保留大面积深靛蓝矿物沉积地貌，形成疏密有致的非对称构图。通道两侧分布银白色、冷灰色的矿物结壳与细窄沟槽，边缘曲折自然，仿佛干涸水系留下的浅色脉络。大片暗青色沉积区域具有细密的波浪状层理，局部夹杂淡蓝绿色细线，纹路顺着地形弯曲、汇聚、分流。<br>
<br>
约十名身穿深灰与黑褐色长衣的微小旅人沿通道疏散行进，人物在画面中占比极小，仅保留清晰的人形轮廓，不强调面部细节。队伍从右下方向中央偏左的弯道延伸，再逐渐隐入左上方的狭窄通路，间距不均，部分人物靠近白色岩块，部分穿行于裸露的灰青色地面。队伍的视觉重心落在左侧三分线附近，与右侧辽阔空旷的地貌形成平衡，人物尺度与巨大地貌形成强烈对比，使画面带有孤独的旅途感与史诗叙事气息。<br>
<br>
通道沿线散落大小不一的灰白色岩石，右下方通道入口附近分布较大的粗粝岩块，中央偏左的转弯处与左上方远处有零散碎石和几块突出的浅色巨石，形成由近及远的空间层次。岩石表面呈风化、粉化的颗粒质感，棱角不规则，受光面泛出冷白亮色，背光面沉入深蓝灰色阴影。地面兼具干燥矿壳、细砂与少量细碎反光颗粒，以高精度游戏环境资产的材质表现呈现丰富细节，不过度锐化。<br>
<br>
低角度冷白色阳光从画面左上方照入，旅人与岩石的阴影向右下方拉出极长的斜线。多道狭长阴影沿S形通道交错分布，与蜿蜒地纹形成鲜明对照。整体采用低调曝光，右侧地貌深沉、左侧通道稍亮，保留自然暗角；银白高光、低饱和青绿色中间调与深靛蓝阴影构成克制的冷色层次，带有轻微空气尘雾与细腻的电影级后期质感。<br>
<br>
风格与参数：高品质游戏CG，写实向三维地貌渲染，电影级游戏过场画面，基于物理的材质表现，全局光照，电影级航拍构图，高空倾斜俯拍，超远景，S形引导线，非对称布局，宽银幕比例约2.5:1，高清细节，深景深，地表纹理清晰，低照度冷光，高动态范围，适度低饱和，柔和高光，深色阴影，无文字、无标志、无边框。</blockquote>

#### 红褐矿物荒原航拍

<p align="center"><img src="assets/showcase/desert-mineral-aerial.jpg" alt="红褐矿物荒原航拍" width="100%"></p>

<blockquote>电影感超广角航拍，近乎垂直俯视辽阔的红褐色矿物荒原，2.5:1宽银幕，无天空与地平线。地表如天然玛瑙切片，铁锈红、深赭石、焦糖橙与暗棕层层交织，形成不规则环状沉积、波浪层理与蜿蜒分支，局部夹杂金色细线，呈现陌生、寂静而壮阔的地貌。<br>
明亮的橙褐色狭长通道从左下延伸至右上，构成对角线骨架。两侧分布乳白矿物结壳、灰白岩块与细窄沟槽，宛如干涸水系。约十名身穿深灰、黑褐长衣的微小旅人沿通道蜿蜒前行，间距不均，部分靠近白色岩块，人物不强调面部，与巨大地貌形成鲜明尺度对比，带出孤独旅途与史诗叙事感。<br>
沿途岩石大小错落，表面粗粝风化、棱角不规则；地面融合干燥矿壳、细砂与少量反光颗粒。低角度暖阳从左上照入，将旅人与岩石的阴影拉向右下，狭长阴影与弯曲地纹交错。整体低调曝光，四周深暗、中央稍亮，暖橙高光与深红褐阴影层次克制。<br>
写实地貌摄影，超远景、深景深、高清纹理、高动态范围，适度低饱和，柔和高光与自然暗角，轻微尘雾和细腻胶片颗粒，不过度锐化，无文字、标志及边框。</blockquote>

#### 森林中的古剧场

<p align="center"><img src="assets/showcase/forest-amphitheater.jpg" alt="森林中的古剧场" width="100%"></p>

<blockquote>画面比例16:9，4K。做一张面向3A游戏的环境概念成图，先读出地形、地标和聚落用途，再看到细节。采用可信写实3D空间，建筑顺应气候与地势，保留前中后景。具体内容：被森林吞没的圆形剧场，树根沿裂缝进入座席。不使用现有作品的名称、角色或品牌标志，不添加水印。</blockquote>

#### 云海仙山宫阙

<p align="center"><img src="assets/showcase/mountain-temple.jpg" alt="云海仙山宫阙" width="100%"></p>

<blockquote>画面比例21:9，4K。制作电影级写实数字绘景，适合3A过场的远景扩展。前景清晰、中景有结构、远景用大气透视递减，统一地平线、光照与尺度，建筑和地貌自然衔接，不出现拼贴边缘。具体内容：高山寺院群沿山脊延伸，金色晨光逐层照亮屋顶。不使用现有作品的名称、角色或品牌标志，不添加水印。</blockquote>

#### 巫师释放扇形火焰

<p align="center"><img src="assets/showcase/fire-mage-vfx.jpg" alt="巫师释放扇形火焰" width="100%"></p>

<blockquote>Aspect ratio 16:9, 4K. Render a realistic AAA game effect at its peak, keeping the character or device and ground readable. Clearly distinguish origin, direction and area of influence, with layered particle density and environmental light interaction, without damage numbers, UI or text. Scene: An adult mage releases a fan of fire from the palm with flame tails bending downwind. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

#### 爆炸的两个阶段

<p align="center"><img src="assets/showcase/explosion-two-state.jpg" alt="爆炸的两个阶段" width="100%"></p>

<blockquote>一张电影特效爆炸模拟的双状态对照画面，纯黑背景，下方各有灰色无纹理水平地面。左右两个并排视窗保持相同机位和尺度：左侧呈现爆炸早期，翻滚火球呈明亮橙黄颜色，火舌密集形成花椰菜状细节；右侧呈现稍晚阶段，底部仍有橙色火焰，上方大团厚重深灰烟云向右上翻卷。体积火焰与烟雾具有真实透光、密度、湍流和层次，较高快门凝固瞬间，画面重点是火与烟的形态及相互遮挡。 输出一张完整图像，保留上述构图和视图数量；不添加网页边框、作者签名或水印。</blockquote>

#### 重甲骑士角色设定

<p align="center"><img src="assets/showcase/armored-knight-sheet.jpg" alt="重甲骑士角色设定" width="100%"></p>

<blockquote>暗黑奇幻游戏角色设定板，深灰渐变摄影棚背景。同一名高大男性重甲骑士以正面、背面和去除披肩后的正面全身三个视图并排展示，姿势和比例一致。面部完全藏在尖棱封闭头盔内，深色钢铁板甲有尖角肩甲、分片胸甲、护臂、膝甲与胫甲；颈肩围着磨损的灰黑布披肩，腰间是层叠的暗褐皮革裙甲和绑带。视图之间放置独立肩甲与胸甲小特写。写实游戏概念美术，金属磨痕、皮革粗糙度和布料褶皱清晰，冷灰主色，柔和顶侧光，完整展示脚部与轮廓。 输出一张完整图像，保留上述构图和视图数量；不添加网页边框、作者签名或水印。</blockquote>

#### 狮王面部特写

<p align="center"><img src="assets/showcase/lion-king-face.jpg" alt="狮王面部特写" width="100%"></p>

<blockquote>画幅比例 21:9。写实奇幻生物面部特写，一个兼具狮子鬃毛与猿类面部结构的兽王朝向镜头略偏左，宽阔灰色鼻梁、深陷眼窝和琥珀色眼睛清楚，嘴唇略微张开露出少量小型象牙色牙齿。面部覆盖短而密的灰白毛发，周围巨大的棕褐与银白鬃毛向画面右侧和下方铺开，毛束有自然卷曲、层次和蓬松体积，发丝受到细腻侧光照亮。右下边缘仅露出一小部分暗金色饰件，主体仍是脸部与鬃毛。深色虚化背景，真实皮肤与毛发交界、湿润眼球反射和电影级生物材质。 输出单张完整作品画面，不添加网站边框、作者署名或水印。</blockquote>

#### 森林中的龙

<p align="center"><img src="assets/showcase/forest-dragon.jpg" alt="森林中的龙" width="600"></p>

<blockquote>写实幻想电影生物立于幽暗森林的岩石上，正方形全身构图。主体是一只高颈、细长身体的龙，灰蓝与墨绿色细鳞皮肤，腹部偏米灰色，背部从肩膀到尾部竖起扇形暗红色鳍膜；头部张嘴嘶吼，额头与脸颊生出许多向后飘卷的粉红色长须和角状肉质冠，须丝形成优雅复杂的轮廓。四肢为有锐爪的爬行动物结构，长尾绕身体向左弯曲，脚踩湿润石块和苔藓。森林柔和自然光穿透部分须冠，材质细腻可信，无文字或水印。</blockquote>

#### 第一人称射击场景

<p align="center"><img src="assets/showcase/fps-wasteland.jpg" alt="第一人称射击场景" width="100%"></p>

<blockquote>画幅比例 16:9。写实末世第一人称射击游戏场景，镜头前方下缘可见玩家双手持握的步枪与瞄具，指向一条荒废林地公路。左侧中景一名穿绿色战术服、背包与头盔的同伴向前方射击，枪口闪出小团橙黄色火光；右侧另一名戴兜帽、穿旧棕色外套的战士半蹲持长枪。远处道路被高大松树、灰色灌木与薄雾包围，左后方有一辆生锈黄色巴士，地面杂草、石块与泥土细节丰富。清晨或黄昏的低位日光从树林后透出，冷灰绿环境与短促枪火对比，人物装备结构真实，紧张但没有血腥内容，不加 HUD。</blockquote>

#### 白模渲染图变电影剧照

<table><tr><td width="50%" valign="top"><img src="assets/showcase/whitebox-moon-input.jpg" alt="输入"><br><sub>输入</sub></td><td width="50%" valign="top"><img src="assets/showcase/moon-rover-render.jpg" alt="白模渲染图变电影剧照"><br><sub>输出</sub></td></tr></table>

<blockquote>把这张白模渲染成真实月面科考电影画面。补全灰色月壤、银白隔热层、涂层金属、玻璃与轮网材质，宇航服为米白色。使用强方向性太阳光和有限地面反射，远处天空纯黑，不加蓝天、云或地球式雾气。保持探测车六个车轮、人物和舱段布局，阴影方向统一，亮部保留材质细节。 保留原图构图、镜头角度、透视、几何结构与各主体的位置和比例；输出4K、16:9横版，呈现3A级写实CG与电影实拍融合的质感，不添加文字、品牌、界面或水印。</blockquote>

#### 峡谷水电站绘景

<p align="center"><img src="assets/showcase/hydro-station-canyon.jpg" alt="峡谷水电站绘景" width="100%"></p>

<blockquote>Aspect ratio 21:9, 4K. Create a cinematic photoreal matte painting suitable for extending an AAA cutscene. Use a crisp foreground, structured middle distance and atmospheric recession, with consistent horizon, light and scale and seamless transitions between architecture and terrain. Scene: An old hydro station enclosed by red canyons with a long channel crossing the scene. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

#### 废弃车站

<p align="center"><img src="assets/showcase/abandoned-station.jpg" alt="废弃车站" width="100%"></p>

<blockquote>Aspect ratio 16:9, 4K. Generate a photorealistic AAA image with a high-end real-time engine look. Emphasize indirect illumination, varied roughness, contact shadows and depth separation. Show only the rendered scene, without an editor or performance counters. Scene: Sunlight enters an abandoned station through a glass roof and reflects its steel frame in wet tiles. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

#### 末世工业厂区

<p align="center"><img src="assets/showcase/industrial-ruins.jpg" alt="末世工业厂区" width="100%"></p>

<blockquote>画幅比例 16:9。写实末世工业厂区外景，低机位穿过满是碎石和废料的狭窄院落。左侧近景为高大的褪色红砖墙，右侧是残破混凝土厂房；中央远处立着多层钢架生产塔、圆筒罐、连桥和粗大烟囱。前景零散摆放生锈油桶、破木板与枯黄灌木，地面泥泞有浅水反射。厚重灰云压低天空，阳光从云缝穿出局部照亮建筑，黑色鸟群盘旋。强烈纵深和建筑遮挡形成紧张气氛，混凝土剥落、锈蚀钢板、断裂窗框与植被侵蚀细节清晰，整体低饱和灰黄配色，写实游戏环境渲染。 输出单张完整作品画面，不添加网站边框、作者署名或水印。</blockquote>

#### 冰封海湾中的沉船

<p align="center"><img src="assets/showcase/frozen-shipwreck-bay.jpg" alt="冰封海湾中的沉船" width="100%"></p>

<blockquote>极寒冰封海湾中的废弃船舶遗址，2.2:1超宽全景，24mm广角微俯视。左侧倾斜船骸覆满积雪与冰柱，锈蚀集装箱散落甲板。中央碎冰裂隙延伸至蓝水道，青绿冰壁透光，浮冰与残片漂流。右侧白灰拖船搁浅，远处红色货轮倾覆于冰川之间。背景雪山、冰崖与稀疏针叶林隐入寒雾。冰蓝青灰主调，暗红船体点缀，冷冽日光形成近暗远亮层次，寂静荒凉。电影级写实，真实冰雪金属材质与水面反射，深景深、体积雾、8K，无人、无字、无水印。</blockquote>

#### 战斗驾驶员

<p align="center"><img src="assets/showcase/combat-pilot.jpg" alt="战斗驾驶员" width="600"></p>

<blockquote>画幅比例 1:1。写实未来战斗驾驶员的近距离半身肖像，年轻男性脸部冷峻、眼睛微向右看，面颊有细小擦伤，头发藏在复杂的开放式装甲头盔内。头盔为橄榄绿与旧白色工业壳体，顶部有红白斜纹徽记，面部两侧排列传感器、黑色光学镜头、通讯盒和铰接支架，下颌装有护颈框架。白灰色胸甲厚重，有深色胸带、软管、编号“003”、贴纸和细小警示标记，表面有划痕、积尘和边缘掉漆。主体靠近镜头，纯黑背景，冷色左上软光勾勒脸部与设备轮廓，强调复杂机械装配、皮肤真实感和军用硬表面材质。 输出单张完整作品画面，不添加网站边框、作者署名或水印。</blockquote>

#### 极地服装设定

<p align="center"><img src="assets/showcase/polar-costume-board.jpg" alt="极地服装设定" width="100%"></p>

<blockquote>Aspect ratio 3:2, 4K. Create an original AAA costume board: full front view on the left, full rear view in the center and one construction close-up on the right, using the same adult model and outfit. Show realistic 3D drape, seams and fastening structures against pale gray without text. Scene: An insulated polar communicator outfit with fur collar, sealed cuffs and gaiters. Use original identities and designs without existing franchise names, characters, brand marks or watermarks.</blockquote>

#### 红色荒原上的头盔

<p align="center"><img src="assets/showcase/helmet-key-art.jpg" alt="红色荒原上的头盔" width="520"></p>

<blockquote>画面比例3:4，4K。绘制原创3A游戏的竖版封面主视觉，写实3D、强烈而克制的电影光影。让单一主角或核心物占据明确焦点，顶部约四分之一保持安静用于后续排字，当前图不生成标题、标志或文字。具体内容：蒙尘宇航头盔躺在红色荒原上，镜面反射远处基地。不使用现有作品的名称、角色或品牌标志，不添加水印。</blockquote>

#### 科幻战斗机

<p align="center"><img src="assets/showcase/scifi-fighter.jpg" alt="科幻战斗机" width="100%"></p>

<blockquote>画幅比例 16:9。写实科幻战斗机资产展示，从上方略俯视机体后侧的三分之四视角，战机停在中性深灰地面上，整体为低矮流线形白灰机身，局部红色装甲与红色尾翼形成鲜明点缀。两组大尺寸黑色矩形喷口位于机身尾部，喷口周围有机械层级与散热结构，机翼向左右展开，翼下分布小型挂载和细长设备，机背有抬起的鳍状结构。表面保留清晰分件缝、面板厚度、金属连接与轻度使用痕迹。柔和棚拍顶光，地面有自然接触阴影，重点展示双引擎布局和干净可读的硬表面轮廓。 输出单张完整作品画面，不添加网站边框、作者署名或水印。</blockquote>

#### 科幻改装肌肉车

<p align="center"><img src="assets/showcase/modded-muscle-car.jpg" alt="科幻改装肌肉车" width="100%"></p>

<blockquote>一张精细的科幻改装载具概念设计展示板，横版构图，浅暖灰色工作室背景。主体是一辆经过重度机械改装的复古双门肌肉跑车：修长的发动机舱、低矮倾斜的前挡风玻璃、流畅的溜背车顶、短促厚实的车尾，车身宽阔，姿态强悍。保留经典公路跑车的辨识度，同时融入近未来工业设备与末世越野载具的机械细节。<br>
<br>
车身造型：<br>
整车采用低饱和灰蓝色涂装，带轻微青绿色倾向。长引擎盖由几块宽大的金属面板构成，表面具有明确的折线、分缝和固定螺栓。车头低平而宽，左右分体式黑色进气格栅嵌在厚实的金属框架内，两侧配置深陷式圆形前灯，辅以细窄的琥珀色灯条。前翼子板外扩，轮拱由多层弧形金属护板叠合而成，边缘清楚可见铆钉与安装缝。<br>
<br>
引擎盖中央安装一组低矮的外露机械动力模块，包含金属进气口、短圆筒、管路、连接支架和紧固件，整体紧贴车身，不破坏修长的车头轮廓。前轮后方设置小型三角通风口和竖向散热百叶。车门宽大，保留简洁的机械门把手与小型后视镜；侧窗开口中可以看见深色座椅、方向盘以及少量防滚架结构。后翼子板饱满有力，车尾设置小型扰流板，一根细长天线从后部垂直伸出。<br>
<br>
轮胎与底盘：<br>
采用四轮布局，前后轮都使用宽厚的越野轮胎，胎面是清晰的大块切割纹路，胎壁有克制的模压字符。轮毂采用深凹式结构，外圈为磨损的橙铜色，中央为暗金属色机械轮芯，形成整车最醒目的色彩点缀。<br>
<br>
车身适度抬高，轮胎与轮拱之间保留可见间隙，露出悬挂、减振器和连接支架。前保险杠下方是开放的机械结构，可以看见横梁、圆形传动件、金属护架、管线与拖曳固定点。车门下沿延伸出细长的金属连杆与保护杆，后轮前方露出银色圆筒形储罐及连接管路，车尾侧下方伸出短粗的金属排气管。机械细节主要集中在前下部、底盘和轮拱内部，车门与车顶保留较完整的大块金属表面。<br>
<br>
材质与使用痕迹：<br>
灰蓝色漆面具有细腻的半哑光反射，局部边缘轻微掉漆，露出暗银色金属。轮拱、检修口、门缝和底盘附近带有少量灰尘、油污与磨损，橡胶轮胎呈现真实的粗糙质感。车身散布少量褪色的白色识别标记、橙色工业警示贴纸、细小编号和维护标签，尺寸克制，分布符合机械设备的使用逻辑。整体呈现长期使用但维护良好的状态。<br>
<br>
主视图构图：<br>
整车占据画面中下部约75%的视觉面积，采用左前侧三分之四视角，车头朝向画面左侧，车尾延伸至右侧。相机略高于车灯，以自然的中长焦透视同时呈现引擎盖、侧面车门、近侧两只车轮和部分车顶。四周留出适当空间，完整保留车头、轮胎、车尾和天线。车辆静止停放在浅灰地面上，底部有清楚的接触阴影，整体姿态沉稳、厚重而富有力量。<br>
<br>
辅助视图与版式：<br>
画面顶部保留一条疏朗的技术资料区域：左上是窄列的小字号说明与几条橙褐色分隔线；顶部偏左放置同一车辆的小型俯视图，中间放置小型侧视图，右上角放置更淡的正面结构线稿。辅助视图使用低对比度灰褐色线条，局部保留淡灰蓝色车身色块，视觉权重明显低于主视图。<br>
<br>
所有辅助图沿统一水平线组织，保持整齐间距，并使用极少量细引线、编号和短标签。标题与标签可使用“VEHICLE CONCEPT”“TOP VIEW”“SIDE VIEW”“FRONT VIEW”等简短英文，采用细窄的工程无衬线字体。整体像一张完成度很高的工业载具设计档案，排版克制，信息丰富，主次明确。<br>
<br>
光照与画面风格：<br>
使用左上方的大面积柔和主光，结合轻微侧逆光，清楚表现车身折面、漆面反射、轮胎厚度和底盘机械层次。背景保持干净的浅灰渐变，阴影自然，色调以灰蓝、暖灰、暗金属和少量橙铜色为主。写实的三维硬表面渲染，精密工业设计质感，高清晰度，细节丰富，整体具有复古、冷静、硬朗的近未来气质。<br>
<br>
输出一张完整概念设计展示图，保持一张大型整车主视图和顶部三张小型技术视图。无真实汽车品牌标识、无网站界面、无作者签名或水印。</blockquote>

### 现实世界

#### 雾中农场，纪实胶片

<p align="center"><img src="assets/showcase/farm-documentary-film.jpg" alt="雾中农场，纪实胶片" width="520"></p>

<blockquote>一张真实的乡村纪实摄影照片，竖幅构图，像纪实摄影师用标准镜头和胶片拍下的一个农场里的普通瞬间，自然光，没有任何人工打光，没有摆拍。<br>
<br>
【天气与空间】<br>
大雾天，可能还飘着细小的雪花或雨丝，空气里散落着微小的白点。远处完全被浓重的白雾吞没，看不到地平线、建筑或树，只有一片均匀的雾白。全漫射光，几乎没有影子。<br>
<br>
【前景主体：妇人与小牛】<br>
画面中下部偏左，一位中年偏老的妇人站在湿漉漉的草地上，约占画面高度的一半。她面容沉静，微微低着头，看着脚边的小牛。头上包着一条红黑花色的头巾，身穿一件黑色过膝的双排扣长大衣，黑裤子、黑鞋。她右手握着一个奶瓶，向下伸着在喂小牛。<br>
她脚边偏右，一头棕黄色毛的小牛犊，仰着头衔住奶瓶吮吸，姿态温顺。<br>
<br>
【中景：旧皮卡和装牛的人】<br>
妇人身后，草地上停着一辆老旧的淡蓝色单排座皮卡车，车斗加装了深蓝色的铁栏板，后栏板向两边大开着，车斗里铺着干草。<br>
- 车斗里站着一头成年的白底褐色斑块奶牛，头朝左；<br>
- 车头侧面，一位微微驼背的老汉，戴深色鸭舌平顶帽，穿深色夹克和黑裤，双手拉着系在车上的绳子；<br>
- 车尾右侧敞开的栏板旁，站着一个戴深色鸭舌帽、穿工装外套的男人，正照看着车斗；<br>
- 车尾正后方，另一个穿灰色连帽卫衣和侧边带白条纹的黑色运动裤的男人，弯着腰把上半身探进车斗里干活；<br>
- 车尾旁的地上，一头黑白花的小牛侧对或背对镜头，正探头往车斗里吃干草。<br>
这些人都在各忙各的，没有人看镜头。<br>
<br>
【前景地面】<br>
颜色偏暗的湿草地，杂草蓬乱，局部露出泥土。<br>
<br>
【镜头与构图】<br>
全景，机位基本平视，略低一点，大约与妇人胸口同高。35mm 到 50mm 的标准焦段，透视自然，没有畸变。中等景深：妇人和小牛相对清晰，后面的皮卡和人的轮廓完整但稍软，远处被雾自然吃掉。<br>
<br>
【色调与画质】<br>
冷色调，整体青绿偏灰，饱和度低。主要颜色是雾白、青灰、衣服的深黑、草地的暗绿和皮卡复古的淡蓝，妇人头巾的红色是唯一的暖色点缀。对比度适中偏低，雾气里的高光略微过曝发白，画面有柔和的漫射感和中等的胶片颗粒。画面里没有任何文字、水印或界面元素。<br>
<br>
整体氛围质朴、苍茫、沉静，带着生计的气息，又有一点人和动物之间的温情。不是CG，不是插画，不是摆拍，是一张真实的照片。</blockquote>

#### 胶片质感野餐

<p align="center"><img src="assets/showcase/picnic-film.jpg" alt="胶片质感野餐" width="520"></p>

<blockquote>一幅复古胶片质感的户外时尚生活方式摄影，三位成年朋友在草地上的华丽织毯间悠闲野餐，整体氛围静谧、亲密、慵懒，带有波西米亚风格与秋日田园气息。横向画幅，画面比例3:2，略高机位斜向俯拍，中近景群像构图，人物与织物占据画面中下部，背景为自然生长的深绿色草地，保留适量环境空间。<br>
<br>
画面中央偏上，一位成年女性坐在地毯上，深棕色齐肩直发自然中分，身穿宽松的玫红色翻领长袖衬衫，布料上分布深酒红色抽象植物纹样。她的身体朝向镜头，面部转向画面左侧，神情沉静，视线望向远处，双手自然搭在身旁朋友的肩臂附近。她是三角形人物布局的最高点，鲜艳上衣成为深绿色环境中的主要视觉焦点。<br>
<br>
前景左下方，一位短发成年男性斜躺在地毯与抱枕上，头部靠近画面中心，双腿伸向左下角，一条腿微微屈起，穿着宽松的青蓝色长裤。胸肩自然露出，深色底、奶白色与土黄色大叶片图案的织物松散覆盖部分躯干，手掌轻搭胸前，表情放松。右侧一位成年女性侧躺，头枕在坐姿女性身旁，戴浅色印花头巾，穿灰玫瑰色粗针织开衫及奶白底酒红色斑点图案长裤，赤足向右侧伸展，手臂自然弯曲，目光轻柔地看向镜头。<br>
<br>
地面铺着大面积黑色与赭黄色动物纹地毯，四周饰有细密红色边框，叠放多条青绿、金黄、酒红、奶白相间的植物印花薄毯。人物头侧与腰前摆放不同形状的装饰抱枕，包括粉红与青绿色叶片纹长枕，以及奶白底棕红色插画、亮黄色侧边的方形抱枕。细致呈现针织开衫的粗线圈、棉布褶皱、地毯绒面与流苏，使繁复图案形成丰富但协调的层次。<br>
<br>
画面左侧安排丰盛而自然的野餐静物：藤编篮中露出长法棍面包、蓝白条纹餐布和一束带浅色小花的乡野花草；篮子后方的木箱上放置白色高脚蛋糕盘，盘中是一只深棕色水果挞。左下角木箱桌面上摆放蓝白陶瓷碗盘、紫红色葡萄、切开的西瓜和几颗暖色水果，部分物件被画框自然裁切。左侧前景加入一簇贴近镜头、明显虚化的深绿色植物，局部遮挡篮子与背景，营造从草木间窥见野餐场景的空间感。<br>
<br>
采用柔和的自然漫射光，略带温暖的侧向光泽，人物肤色真实柔润，阴影保留细节。整体色调以橄榄绿、酒红、玫瑰粉、青蓝与赭黄为主，低至中等对比度，轻微褪色，细腻胶片颗粒，暗部略沉，避免鲜艳过度和商业棚拍般的光滑质感。参数：焦距约40mm，光圈约f/4，快门约1/250秒，感光度ISO 400，中等景深，人物与主要织物清晰，近景植物明显虚化，背景草地柔和可辨；高分辨率，真实人体比例，自然皮肤纹理，无文字、无水印、无界面按钮。</blockquote>

#### 胶片人像特写

<p align="center"><img src="assets/showcase/film-portrait-closeup.jpg" alt="胶片人像特写" width="100%"></p>

<blockquote>一幅写实电影胶片风格的人像特写，画面中央是一位成年女性的面部，浅肤色，浅棕偏红的短发自然蓬松，灰绿色眼睛望向镜头，神情平静而略带思索。面部保留真实肌肤纹理、细微雀斑与自然色泽，眉毛纤细柔和，睫毛清晰，嘴唇呈低饱和玫瑰色，轻轻闭合，不露齿。<br>
<br>
采用极近距离正面构图，面部几乎占满整个影像区域，额头上缘与下巴被画面裁切，嘴唇靠近底部边缘。画面左侧的眼睛完整清晰，是主要视觉焦点；另一只眼睛被掠过面部的发丝部分遮挡。鼻梁与鼻尖位于中央偏下，左右构图略微不对称，呈现自然抓拍感。<br>
<br>
微风吹动浅栗棕色头发，带有铜金色光泽的发束从画面上方斜向右侧横掠，形成柔和的弧线与轻微运动模糊。少量细发散落在额头、眉眼及脸颊前方，与清晰的眼睛、鼻翼和唇部形成虚实对比；发丝层次自然，避免整齐僵硬的造型。<br>
<br>
光线为柔和的暖色自然光，面部受光均匀，鼻侧与脸颊保留浅淡阴影，明暗过渡细腻，没有强烈硬光或明显轮廓光。整体采用温暖的琥珀棕、浅米色与低饱和灰绿色调，背景高度虚化，仅在面部两侧露出少量模糊色块，不出现可辨识的环境细节。<br>
<br>
呈现复古胶片影像截帧质感，低至中等反差，柔和高光，细微颗粒，轻微褪色与柔焦效果，保留眼神与皮肤的真实细节。影像边缘略带柔化，无文字、无水印、无标志。<br>
<br>
参数：整体画幅比例约16:9；内部影像比例约7:5；景别为面部极近特写；镜头焦距85—105mm；光圈f/2.0—f/2.8；浅景深；焦点位于画面左侧眼睛；暖色白平衡；低饱和度；柔和对比；细颗粒胶片质感；发丝轻微动态模糊；自然皮肤纹理；避免过度磨皮、过度锐化及高强度美颜。</blockquote>

#### 老手机随手拍

<p align="center"><img src="assets/showcase/iphone7-snapshot.jpg" alt="老手机随手拍" width="100%"></p>

<blockquote>一张用 iPhone 7 后置摄像头拍的照片，横拿手机，默认相机模式直出，没有美颜、没有滤镜、没有后期修图，就像2017年去贵州黔东南苗寨旅行的人，清晨路过一户人家的廊下，顺手拍下的照片。<br>
<br>
【画面】<br>
清晨的苗寨，山间还有薄雾。一位七十岁左右的苗族阿婆坐在自家木头吊脚楼的廊下，低头专心刺绣，膝上摊着一块靛蓝底的绣片，上面是红、橙、绿色的苗绣纹样，手里捏着针线。她穿着日常的深靛蓝色上衣，衣袖和领口有手绣的花边，头发盘成高髻，插着一把木梳，耳朵上戴着旧银耳环。脸上有皱纹，皮肤被太阳晒得黝黑，神情平静专注，没有注意到镜头。<br>
她身边的木凳上放着竹编针线篓和几团彩线，身后是被熏黑的木板墙，墙上挂着几串晒干的玉米和辣椒，墙角有一个塑料水桶和一双胶鞋。廊外远处，雾气里是层层叠叠的黑瓦吊脚楼和梯田。<br>
<br>
【真实感】<br>
阿婆是真实的普通村民，日常干活时的样子，不是穿盛装的模特。皮肤、手和衣服都是生活里自然的样子，不刻意强调瑕疵。<br>
<br>
【iPhone 7 的拍摄质感】<br>
1200万像素、28mm 等效广角、f/1.8 光圈的手机单摄。白天光线下画面干净清晰，主体锐利，细节够用但不过分锐化。景深较深，背景只有很轻微的柔化，没有人像模式虚化。颜色是那一代 iPhone 自然、略偏暖、饱和度适中的直出色彩，肤色真实。动态范围有限：廊外的雾和天空偏亮、略微过曝，廊下的暗部偏暗、保留一点细颗粒噪点，没有现代手机那种强烈的 HDR 提亮和算法涂抹。构图是随手拍的，阿婆偏左，画面略微倾斜。不是单反、不是专业摄影、不是电影感，不是CG、不是插画，是一张真实、清楚、自然的老款 iPhone 照片。</blockquote>

#### 直闪胶片人像

<p align="center"><img src="assets/showcase/flash-film-portrait.jpg" alt="直闪胶片人像" width="520"></p>

<blockquote>一张复古梦幻的直闪胶片时装肖像，3:4竖幅。<br>
一位二十岁左右的年轻女性，皮肤白皙，深棕色短卷发，刘海微卷，五官立体清秀。她戴一顶亮黄琥珀色半透明欧根纱宽檐软帽，帽檐柔软起伏，两条同色长纱带在下巴处打结，其中一条被风扬起，飘向画面右侧并遮挡部分画面；穿淡粉紫色抹胸裙，有半透明褶皱纱质纹理；颈间戴一条细金链，挂着一枚椭圆形浮雕金色古董徽章吊坠，边缘镶一圈小珍珠。<br>
身体微侧，头部正对略偏，眼神沉静冷淡、放空望向前方，嘴唇微张，疏离内敛。户外园林背景，模糊的绿树、草坪和浅色小路，略带布景感。中近景肖像，人物偏左下，右侧留给扬起的黄色纱带，平视机位。<br>
正面直打闪光灯，硬光，面部高光明显，背景略暗；色温中性偏暖。色盘：亮黄（主色）、淡粉紫、森林绿、苍白肤色与金色。35mm胶片质感，明显颗粒，中等景深，背景轻度虚化。复古、梦幻、前卫、略带忧郁与疏离。单张照片，无文字、水印和边框。</blockquote>

#### 奶奶的生日，家用 DV

<p align="center"><img src="assets/showcase/grandma-birthday-dv.jpg" alt="奶奶的生日，家用 DV" width="100%"></p>

<blockquote>普通旧式居民楼的客厅里，一位六十多岁的中国奶奶穿着日常碎花家居衫，俯身准备吹一个小蛋糕上的几根蜡烛，刚好闭了一下眼睛，带着笑意。矮茶几有花生壳、一个搪瓷杯和皱巴巴的蛋糕纸盒，一只小白狗从画面右下角把鼻子探向蛋糕。背景是碎花沙发、立式电风扇和一台只露出模糊亮光的旧电视。近距离平视手持，奶奶偏在左侧，靠近镜头的椅背挡住一角。主要光线是偏绿的顶灯与橙黄的烛光，屋内暗部略脏，烛火有小小光晕，不是精心策划的生日写真，而是家人突然按下录制键的一瞬间。<br>
<br>
画面像2001年前后普通家用MiniDV摄像机的真实生活录像截帧，横向4:3，未经修饰的私人录像感。小尺寸CCD成像，标准清晰度的柔软细节，阴影有细小彩色数字噪点，轻微色彩溢出和压缩痕迹，自动白平衡有一点偏色，亮处允许过曝，人物运动处有自然的轻微拖影；即使输出为大图也保留原始低清的信息密度。手持机位略歪，构图有偶然遮挡和边缘裁切，深景深，现场环境真实可辨。不要精致电影布光、胶片颗粒滤镜、模拟VHS横纹、夸张漏光、皮肤磨皮、商业摆拍或CG渲染感。画面铺满画布，不加边框、日期时间、录制标志、字幕、水印。只生成一张完整照片。</blockquote>

#### 黄昏屋顶

<p align="center"><img src="assets/showcase/rooftop-bedsheets.jpg" alt="黄昏屋顶" width="100%"></p>

<blockquote>夏末黄昏的旧城市屋顶，几根晾衣绳横跨前景，白床单被风吹起形成柔软的波浪，床单间隙露出远处密集的屋顶、天线和一轮低悬的淡金色月亮；逆光中一位穿白衬衫的人站在右侧收衣服，只保留清晰的侧面轮廓，屋顶水泥表面有暖灰纹理和浅浅积水，天空从玫瑰粉过渡到烟紫，夕阳边缘光穿过织物，画面有生活纪录片的真实和电影静帧的构图诗意，35mm镜头、自然风、轻微胶片颗粒，不要浪漫滤镜过重。<br>
真实摄影与电影静帧质感，优先自然光和可信的物理反射，构图有明确视觉重心与呼吸空间，色彩克制但有一到两个叙事性点色，材质细腻真实，人物动作自然，保留适度35mm胶片颗粒、柔和高光晕染和真实景深；画面高级、耐看、具有叙事瞬间，不要廉价CG感，不要塑料皮肤，不要过度锐化，不要HDR光晕，不要随机添加物件，不要水印、边框、logo或多余文字。</blockquote>

#### 喝茶前的停顿

<p align="center"><img src="assets/showcase/tea-portrait.jpg" alt="喝茶前的停顿" width="100%"></p>

<blockquote>拍摄一位卷发人物喝茶前停顿的真实肖像，头部、肩膀、上胸和双手捧着的深色陶杯入镜，人物略微侧脸。画面右后方的暖色灯光掠过头发，背景是较暗的室内墙面。松散卷发外缘和几根翘起的碎发被照得透亮，发丝之间仍能看见暗背景；浓密发束的内部保持深色，亮边随着发束遮挡自然中断。脸部由相机左前方很弱的柔光照亮，能看清眼睛、面颊和手指。耳廓与肩部只在朝向后侧灯光的边缘受光，陶杯呈宽而弱的表面亮部，杯沿和手指交接处保留接触阴影。焦点覆盖眼睛、外缘发丝与杯口。</blockquote>

#### 清晨火烈鸟

<p align="center"><img src="assets/showcase/flamingo-salt-lake.jpg" alt="清晨火烈鸟" width="100%"></p>

<blockquote>清晨盐湖浅水区，五只火烈鸟分散在宽阔的镜面水面上，最前景一只低头觅食，第二只单腿站立，远处三只形成柔和的粉色节奏，湖面倒映淡粉天空和远处白色盐壳；采用长焦平视构图，水面几乎占据整个画面，鸟群之间留出足够呼吸空间，羽毛粉色从灰粉到珊瑚粉有细腻层次，水纹、倒影、盐壳和鸟腿真实，优雅自然摄影，不要拥挤鸟群，不要高饱和卡通色。<br>
真实摄影与电影静帧质感，优先自然光和可信的物理反射，构图有明确视觉重心与呼吸空间，色彩克制但有一到两个叙事性点色，材质细腻真实，人物动作自然，保留适度35mm胶片颗粒、柔和高光晕染和真实景深；画面高级、耐看、具有叙事瞬间，不要廉价CG感，不要塑料皮肤，不要过度锐化，不要HDR光晕，不要随机添加物件，不要水印、边框、logo或多余文字。</blockquote>

### 超现实世界

#### 理发椅上的云

<p align="center"><img src="assets/showcase/surreal-cloud-barber-chair.jpg" alt="理发椅上的云" width="100%"></p>

<blockquote>一张复古、俏皮又高级的超现实时尚摄影。鲜绿色的山丘上摆着一张樱桃红色理发椅，一团巨大的白云坐在椅子里，蓬松的云体被薄荷绿色理发围布围住。一位成年女模特穿淡紫色短袖衬衫、深紫色铅笔裙和白色长靴，站在椅子旁，认真地用一把银色剪刀修剪白云，另一只手托起云朵的一角。剪下的小团云絮散落在草坪上，像刚剪落的头发。模特留利落的复古短发，神情专注。低机位广角构图，蓝天占据大半画面，布景简洁而色彩鲜明。真人时装大片质感，云朵有柔软半透明的细节与可信的体积阴影，轻微直闪补光，胶片颗粒，无卡通感。横向16:9，无文字。</blockquote>

#### 切月亮

<p align="center"><img src="assets/showcase/surreal-long-table.jpg" alt="切月亮" width="100%"></p>

<blockquote>一张具有复古电影布景质感的超现实时尚摄影。钴蓝色暮光天空下，绿色山丘上摆着一张铺白色桌布的长餐桌。一位成年女模特穿番茄红色丝绒长裙和白色长手套，神情冷静地站在桌子一侧，用银色餐刀从餐盘里的巨大满月上切下一小块楔形月亮。满月如圆形蛋糕般立在盘中，表面保留真实的陨石坑，切口内部散发柔和的乳白色光芒，切下的月亮块稳稳落在旁边的小瓷盘上。月光照亮她的手套与下颌，桌上玻璃杯投下细长阴影。空中的天空没有第二个月亮，远处只有一棵孤独的小树。优雅、荒诞、略带冷幽默，真实人物和实体道具摄影质感，细腻胶片颗粒，横向16:9，无文字。</blockquote>

#### 梨子更衣室

<p align="center"><img src="assets/showcase/surreal-pear-dressing-room.jpg" alt="梨子更衣室" width="100%"></p>

<blockquote>一张2000年代先锋时尚杂志的超现实摄影。浅粉色摄影棚里，一颗三米高的黄绿色梨子被改造成更衣室，梨皮上开出一道圆角小门，门板仍保留厚实的果皮与乳白色果肉切面。一位成年女模特正从梨子里迈出一只脚，穿巧克力棕色缎面连衣裙、浅蓝色连裤袜与尖头鞋，一只手扶着门边，另一只手整理耳环，表情漫不经心。梨子内部铺着酒红色丝绒软垫，挂着两件精致衣服。旁边一把小巧的银色椅子上放着普通大小的梨，形成明确的尺度对照。构图偏心，留出干净空间，柔和棚灯配合轻微正面闪光。果皮毛孔、水分充足的果肉、丝绒与缎面均有可触摸的真实质感，精心搭建的实体布景观感。横向16:9，无文字。</blockquote>

#### 剪纸拼贴

<p align="center"><img src="assets/showcase/blue-collage.jpg" alt="剪纸拼贴" width="520"></p>

<blockquote>3:4竖版抽象拼贴，融合旧时装杂志摄影、手工剪纸与街头海报印刷质感。浓郁钴蓝纸底占约三分之二，右上留白。偏右放置黑白胶片成年女性全身剪像，背对镜头、微向右倾，穿宽肩短夹克与宽松长裤，保留粗颗粒、深黑阴影及不规则细白纸边。沿人物轮廓叠加向左错位的纯橘红剪影，无五官服饰细节，脚下横置短厚炭黑纸片。左边缘窄撕纸带露出米白底纸与褪色照片碎片。真实剪口、纸纤维、油墨不匀与复印网点，平整高清扫描质感，简洁有力，无文字、标志、画框及场景展示。</blockquote>

#### 贴纸残迹字体海报

<p align="center"><img src="assets/showcase/sticker-type-poster.jpg" alt="贴纸残迹字体海报" width="520"></p>

<blockquote>“贴纸离开之后”实验字体海报，3:4竖版。上55%为冷灰蓝旧金属柜门微距，残留透明胶带、乳白撕纸、荧光橙标签与翻卷银膜，点缀残缺蓝花和橙星，柔和侧光突出纤维、残胶与磨损。<br>
下45%为纯白底，以材料自身轮廓拼出小写“residue”，宽约90%。字母融合橙色纸边、半透明胶膜与银膜，d长竖最高；高低错落、粗细各异，清晰可读，禁止标准字体填图。疏落点缀蓝银纸星、蓝胶带与半撕橙花。少量淡铅笔线配微小注记“peel”“trace”“02”、短箭头及未完成星形。真实摄影与手工拼贴质感，俏皮克制、留白充足，无厚重3D、额外文字及水印。</blockquote>

#### 像素白猫海报

<p align="center"><img src="assets/showcase/pixel-white-cat.jpg" alt="像素白猫海报" width="520"></p>

<blockquote>生成一张钴蓝色背景的实验性像素艺术海报。主体是一只白猫的侧脸，朝向画面左侧，耳朵竖起，眼睛半闭，神情冷淡。猫的轮廓由大小不一、边缘硬直的白色、浅灰色和淡粉色方块拼成：眼睛、鼻尖和部分胡须保留少量真实摄影细节，脸颊被中等像素块概括，后脑勺逐渐分解成更大的半透明方格。不同区域形成清楚的像素尺度变化。<br>
部分方格内部填有细小等宽字母与数字，呈现图像被程序分区采样和量化的效果。左下角放置一个小型荧光黄色矩形，其中排入黑色像素字体“PIXEL CAT”。构图偏置，保留大块蓝色空白；具有复古印刷颗粒、轻微套色偏移和低分辨率屏幕质感。整体是平面的数字拼贴海报，方格参与塑造猫的形体，无立体卡通角色，无水印。</blockquote>

### 艺术世界

#### 鸳鸯，古典大师油画

<p align="center"><img src="assets/showcase/baroque-mandarin-ducks.jpg" alt="鸳鸯，古典大师油画" width="520"></p>

<blockquote>一幅17世纪欧洲古典大师风格的布面油画，题材是中国的鸳鸯与荷塘。画面中央，一对鸳鸯在幽暗的荷塘水面上相依而游：雄鸳鸯羽色华丽，橙红色帆状饰羽、带紫绿金属光泽的头冠、白色眉纹、红色的喙；雌鸳鸯灰褐素雅，眼后一道白纹。两只鸳鸯头颈微微相靠，神态安静深情。四周是夏末初秋的荷叶，有的饱满墨绿，有的边缘焦枯卷曲，右上方一枝半开的粉白荷花和一个低垂的莲蓬。伦勃朗式明暗对照光，一束温暖的侧光从左上方落在鸳鸯身上，其余部分沉入深橄榄绿与琥珀棕的暗部。水面像一面墨色的镜子，倒映着鸳鸯与荷花，泛起细小的涟漪。厚涂与薄罩染结合，羽毛高光处颜料堆起，能看到清晰的笔触和画布纹理，古旧清漆带来温暖的金色调和细微的龟裂。构图稳重，留有大片暗部的呼吸空间，诗意、静谧，博物馆级杰作。</blockquote>

#### 渔夫与鹈鹕，卡拉瓦乔风格

<p align="center"><img src="assets/showcase/caravaggio-pelican.jpg" alt="渔夫与鹈鹕，卡拉瓦乔风格" width="100%"></p>

<blockquote>Oil painting in the style of Caravaggio, dramatic chiaroscuro, dark background. Two old fishermen in ragged clothes pull a wet fishing net out of a wooden boat. A pelican is caught in the net, its beak and one wing poking out through the holes as it struggles. The rope mesh wraps around its body and stretches tight between the fishermen's hands. A single beam of light from the upper left falls on the pelican's white feathers and the men's faces.</blockquote>

#### 乒乓球赛，卡拉瓦乔风格

<p align="center"><img src="assets/showcase/caravaggio-ping-pong.jpg" alt="乒乓球赛，卡拉瓦乔风格" width="100%"></p>

<blockquote>卡拉瓦乔油画，一群十七世纪意大利市民正在现代乒乓球馆进行单打比赛与观赛。六人均保留巴洛克时代的面貌、自然卷发与粗麻衬衣，身着褐色短上衣、羊毛披风、束腰长裙或及膝裤与皮靴，没有现代运动装。球台沿画面下方向右后方斜切，清晰呈现绿色台面、白色边线、绷紧的中央球网与两支胶面球拍；一颗小白球越网弹向近处。近侧红褐短衣青年俯身跨步迎球挥拍，对面白衬衣男子压低重心准备下一次回击，动作彼此呼应。左前老妇攥住披风边缘，身后少女越过她肩头追看球路，右后两名男子一人按住椅背前倾、一人抬手示意比分，遮挡形成远近层次。唯一主光自左上高窗侧入，集中照亮击球者颧骨、前臂与白球，观众面孔逐层沉入暖褐暗处。真实肉色、乳白、赭红统摄色彩，木地板与哑光涂层台面各有质感；以细腻转折塑造手指与衣褶，薄层罩染并克制提亮，保持复杂多人叙事油画的重量，避免统一粗厚纹理、龟裂滤镜和摄影感。</blockquote>

#### 苏州园林鸳鸯，印象派油画

<p align="center"><img src="assets/showcase/impressionist-suzhou-garden.jpg" alt="苏州园林鸳鸯，印象派油画" width="520"></p>

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

#### 太阳，中世纪泥金手抄本

<p align="center"><img src="assets/showcase/illuminated-manuscript-a.jpg" alt="太阳，中世纪泥金手抄本" width="520"></p>

<blockquote>A medieval illuminated manuscript illustration with gold leaf and a wide border of curling vines. A rooster in a short red cloak stands upon a stone platform above a sleeping town. It grips a thick cord in its beak and leans backward with its whole body, pulling open a heavy dark blue curtain that covers the sky. Behind the lifted curtain appears a great golden sun with a calm human face. Below, small red roofs, a church tower and a few open windows mark the town beginning to wake. The rooster’s feet are firmly planted, its effort shown through its awkward, determined posture.<br>
<br>
Flat perspective, dark ink outlines, opaque tempera on aged parchment. Rich red, ultramarine blue and gold. A broad blue border filled with curling gold foliage and red blossoms. Worn gilding and slightly irregular hand-painted forms. A small numeral XIX above, and THE SUN in a parchment cartouche below.</blockquote>

#### 玉兔，中世纪泥金手抄本

<p align="center"><img src="assets/showcase/illuminated-manuscript-b.jpg" alt="玉兔，中世纪泥金手抄本" width="520"></p>

<blockquote>A medieval illuminated manuscript illustration with gold leaf and a wide border of curling vines. Beneath an old osmanthus tree, the Jade Rabbit of Chinese folklore stands beside a blue-grey stone mortar. Wearing a simple red cloth sash, it grips a long jade pestle and carefully grinds a single ivory crescent moon into fine golden powder. Part of the crescent remains intact inside the mortar. Small osmanthus blossoms fall onto the stone rim, and several folded medicine packets lie nearby. The rabbit works with the solemn concentration of an old apothecary. The deep blue sky contains a few stars but no second moon.<br>
Flat perspective, dark ink outlines, opaque tempera on aged parchment. Rich red, ultramarine blue and antique gold. A broad blue border filled with curling gold lotus vines, small blossoms and Chinese cloud motifs. Worn gold leaf and slightly irregular hand-painted forms. A small numeral XVIII above, and THE MOON in a parchment cartouche below.</blockquote>

#### 空间站维修，敦煌壁画

<p align="center"><img src="assets/showcase/dunhuang-space-station.jpg" alt="空间站维修，敦煌壁画" width="100%"></p>

<blockquote>把现代空间站舱外维修转译为敦煌唐代矿物重彩土壁壁画，画面是平面壁绘，不是太空电影。中央一位飞天形貌的维修者侧身伸向太阳能板转轴，宽袖外叠着简化的现代安全背心，长飘带在身后绕成两段流畅弧线；左下同伴将一件工具递向主角，右上另一人扶住折起的太阳能板，三人的手眼都指向同一转轴。安全绳以清楚细线连接人物与舱壁，飘带与安全绳各有路径，不能合为杂乱细线。空间站舱体是赭白色圆筒与几块几何平面，太阳能板以石青小格表现，可辨现代设施，但不用光滑金属与真实太空光照。人物面容和衣褶用唐代壁画式线描，身体轮廓轻盈，叠压关系代替精密透视，侧面地球画成一枚低饱和石绿圆盘，背景仍是土壁赭色与少数传统卷云、星点。朱砂、石青、石绿和温白彼此制约，色层有矿物颗粒与轻微自然磨损，局部露出墙底而非全幅统一裂纹滤镜。画面动势由飘带、板翼与圆筒共同组织，主角大、协作者略小，有纸白般的空壁呼吸。不画科幻盔甲、蓝色体积光、摄影星空、字幕和商标，无题款与印章。</blockquote>

#### 鹈鹕皮影戏

<p align="center"><img src="assets/showcase/shadow-puppet-pelican.jpg" alt="鹈鹕皮影戏" width="100%"></p>

<blockquote>中国传统皮影戏，背后的油灯把米黄色布幕照得发亮。幕布上是一只彩色半透明的皮影鹈鹕，红色的喉囊里装着一条蓝色小鱼，身上刻着精细的镂空花纹。幕布上还能看到几根操纵杆的细影子，以及艺人两只手的模糊影子在操控。幕布外面是红色木框和流苏。</blockquote>

#### 电路与花，工笔织物纹样

<p align="center"><img src="assets/showcase/gongbi-circuit-textile.jpg" alt="电路与花，工笔织物纹样" width="600"></p>

<blockquote>设计一块可以上下左右连续拼接的现代织物纹样，以中国工笔绢本设色把电路板与植物组织融合：集成电路像花床，电阻形成纤长花梗，卷叶之间可见整齐焊点，小型甲虫沿铜箔线路爬行。构图采用有松有紧的散点组织，四边切出的枝线在对边准确接续，避免中心孤立的大团花。茄紫底色上配置灰绿、浅珊瑚与淡铜金，细密线描把芯片引脚、叶脉和甲壳分得清楚，分染罩染让叶片薄、甲壳润、线路平整，所有细节仍是手绘工笔。精确装饰线既维持电路的秩序，也形成自然生长的曲折。以均匀分布的小块净绢色负形让纹样呼吸，不另设题签或边框，远看节奏现代，近看材质丰富，可直接作为服装面料图案。</blockquote>

#### 照镜子的鹈鹕，工笔画

<p align="center"><img src="assets/showcase/gongbi-pelican-mirror.jpg" alt="照镜子的鹈鹕，工笔画" width="520"></p>

<blockquote>中国工笔画风格，绢本设色。古代闺房的梳妆台上立着一面圆形铜镜，一只白色鹈鹕站在镜前，低头用长嘴整理胸前的羽毛。铜镜表面偏黄、有点模糊，映出鹈鹕的正脸和它身后的雕花木窗。左上角有竖排题字和一枚红色印章。</blockquote>

#### 金色烈焰，东方幻想插画

<p align="center"><img src="assets/showcase/eastern-fantasy-lineart.jpg" alt="金色烈焰，东方幻想插画" width="100%"></p>

<blockquote>制作一张以金色烈焰和舞动妖灵为主题的东方幻想二次元插画。画风标签：#二次元插画 #东方幻想 #工笔重彩 #装饰性平涂 #精细线描 #金箔肌理。横向16:9，构图充满旋转动势：中央偏右是一位黑金卷发、头生短角的年轻男性，俯身扭转，脸朝左下方，宽大金色袖袍和红绳随动作翻飞；背后的大型圆形器物和弧形飘带沿右上至左下形成旋涡。左上安排浅金色长发妖灵侧身托起盛有金色液体的浅盘，左下与右前景再安排浅金色人形妖灵，珠串、长发、手臂和圆盘交错环绕中央人物。中央服装以金褐、朱红、墨绿叠搭，背景用朱橙色铺满，加入弯曲金边、喷溅酒液、火焰和烟云纹样。画风重点：将日系二次元人物造型与工笔重彩式细密线描结合，细长流动线条贯穿发丝、珠串和衣褶。以朱砂红、赭橙、古金的大块平涂为底，局部薄层罩染表现体积，保留纸张颗粒、金箔斑驳与传统装饰纹样，平面装饰感突出。画面不含文字、数字、字母、Logo、署名或水印。</blockquote>

