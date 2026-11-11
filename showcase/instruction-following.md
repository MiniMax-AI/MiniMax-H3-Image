<p align="center">
  <a href="instruction-following.md"><strong>English</strong></a> |
  <a href="instruction-following.zh-CN.md">简体中文</a> |
  <a href="instruction-following.ko.md">한국어</a> |
  <a href="instruction-following.ja.md">日本語</a>
</p>

# Precise Instruction Following and Understanding

The model understands the knowledge, structure, and presentation requirements in a prompt and organizes them into clear visuals.

← [Up to 16 Reference Images](multi-reference.md) · [Showcase](README.md) · [Complex Visual Challenges](visual-challenges.md) →

## Education, Science Communication, and Knowledge-Based Reasoning

### Biology figure from a paper page

<table><tr><td width="28%" valign="top"><img src="../assets/showcase/bio-figure-input.jpg" alt="Input"><br><sub>Input</sub></td><td width="72%" valign="top"><img src="../assets/showcase/bio-figure-output.jpg" alt="Biology figure from a paper page"><br><sub>Output</sub></td></tr></table>

<details>
<summary>Prompt</summary>
<blockquote>Based on the uploaded text page from an English-language paper, generate a publication-quality biological research figure in 16:9 landscape format at 4K. Organize it into three logically connected panels: the lighting experiment setup; a comparison of the seedlings' initial and final states with the angle definition; and a plot of time versus bending angle. Use simple, credible scientific renderings or academic schematics for the seedlings and growth apparatus, and keep the data plot accurate, clear, and restrained. Read the viewing direction, light-source position, morphological changes, angle definition, and data from the source text yourself, and keep them consistent across all panels. Use a white background, consistent typography, short English labels, and panel labels a–c, with the hierarchy and whitespace of a formal academic figure. Retain the label “synthetic study” and identify the visuals as schematics or renderings. Do not add control groups, molecular mechanism diagrams, error bars, or statistical conclusions absent from the original text.</blockquote>
</details>

### Red panda infographic

<p align="center"><img src="../assets/showcase/red-panda-infographic.jpg" alt="Red panda infographic" width="520"></p>

<details>
<summary>Prompt</summary>
<blockquote>Create a 2:3 portrait infographic in Chinese, with the exact Chinese title “读懂小熊猫” and subtitle “山地森林里的树栖生活家” (meaning “Understanding Red Pandas” and “Tree-Dwelling Specialists of Mountain Forests,” respectively). Use a dense animal field-guide style with flat vector illustrations, a pale lime background, dark pine-green text, terracotta-orange bodies, and creamy-white facial markings. Place a dark rounded title bar at the top, followed by a profile, scale bars, a distribution map, and behavioral icons. A central red panda should occupy about one quarter of the composition, standing sideways on a branch and looking back, with its ringed tail hanging naturally toward the lower right and accurate proportions. Arrange detail illustrations and annotations on both sides, with a continuous information strip along the bottom, keeping the entire panel visually consistent.<br>
Include all 14 knowledge groups below, each with a heading, 3–5 short facts, and illustrations:<br>
01 Identity: Class Mammalia, order Carnivora, family Ailuridae; use silhouettes to distinguish it from giant panda cubs and raccoons.<br>
02 Size: Head-and-body length approximately 56–62.5 cm, excluding the tail; tail length approximately 37–47 cm. Use two scale bars and note individual variation.<br>
03 Face: Round head, short muzzle, pointed ears, pale face with dark tear markings, and dark legs and belly; include close-up windows.<br>
04 Fur: Long guard hairs, dense underfur, and fur on the soles; compare its colors with a moss-and-lichen environment.<br>
05 Grip: Five toes on each foot and partially retractile claws; the false thumb is a specialized wrist bone that helps it grasp bamboo.<br>
06 Tail: Ringed pattern, balance, and wrapping around the body for warmth; it cannot coil around a branch to support body weight.<br>
07 Climbing: Rests and takes refuge in trees, grips trunks with its claws, and uses flexible ankles to descend headfirst.<br>
08 Diet: Mainly bamboo leaves and tender shoots, with fruit and insects as well; do not invent dietary percentages.<br>
09 Eating Bamboo: Forepaws hold the branch, the mouth selects tender leaves, and molars chew them; include a three-step diagram.<br>
10 Habitat: Suitable mountain regions in Nepal, India, Bhutan, China, and Myanmar; include a regional distribution map and illustrations of forests, bamboo thickets, and water sources.<br>
11 Activity: Active around dawn and dusk; rests in trees when hot, curls up when cold, and stretches out when warm. Do not invent an exact daily timetable.<br>
12 Communication: Mostly solitary; communicates through scent, calls, and posture.<br>
13 Development: Builds nests in secluded places; newborns have closed eyes, nurse from the mother, and gradually begin exploring. Include a four-stage diagram.<br>
14 Conservation: Forest loss and fragmentation, poaching and trade, and free-roaming dogs; pair these with habitat protection, patrols and monitoring, and community participation.<br>
Include at least 40 substantive facts and approximately 25 supporting illustrations. Keep forms and line weights consistent, organizing the content through numbering, alignment, and thin dividers. Avoid repetitive cards, large empty areas, and crossing leader lines. Maintain a clear Chinese text hierarchy with no garbled characters, repetitive filler, or invented data. Footer sources: Smithsonian National Zoo, San Diego Zoo Wildlife Alliance, Red Panda Network. Output a complete flat display panel, not a mockup.</blockquote>
</details>

### Staff-selection puzzle

<p align="center"><img src="../assets/showcase/staffing-logic-puzzle.jpg" alt="Staff-selection puzzle" width="100%"></p>

<details>
<summary>Prompt</summary>
<blockquote>Solve the following personnel-selection reasoning problem and generate a visual explanation. Use 16:9 landscape format, a white background, and clear, standardized Chinese typography.<br>
An organization must select exactly three of six staff members—甲, 乙, 丙, 丁, 戊, and 己—for a research team. All of the following conditions must be met:<br>
If 甲 is selected, 乙 must also be selected.<br>
Exactly one of 丙 and 丁 must be selected.<br>
乙 and 戊 cannot both be selected.<br>
If 己 is selected, 丙 must also be selected.<br>
戊 has already been confirmed as selected.<br>
Determine the three-person team using all the conditions.<br>
Show the problem conditions at the top. Divide the lower section into “入选” (Selected) and “未入选” (Not Selected), placing each of the six staff cards in the correct area. Each card should contain a person icon and a prominent name label. Each person must appear exactly once, with no duplicates or omissions.<br>
At the bottom, use brief notes to show the key reasons for exclusion. The card placements, selected names, and notes must agree. Do not add extra conditions. Output only the finished solution image.</blockquote>
</details>

## Industrial and Product Design

### Electric motorcycle, exploded view

<table><tr><td width="50%" valign="top"><img src="../assets/showcase/e-motorcycle-input.jpg" alt="Input"><br><sub>Input</sub></td><td width="50%" valign="top"><img src="../assets/showcase/e-motorcycle-exploded.jpg" alt="Electric motorcycle, exploded view"><br><sub>Output</sub></td></tr></table>

<details>
<summary>Prompt</summary>
<blockquote>Disassemble the concept electric motorcycle in image 1 into a highly detailed exploded parts diagram, keeping its form, white geometric bodywork, metallic-gray motor, hubless wheels, and orange-red light strips consistent with image 1.<br>
<br>
Disassembly layout: Use an isometric view centered on the motor unit, with all parts radiating outward along their respective assembly directions, clearly spaced and without overlap:<br>
- Front: Split the front fairing into upper and lower sections. Separate the headlight strip, windshield, front fork, hubless front rim, tire, annular bearing inside the rim, and brake disc.<br>
- Middle: Split the white geometric frame shell into multiple faceted panels on both sides, revealing the tubular main frame. Separate the motor housing, cooling fins, stator, rotor, and motor controller. Pull the battery pack out separately, placing the battery modules and wiring harness beside it.<br>
- Rear: Separate the seat assembly into cushion and base, followed by the rear swingarm, rear shock absorber, rear rim, tire, and taillight strip.<br>
- Small parts: Group bolts, washers, clips, bearings, and connectors beside their corresponding components according to their installation positions, with fine dashed lines leading back to the mounting points.<br>
- Add two circular magnified insets showing the bearing structure of the hubless rim and the stator windings inside the motor.<br>
<br>
Text annotations: Connect every major component to an ALL-CAPS English label using a thin white leader line with a small dot at its endpoint. Text must be legible and correctly spelled, with labels arranged neatly along the edges.<br>
<br>
Use a dark-gray background with faint isometric grid lines, soft even lighting, and clean highlights along the component edges. The composition should be full, clearly layered, and orderly, resembling a structural breakdown from a professional industrial design firm.</blockquote>
</details>

### Jet engine, exploded view

<table><tr><td width="50%" valign="top"><img src="../assets/showcase/jet-engine-input.jpg" alt="Input"><br><sub>Input</sub></td><td width="50%" valign="top"><img src="../assets/showcase/jet-engine-exploded.jpg" alt="Jet engine, exploded view"><br><sub>Output</sub></td></tr></table>

<details>
<summary>Prompt</summary>
<blockquote>Turn the jet engine in image 1 into a high-precision exploded structural rendering. Use a solid dark-gray background and an oblique overhead isometric view, with components floating apart along a diagonal axis from the upper right to the lower left: intake cowling, compressor blade discs, combustion chamber, turbine discs, central shaft, and exhaust nozzle in sequence. Divide the engine casing into curved panels suspended around the main shaft; distribute the electronic control box, fuel pump, accessory gears, fuel lines, and copper-colored wiring harnesses on either side. Use cool gray, silver, and matte white for the outer shell and casing, with warm gold and bronze for the turbine core and shaft. Keep components aligned and evenly spaced, with soft studio lighting and realistic metallic reflections. Connect major components to both sides of the image with thin white leader lines and label them in Chinese: “进气罩,” “压气机叶片盘,” “燃烧室,” “涡轮盘,” “中心主轴,” “尾喷管,” “机匣外壳,” “电子控制单元,” “燃油泵,” “附件齿轮箱,” and “燃油管路” (intake cowling, compressor blade discs, combustion chamber, turbine discs, central shaft, exhaust nozzle, engine casing, electronic control unit, fuel pump, accessory gearbox, and fuel lines, respectively). Use small, simple white sans-serif text in two neat columns, with leader lines that neither cross nor obscure components. Portrait 2:3, with no branding.</blockquote>
</details>

### Moka pot blueprint

<table><tr><td width="39%" valign="top"><img src="../assets/showcase/moka-pot-input.jpg" alt="Image 1"><br><sub>Image 1</sub><br><img src="../assets/showcase/moka-pot-parts-input.jpg" alt="Image 2"><br><sub>Image 2</sub></td><td width="61%" valign="top"><img src="../assets/showcase/moka-pot-blueprint.jpg" alt="Moka pot blueprint"><br><sub>Output</sub></td></tr></table>

<details>
<summary>Prompt</summary>
<blockquote>Turn the octagonal moka pot in image 1 into a classic engineering blueprint poster, using image 2 as the reference for its component structure. Use a dark-blue background with a light grid, and render all graphics as white line drawings with a slightly weathered grain. Center the uppercase title “MOKA POT” at the top. Arrange an exploded view of the components vertically on the left: lid with small Bakelite knob, upper chamber with handle, stainless-steel filter screen, rubber gasket, funnel filter basket, and lower chamber with safety pressure-release valve. Place a larger cross-section at the upper right showing the internal water path and coffee chamber, and smaller top and side views at the lower right. Include dimension lines, leader lines, and letter labels throughout. Portrait 3:4, with a technical-drawing layout.</blockquote>
</details>

### Ant-inspired hexapod mech, line art

<p align="center"><img src="../assets/showcase/ant-hexapod-mech-lineart.jpg" alt="Ant-inspired hexapod mech, line art" width="100%"></p>

<details>
<summary>Prompt</summary>
<blockquote>A hand-drawn line-art industrial concept design board for a sci-fi biomimetic six-legged heavy mech, in a wide landscape composition on a pure white background. The subject is a giant mechanical walking platform designed after the body structure of an ant, seen in a front-left three-quarter view from slightly above. The mech's head points to the lower left, while its torso and tall rear pod extend to the back right; its six mechanical legs spread out to both sides in a stable, imposing stance. The subject occupies the lower middle of the image; the blank space at the top and around it holds separate component line drawings, biomimetic structure sketches, handwritten notes, and curved pointer arrows, forming the complete layout of a game mech design sheet.<br>
<br>
The silhouette clearly separates three masses: a low head, a connecting thorax, and a heavy abdomen. The head is flat, wedge-shaped armor with a narrow blue-cyan optical viewport at the front and small sensors and round mechanical ports on both sides; the back is covered by two mustard-yellow module boxes with reinforcing ribs, latches, segmented cover plates, and dark-gray mounting frames. Below and in front of the head hang two long, slender fictional sci-fi devices side by side, with dark-gray bodies and exposed orange-yellow brackets, pointing diagonally to the lower left; curved, segmented metal chain belts hang from the boxes above and connect to the components below, forming clear layers of arcs. The midsection narrows slightly, leaving visible space for black hoses, load-bearing frames, and internal linkages.<br>
<br>
The six mechanical legs have insect-like multi-segment joints and thick industrial armor: the heavy upper limbs stretch out diagonally, the slender lower limbs support the ground, and each ends in a low, wide, segmented mechanical foot. Every leg includes large round pivots, layered guard plates, hydraulic rods, pistons, joint stops, and exposed wiring; the legs in the foreground are larger, and those in the background are partly hidden by the body, with clear perspective and depth. The abdominal pod at the upper right of the body is tall and heavy, built from slanted polygonal armor plates, with a worn white number "02" on its side, rectangular maintenance hatches, cooling vents, bolts, and two small red cylindrical canisters; the underside of the abdomen is dense with mechanical framework and connecting pipes.<br>
<br>
Several fictional equipment modules are mounted on top of the abdomen: a horizontal group of rectangular box components with four dark-red round end caps lined up at the left end; next to it, a disc-shaped detector, a thin antenna, pairs of small upright sensor rods, teal indicator lights, and clusters of short tubular parts set at an angle. A short, thick, horizontal cylindrical sensor extends from the front of the top, its front end made of several square, colored optical lenses. All attached equipment keeps a unified military-green industrial look, with varied joints and bracket shapes, but serves only as a sci-fi exterior design display; show no firing, explosions, or combat.<br>
<br>
At the upper left, lay out horizontally a very long, thin black-and-white line drawing of a twin-rail sci-fi device, with a complex box, cables, and cylindrical modules at its right end and a straight, narrow rail extending to the left. In the upper middle of the left side, place a perspective line drawing of a short, thick multi-barrel component, and in the upper center a separate line drawing of a rectangular storage box, with freely curving black arrows pointing to the matching places on the subject. In the upper right corner, draw a side-view sketch of an ant, summarizing the head, thorax, and abdomen with simple black lines and labeled with the light-red numbers "1, 2, 3"; right of center at the bottom, keep a loose black sketch of a biomimetic six-legged structure, showing the link between the mech and the insect form. A few small handwritten notes serve as supporting design annotations, avoiding large areas of text that would distract from the subject.<br>
<br>
The whole piece is a pure hand-drawn line-art design sheet: all structures are outlined in thin, slightly shaky black ink lines of varying density, keeping a few doubled lines, broken lines, and exploratory strokes that do not fully close. Apart from tiny spots of pale color, use no thick painted textures, do no realistic rendering, and show no specular highlights, light flares, gradient volume, or photographic texture. The main mech uses line art with very light flat gray tones: most armor surfaces are left white, and only the shaded sides and structural gaps use light-gray and mid-gray blocks with occasional pure-black shadows to describe the turns, while armor seams, bolts, hydraulic rods, pistons, exposed wiring, cable bundles, and other internal mechanical details are all drawn precisely with fine lines. The mustard-yellow module boxes, the orange-yellow exposed brackets, the two small red cylindrical canisters, and the teal indicator lights are suggested only by tiny spots of pale color, never by large color fills. A few short broken lines and dry-brush strokes along the armor edges suggest wear, without painted material textures. Almost no shadow is drawn under the body; only two or three very faint gray lines show where the feet meet the ground, and the edges of the canvas stay clean.<br>
<br>
The twin-rail device drawing at the upper left, the multi-barrel component perspective drawing on the left, the rectangular storage box drawing in the upper middle, and the biomimetic six-legged structure sketch at the lower right are all uncolored pure line art, in the same line language as the subject. The ant side-view sketch in the upper right corner also outlines the head, thorax, and abdomen in fine black lines, with light red used only for the labels "1, 2, 3". The curved pointer arrows and handwritten notes are casually sketched black lines, free and slightly irregular. A few small handwritten notes serve as supporting design annotations, avoiding large areas of text that would distract from the subject.<br>
<br>
Parameters: aspect ratio about 3:2, ultra-high definition, extremely crisp line art, clearly varied line weight, very low color saturation, medium-high black-and-white contrast, no cast shadows, no material rendering, no environment, no people, no extra decorative border.</blockquote>
</details>

## Robotics and Embodied Intelligence

### Quadruped mech, CAD drawing

<table><tr><td width="50%" valign="top"><img src="../assets/showcase/quadruped-mech-input.jpg" alt="Input"><br><sub>Input</sub></td><td width="50%" valign="top"><img src="../assets/showcase/quadruped-mech-cad.jpg" alt="Quadruped mech, CAD drawing"><br><sub>Output</sub></td></tr></table>

<details>
<summary>Prompt</summary>
<blockquote>Turn the quadruped mech in image 1 into a standardized CAD engineering drawing with multiple views. Use a white drawing-sheet background and fine black lines: solid lines for visible outlines, dashed lines for hidden structures, and dash-dot lines for axes of symmetry and joint centers.<br>
<br>
Include five neatly arranged views:<br>
- Upper left: Front view.<br>
- Upper right: Left-side view.<br>
- Middle left: Top view, clearly showing the launch-port arrays of both weapon pods and the spread angles of all four legs.<br>
- Middle right: Rear view.<br>
- Bottom: A larger isometric wireframe view showing the overall three-dimensional structure.<br>
<br>
Use the same scale across all views, keeping the shapes of the body, weapon pods, leg joints, and thigh armor plates consistent with image 1. Annotate the main dimensions: overall height, length, width, leg span, and weapon-pod dimensions. Use leader lines to label the key parts “武器舱,” “翻盖,” “机身,” “大腿装甲板,” “膝关节,” and “足部” (weapon pod, hatch, body, thigh armor plate, knee joint, and foot). Place a standard title block in the lower right reading “四足机甲 总装图 1:20” (Quadruped Mech — General Assembly — 1:20). Use clean, accurate lines and an orderly layout resembling a formal mechanical design drawing.</blockquote>
</details>

### Mech beast, exploded CAD view

<table><tr><td width="43%" valign="top"><img src="../assets/showcase/mech-monster-input.jpg" alt="Input"><br><sub>Input</sub></td><td width="57%" valign="top"><img src="../assets/showcase/mech-monster-exploded-cad.jpg" alt="Mech beast, exploded CAD view"><br><sub>Output</sub></td></tr></table>

<details>
<summary>Prompt</summary>
<blockquote>[Left Side Exploded View: Widely Spread, Fully Separated]<br>
<br>
The left side shows a fully spread mechanical assembly exploded view. Only the continuous internal load-bearing skeleton stays in the center; the head shell, chest and back armor, limb guard plates, joint end caps, back spikes, and tail scales move far from their mounting positions, forming a wide, orderly array of parts around the skeleton.<br>
<br>
The central skeleton takes up only about 45% of the width and 40% of the height of the left area; the complete group of exploded components covers about 90% of the width and 85% of the height of the left area. Leave enough space for the removed parts to show each part's full outline, thickness, inner reinforcing ribs, and mounting holes.<br>
<br>
[Clear Separation Distances]<br>
<br>
At least 80% of the external armor is completely detached from the skeleton. Each large armor piece moves away from its original mounting position by about 1 to 1.5 times its own width. Clearly visible white gaps separate the main parts; avoid guard plates that still touch the body with only a thin seam showing.<br>
<br>
Use three levels of separation distance:<br>
<br>
The outer armor moves farthest, forming the outer ring of parts; the middle-layer connecting brackets sit between the armor and the skeleton; internal bearings, connecting rings, washers, and fasteners spread out in order along their axes. Leave clear empty space between the layers so the assembly order can be read at a glance.<br>
<br>
[Separation Direction by Region]<br>
<br>
The head components spread toward the upper left: the forehead plate, the twin horn mounting modules, the cheek guards on both sides, the sensor module, and the jaw assembly each move away from the skull along their own assembly direction. Leave a large enough gap between the head shell and the internal frame to fully reveal the structure hidden inside the skull.<br>
<br>
The chest and back armor spread upward: the back spikes and scale armor, in their original front-to-back order, form two to three staggered layers of floating component bands above the skeleton. Each armor piece has its own outline, with white gaps between the pieces. The inner sides of the armor face the viewer, clearly showing reinforcing ribs, mounting seats, and screw holes.<br>
<br>
The chest side plates spread left and right: the outer armor moves to the outer ring, the rib-like brackets stay in the middle layer, and the central power module and mechanical spine stay at the center of the skeleton. Pipes and cables stay with the components they belong to, and the separated connectors are clearly visible.<br>
<br>
The limb components spread outward and downward: the front-limb armor is laid out in the lower left and the rear-limb armor in the lower right; guard plates, brackets, and joint assemblies each have their own space, avoiding dense stacks around the legs.<br>
<br>
The round joints are pulled out into long rows along their axes: end caps, locking rings, washers, bearings, and connecting flanges are arranged in order, with gaps of about 0.3 to 0.6 times the joint diameter between adjacent main parts; all rings are strictly coaxial, clearly showing each layer's thickness and the assembly order.<br>
<br>
The tail components spread toward the upper right: the central vertebra chain stays continuous, while the outer scale armor moves up and to the sides in groups, forming component bands parallel to the tail. The hooked blade at the tip of the tail is clearly detached from its mount, keeping a clear assembly axis.<br>
<br>
[Assembly Relationships and Readability]<br>
<br>
All removed parts keep their original proportions and mounting orientation and are connected to their positions by thin, clear dashed lines. Even with the larger separation distances, it should remain clear which body part each armor piece belongs to and how each joint group goes back together.<br>
<br>
Avoid main parts hiding each other, and keep the assembly guide lines as parallel as possible with few crossings. Screws and small fasteners are grouped near the components they belong to and do not fill the white space between the main parts.<br>
<br>
The final image should clearly show a bare mechanical beast skeleton in the center, surrounded by widely displaced, multi-layered armor and mechanical components, with wide, distinct, continuous white gaps between the parts. Keep the pure white background, the precise black CAD line art, and the assembled four views on the right.</blockquote>
</details>

### Ceiling rail courier

<p align="center"><img src="../assets/showcase/ceiling-rail-courier.jpg" alt="Ceiling rail courier" width="100%"></p>

<details>
<summary>Prompt</summary>
<blockquote>Create a 16:9 English engineering concept sheet titled "Ceiling Rail Courier," marked "Fictional indoor transport concept." Show a long side elevation across the upper half, a detailed suspended carriage at lower left, and a three-position storyboard at lower right. Use warm white paper and cobalt linework.<br>
A straight horizontal rail spans X = 0 to 2400 mm. Define three docking stations by carriage-center coordinates: A at X = 300, B at X = 1200, and C at X = 2100 mm. Adjacent station spacing is 900 mm. The carriage is 400 mm long along X, so its footprint at A is 100–500 mm and at C is 1900–2300 mm; all positions remain within the rail. The three storyboard panels show the same carriage at A, B, and C, not three simultaneous robots.<br>
At the illustrated extension, the vertical suspension comprises an 80 mm carriage housing, a 120 mm mounting bracket, a 300 mm telescoping stem, and a 60 mm gripper, measured as consecutive segments. Mark their total as 560 mm, measured from the housing top to the gripper bottom; rail, rollers and parcel are excluded from this dimension. The gripper holds one sealed parcel throughout all panels. Include two rail rollers, one linear drive unit, one downward camera, and one two-finger gripper in the component ledger. Maintain the same dimensions, parcel, roller count, and sensor position across all views. Clearly separate horizontal station dimensions from the vertical stack.</blockquote>
</details>

### Wheel-legged delivery robot

<p align="center"><img src="../assets/showcase/wheel-leg-robot.jpg" alt="Wheel-legged delivery robot" width="100%"></p>

<details>
<summary>Prompt</summary>
<blockquote>Draw a 16:9 concept diagram in Chinese of a wheeled-legged delivery robot. Include side views of the same robot standing and crouching, a 3D view, and an actuator-axis table, labeled “虚构结构研究” (Fictional Structural Study). The body is 500 mm long, 360 mm wide, and 180 mm high. Each of its four corners has a two-joint leg ending in a powered wheel 120 mm in diameter. There are eight leg joints and four wheel-axis motors, for a total of 12 controlled rotary axes. Label the legs FL, FR, RL, and RR, with upper and lower joints numbered 1 and 2 and wheel axes labeled W. Left and right are from the robot's own perspective. The top of the body is 560 mm above the ground when standing and 440 mm when crouching. Use the same ground line to show the 120 mm reduction. Change only the joint angles between the two views; keep the body, wheel diameters, and link lengths identical. There is only one depth camera on the front panel and only one enclosed cargo box above the body; keep the box level in both poses. Use a comparison table to distinguish the eight leg joints from the four powered wheel axes, avoiding any depiction of 12 controlled axes as 12 legs or 12 wheels.</blockquote>
</details>

---

← [Up to 16 Reference Images](multi-reference.md) · [Showcase](README.md) · [Complex Visual Challenges](visual-challenges.md) →
