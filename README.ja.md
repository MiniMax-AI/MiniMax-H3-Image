<div align="center">
  <img width="100%" src="assets/minimax-h3-image.jpg" alt="MiniMax H3 Image、オープンウェイト">
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
  <a href="README.zh-CN.md">简体中文</a> |
  <a href="README.ko.md">한국어</a> |
  <a href="README.ja.md"><strong>日本語</strong></a>
</p>

<h1 align="center">MiniMax-H3-Image</h1>

<p align="center"><b><i>One idea with open weights. A world of uses.</i></b></p>

<p align="center">
  <a href="#プロンプト作成スキル">プロンプト作成スキル</a> ·
  <a href="#ショーケース">ショーケース</a> ·
  <a href="#オンラインで使う">オンラインで使う</a> ·
  <a href="#概要">概要</a> ·
  <a href="#ローカルで実行">ローカルで実行</a> ·
  <a href="#プロンプトのコツ">プロンプトのコツ</a> ·
  <a href="#ライセンス">ライセンス</a>
</p>

## プロンプト作成スキル

`h3-image-prompt-writing` スキルは、短いアイデア、ブリーフ、参照画像のセットから MiniMax-H3-Image 用の完全なプロンプトを作成し、MiniMax API で画像まで生成できます。Claude Code、Codex、Cursor など、`SKILL.md` を読み取れるあらゆるエージェントで動作します。[skills CLI](https://github.com/vercel-labs/skills) でインストールします：

```bash
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --skill h3-image-prompt-writing
```

あとはエージェントに依頼するだけです。例：

```text
h3-image-prompt-writing を使って、雨の夜市を描いた 3:4 のポスターを作ってください。
タイトルは「雨夜集市」にして、画像まで生成してください。
```

画像の生成には `MINIMAX_API_KEY` が必要です。中国版プラットフォームでは `MINIMAX_API_BASE=https://api.minimax.cn` も設定します。詳しくは [`skills/README.md`](skills/README.md) を参照してください。

## ショーケース

<!-- BEGIN showcase-grid -->
<table>
<tr><th colspan="4" align="left">オープンソースの先進的な能力</th></tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#16-人の群像6-つのシーン"><img src="assets/showcase/tiles/multi-ref-group-a-output.jpg" alt="16 人の群像、6 つのシーン"></a><br><sub><a href="SHOWCASE.ja.md#16-人の群像6-つのシーン">16 人の群像、6 つのシーン</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#複数参照による服の配色"><img src="assets/showcase/tiles/multi-ref-outfit-color-output.jpg" alt="複数参照による服の配色"></a><br><sub><a href="SHOWCASE.ja.md#複数参照による服の配色">複数参照による服の配色</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#参照画像-10-枚からリビングルーム"><img src="assets/showcase/tiles/furniture-room-output.jpg" alt="参照画像 10 枚からリビングルーム"></a><br><sub><a href="SHOWCASE.ja.md#参照画像-10-枚からリビングルーム">参照画像 10 枚からリビングルーム</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#論文ページから生物学の図"><img src="assets/showcase/tiles/bio-figure-output.jpg" alt="論文ページから生物学の図"></a><br><sub><a href="SHOWCASE.ja.md#論文ページから生物学の図">論文ページから生物学の図</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#レッサーパンダの図解"><img src="assets/showcase/tiles/red-panda-infographic.jpg" alt="レッサーパンダの図解"></a><br><sub><a href="SHOWCASE.ja.md#レッサーパンダの図解">レッサーパンダの図解</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#人員選抜の推理問題"><img src="assets/showcase/tiles/staffing-logic-puzzle.jpg" alt="人員選抜の推理問題"></a><br><sub><a href="SHOWCASE.ja.md#人員選抜の推理問題">人員選抜の推理問題</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#電動バイクの分解図"><img src="assets/showcase/tiles/e-motorcycle-exploded.jpg" alt="電動バイクの分解図"></a><br><sub><a href="SHOWCASE.ja.md#電動バイクの分解図">電動バイクの分解図</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ジェットエンジンの分解図"><img src="assets/showcase/tiles/jet-engine-exploded.jpg" alt="ジェットエンジンの分解図"></a><br><sub><a href="SHOWCASE.ja.md#ジェットエンジンの分解図">ジェットエンジンの分解図</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#モカポットの設計図"><img src="assets/showcase/tiles/moka-pot-blueprint.jpg" alt="モカポットの設計図"></a><br><sub><a href="SHOWCASE.ja.md#モカポットの設計図">モカポットの設計図</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#アリ型六脚メカの線画"><img src="assets/showcase/tiles/ant-hexapod-mech-lineart.jpg" alt="アリ型六脚メカの線画"></a><br><sub><a href="SHOWCASE.ja.md#アリ型六脚メカの線画">アリ型六脚メカの線画</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#四脚メカの-cad-図面"><img src="assets/showcase/tiles/quadruped-mech-cad.jpg" alt="四脚メカの CAD 図面"></a><br><sub><a href="SHOWCASE.ja.md#四脚メカの-cad-図面">四脚メカの CAD 図面</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#メカ獣の分解-cad-図"><img src="assets/showcase/tiles/mech-monster-exploded-cad.jpg" alt="メカ獣の分解 CAD 図"></a><br><sub><a href="SHOWCASE.ja.md#メカ獣の分解-cad-図">メカ獣の分解 CAD 図</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#天井レール配送機"><img src="assets/showcase/tiles/ceiling-rail-courier.jpg" alt="天井レール配送機"></a><br><sub><a href="SHOWCASE.ja.md#天井レール配送機">天井レール配送機</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#車輪脚型配送ロボット"><img src="assets/showcase/tiles/wheel-leg-robot.jpg" alt="車輪脚型配送ロボット"></a><br><sub><a href="SHOWCASE.ja.md#車輪脚型配送ロボット">車輪脚型配送ロボット</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#直角の合わせ鏡"><img src="assets/showcase/tiles/mirror-reflection.jpg" alt="直角の合わせ鏡"></a><br><sub><a href="SHOWCASE.ja.md#直角の合わせ鏡">直角の合わせ鏡</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#投影に差し入れた手"><img src="assets/showcase/tiles/projection-hand-shadow.jpg" alt="投影に差し入れた手"></a><br><sub><a href="SHOWCASE.ja.md#投影に差し入れた手">投影に差し入れた手</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ゲームマップから-3d-ゲーム画面"><img src="assets/showcase/tiles/game-map-to-3d.jpg" alt="ゲームマップから 3D ゲーム画面"></a><br><sub><a href="SHOWCASE.ja.md#ゲームマップから-3d-ゲーム画面">ゲームマップから 3D ゲーム画面</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ペリカンの卒業ピラミッド"><img src="assets/showcase/tiles/pelican-graduation-pyramid.jpg" alt="ペリカンの卒業ピラミッド"></a><br><sub><a href="SHOWCASE.ja.md#ペリカンの卒業ピラミッド">ペリカンの卒業ピラミッド</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ペリカンのクリスマスツリー"><img src="assets/showcase/tiles/pelican-christmas-tree.jpg" alt="ペリカンのクリスマスツリー"></a><br><sub><a href="SHOWCASE.ja.md#ペリカンのクリスマスツリー">ペリカンのクリスマスツリー</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ペリカンのバランス芸"><img src="assets/showcase/tiles/pelican-challenge-3.jpg" alt="ペリカンのバランス芸"></a><br><sub><a href="SHOWCASE.ja.md#ペリカンのバランス芸">ペリカンのバランス芸</a></sub></td>
</tr>
<tr><th colspan="4" align="left">クリエイティブな活用</th></tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#辺境の騎手"><img src="assets/showcase/tiles/frontier-rider.jpg" alt="辺境の騎手"></a><br><sub><a href="SHOWCASE.ja.md#辺境の騎手">辺境の騎手</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#砂漠の大集会"><img src="assets/showcase/tiles/desert-gathering.jpg" alt="砂漠の大集会"></a><br><sub><a href="SHOWCASE.ja.md#砂漠の大集会">砂漠の大集会</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#寒色の鉱物荒野空撮"><img src="assets/showcase/tiles/cold-mineral-aerial.jpg" alt="寒色の鉱物荒野、空撮"></a><br><sub><a href="SHOWCASE.ja.md#寒色の鉱物荒野空撮">寒色の鉱物荒野、空撮</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#赤褐色の鉱物荒野空撮"><img src="assets/showcase/tiles/desert-mineral-aerial.jpg" alt="赤褐色の鉱物荒野、空撮"></a><br><sub><a href="SHOWCASE.ja.md#赤褐色の鉱物荒野空撮">赤褐色の鉱物荒野、空撮</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#森の古代劇場"><img src="assets/showcase/tiles/forest-amphitheater.jpg" alt="森の古代劇場"></a><br><sub><a href="SHOWCASE.ja.md#森の古代劇場">森の古代劇場</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#雲海の上の宮殿"><img src="assets/showcase/tiles/mountain-temple.jpg" alt="雲海の上の宮殿"></a><br><sub><a href="SHOWCASE.ja.md#雲海の上の宮殿">雲海の上の宮殿</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#扇状の炎を放つ魔法使い"><img src="assets/showcase/tiles/fire-mage-vfx.jpg" alt="扇状の炎を放つ魔法使い"></a><br><sub><a href="SHOWCASE.ja.md#扇状の炎を放つ魔法使い">扇状の炎を放つ魔法使い</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#爆発の-2-段階"><img src="assets/showcase/tiles/explosion-two-state.jpg" alt="爆発の 2 段階"></a><br><sub><a href="SHOWCASE.ja.md#爆発の-2-段階">爆発の 2 段階</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#重装騎士のキャラクターシート"><img src="assets/showcase/tiles/armored-knight-sheet.jpg" alt="重装騎士のキャラクターシート"></a><br><sub><a href="SHOWCASE.ja.md#重装騎士のキャラクターシート">重装騎士のキャラクターシート</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#獅子王の顔のクローズアップ"><img src="assets/showcase/tiles/lion-king-face.jpg" alt="獅子王の顔のクローズアップ"></a><br><sub><a href="SHOWCASE.ja.md#獅子王の顔のクローズアップ">獅子王の顔のクローズアップ</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#森のドラゴン"><img src="assets/showcase/tiles/forest-dragon.jpg" alt="森のドラゴン"></a><br><sub><a href="SHOWCASE.ja.md#森のドラゴン">森のドラゴン</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#一人称シューティングの場面"><img src="assets/showcase/tiles/fps-wasteland.jpg" alt="一人称シューティングの場面"></a><br><sub><a href="SHOWCASE.ja.md#一人称シューティングの場面">一人称シューティングの場面</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#白モデルのレンダリングを映画のスチルに"><img src="assets/showcase/tiles/moon-rover-render.jpg" alt="白モデルのレンダリングを映画のスチルに"></a><br><sub><a href="SHOWCASE.ja.md#白モデルのレンダリングを映画のスチルに">白モデルのレンダリングを映画のスチルに</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#峡谷の水力発電所マットペインティング"><img src="assets/showcase/tiles/hydro-station-canyon.jpg" alt="峡谷の水力発電所、マットペインティング"></a><br><sub><a href="SHOWCASE.ja.md#峡谷の水力発電所マットペインティング">峡谷の水力発電所、マットペインティング</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#廃駅"><img src="assets/showcase/tiles/abandoned-station.jpg" alt="廃駅"></a><br><sub><a href="SHOWCASE.ja.md#廃駅">廃駅</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#荒廃した工業地帯"><img src="assets/showcase/tiles/industrial-ruins.jpg" alt="荒廃した工業地帯"></a><br><sub><a href="SHOWCASE.ja.md#荒廃した工業地帯">荒廃した工業地帯</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#凍った湾の難破船"><img src="assets/showcase/tiles/frozen-shipwreck-bay.jpg" alt="凍った湾の難破船"></a><br><sub><a href="SHOWCASE.ja.md#凍った湾の難破船">凍った湾の難破船</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#戦闘パイロット"><img src="assets/showcase/tiles/combat-pilot.jpg" alt="戦闘パイロット"></a><br><sub><a href="SHOWCASE.ja.md#戦闘パイロット">戦闘パイロット</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#極地服のコスチュームボード"><img src="assets/showcase/tiles/polar-costume-board.jpg" alt="極地服のコスチュームボード"></a><br><sub><a href="SHOWCASE.ja.md#極地服のコスチュームボード">極地服のコスチュームボード</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#赤い荒野のヘルメット"><img src="assets/showcase/tiles/helmet-key-art.jpg" alt="赤い荒野のヘルメット"></a><br><sub><a href="SHOWCASE.ja.md#赤い荒野のヘルメット">赤い荒野のヘルメット</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#sf-戦闘機"><img src="assets/showcase/tiles/scifi-fighter.jpg" alt="SF 戦闘機"></a><br><sub><a href="SHOWCASE.ja.md#sf-戦闘機">SF 戦闘機</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#改造マッスルカー"><img src="assets/showcase/tiles/modded-muscle-car.jpg" alt="改造マッスルカー"></a><br><sub><a href="SHOWCASE.ja.md#改造マッスルカー">改造マッスルカー</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#霧の農場ドキュメンタリーのフィルム写真"><img src="assets/showcase/tiles/farm-documentary-film.jpg" alt="霧の農場、ドキュメンタリーのフィルム写真"></a><br><sub><a href="SHOWCASE.ja.md#霧の農場ドキュメンタリーのフィルム写真">霧の農場、ドキュメンタリーのフィルム写真</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#フィルムで撮ったピクニック"><img src="assets/showcase/tiles/picnic-film.jpg" alt="フィルムで撮ったピクニック"></a><br><sub><a href="SHOWCASE.ja.md#フィルムで撮ったピクニック">フィルムで撮ったピクニック</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#フィルムのクローズアップポートレート"><img src="assets/showcase/tiles/film-portrait-closeup.jpg" alt="フィルムのクローズアップポートレート"></a><br><sub><a href="SHOWCASE.ja.md#フィルムのクローズアップポートレート">フィルムのクローズアップポートレート</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#古いスマホのスナップ"><img src="assets/showcase/tiles/iphone7-snapshot.jpg" alt="古いスマホのスナップ"></a><br><sub><a href="SHOWCASE.ja.md#古いスマホのスナップ">古いスマホのスナップ</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#直射フラッシュのフィルムポートレート"><img src="assets/showcase/tiles/flash-film-portrait.jpg" alt="直射フラッシュのフィルムポートレート"></a><br><sub><a href="SHOWCASE.ja.md#直射フラッシュのフィルムポートレート">直射フラッシュのフィルムポートレート</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#おばあちゃんの誕生日ホームビデオ"><img src="assets/showcase/tiles/grandma-birthday-dv.jpg" alt="おばあちゃんの誕生日、ホームビデオ"></a><br><sub><a href="SHOWCASE.ja.md#おばあちゃんの誕生日ホームビデオ">おばあちゃんの誕生日、ホームビデオ</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#夕暮れの屋上"><img src="assets/showcase/tiles/rooftop-bedsheets.jpg" alt="夕暮れの屋上"></a><br><sub><a href="SHOWCASE.ja.md#夕暮れの屋上">夕暮れの屋上</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#お茶を飲む前のひととき"><img src="assets/showcase/tiles/tea-portrait.jpg" alt="お茶を飲む前のひととき"></a><br><sub><a href="SHOWCASE.ja.md#お茶を飲む前のひととき">お茶を飲む前のひととき</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#夜明けのフラミンゴ"><img src="assets/showcase/tiles/flamingo-salt-lake.jpg" alt="夜明けのフラミンゴ"></a><br><sub><a href="SHOWCASE.ja.md#夜明けのフラミンゴ">夜明けのフラミンゴ</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#理容椅子に座る雲"><img src="assets/showcase/tiles/surreal-cloud-barber-chair.jpg" alt="理容椅子に座る雲"></a><br><sub><a href="SHOWCASE.ja.md#理容椅子に座る雲">理容椅子に座る雲</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#月を切り分ける"><img src="assets/showcase/tiles/surreal-long-table.jpg" alt="月を切り分ける"></a><br><sub><a href="SHOWCASE.ja.md#月を切り分ける">月を切り分ける</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#洋梨の更衣室"><img src="assets/showcase/tiles/surreal-pear-dressing-room.jpg" alt="洋梨の更衣室"></a><br><sub><a href="SHOWCASE.ja.md#洋梨の更衣室">洋梨の更衣室</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#切り紙コラージュ"><img src="assets/showcase/tiles/blue-collage.jpg" alt="切り紙コラージュ"></a><br><sub><a href="SHOWCASE.ja.md#切り紙コラージュ">切り紙コラージュ</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#剥がし跡のタイポグラフィポスター"><img src="assets/showcase/tiles/sticker-type-poster.jpg" alt="剥がし跡のタイポグラフィポスター"></a><br><sub><a href="SHOWCASE.ja.md#剥がし跡のタイポグラフィポスター">剥がし跡のタイポグラフィポスター</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ピクセルアートの白猫ポスター"><img src="assets/showcase/tiles/pixel-white-cat.jpg" alt="ピクセルアートの白猫ポスター"></a><br><sub><a href="SHOWCASE.ja.md#ピクセルアートの白猫ポスター">ピクセルアートの白猫ポスター</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#オシドリオールドマスター風油彩"><img src="assets/showcase/tiles/baroque-mandarin-ducks.jpg" alt="オシドリ、オールドマスター風油彩"></a><br><sub><a href="SHOWCASE.ja.md#オシドリオールドマスター風油彩">オシドリ、オールドマスター風油彩</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#漁師とペリカンカラヴァッジョ風"><img src="assets/showcase/tiles/caravaggio-pelican.jpg" alt="漁師とペリカン、カラヴァッジョ風"></a><br><sub><a href="SHOWCASE.ja.md#漁師とペリカンカラヴァッジョ風">漁師とペリカン、カラヴァッジョ風</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#卓球の試合カラヴァッジョ風"><img src="assets/showcase/tiles/caravaggio-ping-pong.jpg" alt="卓球の試合、カラヴァッジョ風"></a><br><sub><a href="SHOWCASE.ja.md#卓球の試合カラヴァッジョ風">卓球の試合、カラヴァッジョ風</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#蘇州庭園のオシドリ印象派の油彩"><img src="assets/showcase/tiles/impressionist-suzhou-garden.jpg" alt="蘇州庭園のオシドリ、印象派の油彩"></a><br><sub><a href="SHOWCASE.ja.md#蘇州庭園のオシドリ印象派の油彩">蘇州庭園のオシドリ、印象派の油彩</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#太陽中世の装飾写本"><img src="assets/showcase/tiles/illuminated-manuscript-a.jpg" alt="太陽、中世の装飾写本"></a><br><sub><a href="SHOWCASE.ja.md#太陽中世の装飾写本">太陽、中世の装飾写本</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#玉兎中世の装飾写本"><img src="assets/showcase/tiles/illuminated-manuscript-b.jpg" alt="玉兎、中世の装飾写本"></a><br><sub><a href="SHOWCASE.ja.md#玉兎中世の装飾写本">玉兎、中世の装飾写本</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#宇宙ステーションの修理敦煌壁画"><img src="assets/showcase/tiles/dunhuang-space-station.jpg" alt="宇宙ステーションの修理、敦煌壁画"></a><br><sub><a href="SHOWCASE.ja.md#宇宙ステーションの修理敦煌壁画">宇宙ステーションの修理、敦煌壁画</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#ペリカンの影絵芝居"><img src="assets/showcase/tiles/shadow-puppet-pelican.jpg" alt="ペリカンの影絵芝居"></a><br><sub><a href="SHOWCASE.ja.md#ペリカンの影絵芝居">ペリカンの影絵芝居</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#回路と花工筆のテキスタイル"><img src="assets/showcase/tiles/gongbi-circuit-textile.jpg" alt="回路と花、工筆のテキスタイル"></a><br><sub><a href="SHOWCASE.ja.md#回路と花工筆のテキスタイル">回路と花、工筆のテキスタイル</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#鏡の前のペリカン工筆画"><img src="assets/showcase/tiles/gongbi-pelican-mirror.jpg" alt="鏡の前のペリカン、工筆画"></a><br><sub><a href="SHOWCASE.ja.md#鏡の前のペリカン工筆画">鏡の前のペリカン、工筆画</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ja.md#金色の炎東洋ファンタジーのイラスト"><img src="assets/showcase/tiles/eastern-fantasy-lineart.jpg" alt="金色の炎、東洋ファンタジーのイラスト"></a><br><sub><a href="SHOWCASE.ja.md#金色の炎東洋ファンタジーのイラスト">金色の炎、東洋ファンタジーのイラスト</a></sub></td>
</tr>
</table>

画像を選ぶと、大きな画像とプロンプトを表示します。
<!-- END showcase-grid -->

## オンラインで使う

| | グローバル | 中国 |
| --- | --- | --- |
| Web アプリ | [hailuoai.video](https://hailuoai.video/) | [hailuoai.com](https://hailuoai.com/) |
| デスクトップアプリ | [agent.minimax.io](https://agent.minimax.io/) | [agent.minimax.cn](https://agent.minimax.cn) |
| API プラットフォーム | [platform.minimax.io](https://platform.minimax.io/docs/guides/image-generation) | [platform.minimax.cn](https://platform.minimax.cn/docs/guides/image-generation) |
| API リファレンス | [テキストからの画像生成](https://platform.minimax.io/docs/api-reference/image-generation-h3-generations) · [画像編集](https://platform.minimax.io/docs/api-reference/image-generation-h3-edits) · [プロンプト拡張](https://platform.minimax.io/docs/api-reference/image-generation-h3-context-ir) | [テキストからの画像生成](https://platform.minimax.cn/docs/api-reference/image-generation-h3-generations) · [画像編集](https://platform.minimax.cn/docs/api-reference/image-generation-h3-edits) · [プロンプト拡張](https://platform.minimax.cn/docs/api-reference/image-generation-h3-context-ir) |

## 概要

MiniMax-H3-Image は、[MiniMax H3](https://huggingface.co/MiniMaxAI/MiniMax-H3) ファミリーの最先端のオープンソース画像生成・編集モデルです。テキストからの画像生成と複数画像の編集を 1 つの checkpoint で行えます。

- **実用的なコストで 16 MP を生成**：どのアスペクト比でも約 16 MP の画像を、アップスケーラーを使わず 6 サンプリングステップで直接生成します。
- **豊かなディテールと高いリアリティ**：見慣れた「AI っぽさ」を超えた画像を生成します。
- **オープンソースモデルで最も強い指示追従**：最大 16 枚の参照画像に対応します。

### 仕様

MiniMax API の仕様です。ローカルサーバーのフィールドは [リクエストパラメータ](#リクエストパラメータ) を参照してください。

| パラメータ | 仕様 |
| --- | --- |
| モデル ID | `MiniMax-H3-Image` |
| タスク | テキストからの画像生成、画像編集 |
| 画像サイズ | `width` + `height`、または `area` + `aspect_ratio` で指定します。デフォルトは `auto` で、面積は 4K、アスペクト比は自動で決まります |
| 出力面積 | `1K`、`2K`、または **`4K`（最良の結果 👍）**。`width` × `height` を直接指定する場合は 655,360〜20,000,000 ピクセル |
| アスペクト比 | 1:3〜3:1 |
| プロンプト | 最大 32,000 文字。4,096 トークンを超える部分は切り捨てられます |
| 参照画像 | 最大 16 枚。1 枚あたり 64 MiB 以下で、辺の長さは 128〜8192 ピクセル、アスペクト比は 1:4〜4:1 |
| 参照画像の形式 | JPG、PNG、WebP、HEIC、HEIF。HTTP(S) URL、Base64、または MiniMax のファイル ID で送信します |
| 1 リクエストあたりの画像数 | 1〜10 |
| プロンプト拡張 | テキストからの画像生成ではデフォルトで有効で、無効にもできます。画像編集では常に有効です。拡張後のプロンプトを返すこともできます |
| 出力 | PNG（デフォルト）、JPEG、WebP。`output_compression` は 0〜100。URL（デフォルト）または Base64 で返されます |
| 現時点で未対応 | マスクを使ったインペインティング、透明背景、ユーザー指定の seed、プレビュー画像 |

### モデル一覧

| モデル | 役割 | 精度 | サイズ | Hugging Face |
| --- | --- | --- | --- | --- |
| **MiniMax-H3-Image** | テキストからの画像生成と画像編集 | BF16 (DiT) | 68.65 GB | [MiniMaxAI/MiniMax-H3-Image](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image) |
| **MiniMax-H3-Image-PE**（任意） | テキストからの画像生成用のプロンプト拡張モデル | NVFP4 | 17.9 GB | [MiniMaxAI/MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE) |

### モデルアーキテクチャ

MiniMax-H3-Image は H3-Base の設計を踏襲し、音声ブランチを取り除いたものです。テキストプロンプトと参照画像は H3 テキストエンコーダーでエンコードされ、参照画像は画像 VAE でもエンコードされます。すべてのトークンは 1 つのパック済みシーケンスにまとめられてシングルストリーム Transformer に入力され、Transformer がターゲット画像の latent を予測します。VAE はその latent を画像にデコードします。

- **テキストエンコーダー**：MiniMax-H3 の Qwen3-VL テキストエンコーダー全体をそのまま使用します。DiT はその第 50 層の hidden states を読み取ります。
- **画像 VAE**：CNN エンコーダーと 2D ViT デコーダー（24 層）で構成され、空間方向に 16 倍のダウンサンプリングを行い、latent のチャネル数は 24 です。DiT は latent を 2x2 のパッチでパッチ化するため、Transformer の各トークンは 32x32 ピクセルに相当します。
- **拡散 Transformer**：パラメータ数 33.1B の dense なシングルストリーム Transformer で、50 層（hidden size 5376、attention head 数 56、FFN サイズ 14336）と 3D マルチモーダル RoPE を備えます。これは H3-Omni-Transformer と同じ構成です。重みは BF16 で、embedding 層、timestep 層、出力層は FP32 です。

## ローカルで実行

### ダウンロード

| コンポーネント | 内容 | サイズ |
| --- | --- | --- |
| `transformer/` | DiT の重み。 | 66.28 GB |
| `pdd_fused_heads.safetensors`、`pdd_config.json` | Transformer の出力層を置き換えるステップごとの出力ヘッドと、サンプリングスケジュール。 | 12 MB |
| `vae/` | 画像 VAE、FP32。 | 2.34 GB |
| `tokenizer/`、`processor/` | Qwen3-VL の tokenizer と processor。MiniMax-H3 と同一です。 | 23 MB |
| テキストエンコーダー | 元の checkpoint には含まれません。`model_index.json` が [`MiniMaxAI/MiniMax-H3`](https://huggingface.co/MiniMaxAI/MiniMax-H3) の `text_encoder/` フォルダから読み込みます。MiniMax-H3 をすでにダウンロードしている場合、再度ダウンロードされることはありません。 | 66.7 GB |

Hugging Face リポジトリでは、この元の checkpoint と diffusers 形式を並べて提供しており、合計で約 204 GB です。SGLang と vLLM-Omni に必要なのは元の checkpoint と MiniMax-H3 のテキストエンコーダーだけで、合計約 135 GB です：

```bash
hf download MiniMaxAI/MiniMax-H3-Image model_index.json "pdd_*" "processor/*" "tokenizer/*" \
  "transformer/*" "vae/*"
hf download MiniMaxAI/MiniMax-H3 --include "text_encoder/*"
# optional prompt expander
hf download MiniMaxAI/MiniMax-H3-Image-PE
```

diffusers は `ModularPipeline.from_pretrained("MiniMaxAI/MiniMax-H3-Image")` で必要なファイルを自動で取得します。

### デプロイ

モデルのサービングには以下の推論フレームワークを推奨します：

- [SGLang](https://docs.sglang.io/) - [cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3-Image) を参照
- [vLLM-Omni](https://github.com/vllm-project/vllm-omni) - [vllm-omni recipe](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image) を参照
- [diffusers](https://github.com/huggingface/diffusers) - [diffusers ドキュメント](https://huggingface.co/docs/diffusers/main/en/api/pipelines/minimax_h3_image) を参照
- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) - [Comfy チュートリアル](https://docs.comfy.org/tutorials/image/minimax/minimax-h3-image) を参照。テンプレートは [T2I テンプレート](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/image_minimax_h3_image_t2i.json) / [Edit テンプレート](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/image_minimax_h3_image_edit.json) を使用します

#### SGLang

main ブランチから SGLang を拡散モデル用の依存関係とともにインストールします（[インストールガイド](https://docs.sglang.io/docs/sglang-diffusion/installation) を参照）：

```bash
git clone https://github.com/sgl-project/sglang.git
cd sglang
python3 -m pip install -e 'python[diffusion]'
```

1 枚の GPU で起動できます（空きメモリが 130 GiB 未満の場合、SGLang はモデルの一部のコンポーネントをオフロードします）。レイテンシを下げるには、シーケンス並列（Ulysses）で各リクエストを複数の GPU に分割します：

```bash
sglang serve --model-path MiniMaxAI/MiniMax-H3-Image --host 0.0.0.0 --port 30000 --warmup-mode off
# 4 GPUs
sglang serve --model-path MiniMaxAI/MiniMax-H3-Image --host 0.0.0.0 --port 30000 --warmup-mode off \
  --num-gpus 4 --ulysses-degree 4
```

ローカルにある MiniMax-H3 のテキストエンコーダーを使うには `--text-encoder-path <path to text_encoder>` を追加します。[SGLang cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3-Image) には、B300 から 12 GB のカードまで、ほかの GPU 向けのレシピがあります。

#### vLLM-Omni

vLLM 0.33.0 をインストールしてから、vLLM-Omni をソースからインストールします：

```bash
uv venv --python 3.12 --seed && source .venv/bin/activate
uv pip install vllm==0.33.0 --torch-backend=cu130
git clone https://github.com/vllm-project/vllm-omni.git && cd vllm-omni && uv pip install -e .
```

シーケンス並列（Ulysses）で 4 枚の GPU を使うか、1 枚の GPU でサービングします。B200、B300 は約 135 GiB のメモリにモデル全体を載せ、1 枚の H200 ではテキストエンコーダーをオフロードします：

```bash
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 \
  --num-gpus 4 --usp 4 --text-encoder-tp-size 4
# one B200 or B300
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 --num-gpus 1
# one H200: offload the text encoder
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 --num-gpus 1 \
  --diffusion-offload-config '{"mode":"layer","components":["text_encoder"]}'
```

AMD Instinct などほかの GPU 向けの構成は [vLLM-Omni recipe](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image) にあります。

### リクエストパラメータ

SGLang では、テキストからの画像生成のリクエストは JSON として `/v1/images/generations` に、画像編集のリクエストは multipart form data として `/v1/images/edits` に送信します。どちらも PNG を `data[0].b64_json` で返します。vLLM-Omni はフィールドが少し異なるため、[recipe](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image) を参照してください。

| フィールド | テキストからの画像生成 | 画像編集 | 備考 |
| --- | --- | --- | --- |
| `prompt` | 必須 | 必須 | そのまま使用され、4096 トークンで切り詰められます |
| `size` | 必須 | 必須 | `WIDTHxHEIGHT`。返される画像はちょうどこのサイズになります。[サイズ](#サイズ) を参照 |
| `image` | — | 1 つ以上のファイル | アップロード順に、プロンプト内の `<Picture 1>`、`<Picture 2>`、... になります |
| `seed` | 推奨 | 推奨 | 整数 |
| `generator_device` | `cpu` を推奨 | `cpu` を推奨 | 同じ seed なら、どのマシンでも同じ初期ノイズになります |
| `response_format` | `b64_json` | `b64_json` | |
| `min_generation_area` | 任意 | 任意 | 生成する最小面積（ピクセル数）。1024-16777216、デフォルトは 4194304（2048x2048）。これより小さい `size` は、同じアスペクト比のより大きなキャンバスで生成してから LANCZOS で元のサイズに縮小します。この動作を無効にするには 1024 を指定します。下の表のサイズはすべてデフォルトより大きくなっています |
| `num_inference_steps` | 省略または 6 | 省略または 6 | それ以外の値は HTTP 400 を返します |
| `guidance_scale` | 省略または 1 | 省略または 1 | それ以外の値は HTTP 400 を返します |
| `negative_prompt` | 非対応 | 非対応 | 拒否されます |

### サイズ

有効に動作する範囲はおよそ 4 MP から 20 MP で、一般に 16 MP 前後で最も良い結果が得られます。よく使われる 16 MP のサイズ：

| アスペクト比 | サイズ（幅 x 高さ） |
| --- | --- |
| 1:1 | 4096x4096 |
| 4:3 / 3:4 | 4736x3552 / 3552x4736 |
| 3:2 / 2:3 | 5024x3360 / 3360x5024 |
| 16:9 / 9:16 | 5472x3072 / 3072x5472 |
| 21:9 | 6272x2688 |

ほかのアスペクト比では、約 16 MP を保ち、幅と高さをどちらも 32 の倍数にします。[`examples/context_ir.py`](examples/context_ir.py) の `size_for()` で計算できます：

```bash
cd MiniMax-H3-Image/examples
python3 -c "from context_ir import size_for; print(size_for('5:4'))"   # 4576x3648
```

### 完全なワークフロー

MiniMax API は生成前に **H3-Image-Context-IR** を使い、任意の言語で書かれた短いプロンプトを、画像全体を詳しく記述した英語の説明文に拡張します。ローカルサーバーはプロンプトをそのまま使うため、以下の例のように先に拡張してください。[`examples/`](examples) のスクリプトは、上の SGLang サーバーを使って API の結果を再現します。Python 標準ライブラリだけを使用します：

```bash
git clone https://github.com/MiniMax-AI/MiniMax-H3-Image.git
cd MiniMax-H3-Image/examples
export MINIMAX_API_BASE="https://api.minimax.io"   # China: https://api.minimax.cn
export MINIMAX_API_KEY="<api-key>"
```

`t2i.py` と `edit.py` は `http://127.0.0.1:30000` にリクエストを送ります。別のアドレスを使う場合は `--url` を指定してください。

#### case-T2I

[`instruction.t2i.txt`](examples/instruction.t2i.txt) を使用します。

<table>
<thead>
<tr><th colspan="2">段階</th><th>リクエスト</th><th>結果</th></tr>
</thead>
<tbody>
<tr><td rowspan="3">プロンプト強化</td><td>H3-Image-Context-IR (MiniMax API)</td><td><code>python3 context_ir.py t2i</code>（<a href="examples/context_ir.py">スクリプト</a>）</td><td><code>revised_prompt.txt</code>、<code>revised_size.txt</code>。こちらで実行した結果：<a href="examples/revised_prompt.t2i.txt"><code>revised_prompt.t2i.txt</code></a>、<a href="examples/revised_size.t2i.txt"><code>revised_size.t2i.txt</code></a>（4736x3552）</td></tr>
<tr><td>ローカルでの代替手段：<a href="https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE">MiniMax-H3-Image-PE</a></td><td>PE リポジトリの <code>scripts/expand_prompt.py</code></td><td><code>expanded_caption</code> を <code>revised_prompt.txt</code> として保存し、<code>aspect_ratio</code> に対応するサイズを <code>revised_size.txt</code> として保存</td></tr>
<tr><td>エージェントによる代替手段：<a href="#プロンプト作成スキル">h3-image-prompt-writing</a></td><td>エージェントに、スキルを使って <code>instruction.t2i.txt</code> のプロンプトとアスペクト比を書くよう依頼</td><td>プロンプトを <code>revised_prompt.txt</code> として保存し、そのアスペクト比に対応する<a href="#サイズ">サイズ</a>を <code>revised_size.txt</code> として保存</td></tr>
<tr><td colspan="2">MiniMax-H3-Image による生成：ローカル SGLang</td><td><code>python3 t2i.py --prompt revised_prompt.txt --size $(cat revised_size.txt)</code>（<a href="examples/t2i.py">スクリプト</a>）</td><td><code>t2i.png</code></td></tr>
<tr><td colspan="2">E2E API リファレンス：MiniMax API を直接呼び出したテキストからの画像生成</td><td><code>python3 api_generate.py t2i</code>（<a href="examples/api_generate.py">スクリプト</a>）</td><td><code>api_t2i.png</code></td></tr>
</tbody>
</table>

<p align="center">
<img src="assets/workflow_t2i.jpg" alt="左：拡張済みプロンプトを使ってローカル SGLang で生成した t2i.png。右：MiniMax API で生成した api_t2i.png。どちらも、使い込まれた木のテーブルにパン、野菜、チーズが並ぶファーム・トゥ・テーブルの食卓を真上から写したもの" width="100%"/>
</p>
<p align="center"><em>ローカル SGLang による t2i.png（左）と MiniMax API による api_t2i.png（右）、4736x3552（H3-Image-Context-IR が 4:3 を選択）</em></p>

#### case-Edit

[`instruction.edit.txt`](examples/instruction.edit.txt) と、`<Picture 1>` として参照画像 [`reference1.png`](examples/reference1.png) を使用します。

| 段階 | リクエスト | 結果 |
| --- | --- | --- |
| プロンプト強化：H3-Image-Context-IR (MiniMax API) | `python3 context_ir.py edit`（[スクリプト](examples/context_ir.py)） | `revised_prompt.txt`、`revised_size.txt`。こちらで実行した結果：[`revised_prompt.edit.txt`](examples/revised_prompt.edit.txt)、[`revised_size.edit.txt`](examples/revised_size.edit.txt)（4096x4096） |
| プロンプト強化、エージェントによる代替手段：[h3-image-prompt-writing](#プロンプト作成スキル) | エージェントに、スキルを使って `reference1.png` 向けに `instruction.edit.txt` を書き直すよう依頼 | プロンプトを `revised_prompt.txt` として、`4096x4096` を `revised_size.txt` として保存 |
| MiniMax-H3-Image による生成：ローカル SGLang | `python3 edit.py --prompt revised_prompt.txt --size $(cat revised_size.txt)`（[スクリプト](examples/edit.py)） | `edit.png` |
| E2E API リファレンス：MiniMax API を直接呼び出した画像編集 | `python3 api_generate.py edit`（[スクリプト](examples/api_generate.py)） | `api_edit.png` |

<p align="center">
<img src="assets/workflow_edit.jpg" alt="左：参照画像 reference1.png。2 人のポッドキャストホストが写っており、男性はヘッドホンを着けている。中央：拡張済みプロンプトを使ってローカル SGLang で生成した edit.png。右：MiniMax API で生成した api_edit.png。どちらの結果でもヘッドホンはなくなり、2 人が MONEY TALKS の看板の上で拳を合わせている" width="100%"/>
</p>
<p align="center"><em>参照画像 reference1.png（左）、ローカル SGLang による edit.png（中央）、MiniMax API による api_edit.png（右）、4096x4096（H3-Image-Context-IR が 1:1 を選択）</em></p>

## プロンプトのコツ

公式ユーザーガイドのコツです。MiniMax API にもローカルサーバーにも当てはまり、[プロンプト作成スキル](#プロンプト作成スキル) はこれらに従ってプロンプトを書きます。

- **スタイルより先にタスク、細部より先にレイアウト。** 画像の用途と内容、次にレイアウトを書き、スタイルは「高級感」のような言葉ではなく、色、素材、光など目に見えるディテールで表現します。
- **表示する文字はすべて引用符で書く。** 位置と改行も指定します。文字が不要な場合は「画像内に文字、アルファベット、数字を入れない」と書きます。
- **グラフや教育用の画像には正確なデータを示す。** 単位と期間を書き、例示用のデータはそのことを明記します。
- **参照画像ごとに役割を割り当てる。** 変える部分と残す部分も書きます。例：「左側のカップを青にする。形、素材、位置、サイズは変えない」。
- **グリッドは行と列で指定する。** 「2×3」ではなく「2 行 3 列」のように書きます。

## ライセンス

- MiniMax-H3-Image は [MiniMax-H3-Image Community License Agreement](LICENSE) の下で公開されています。
- T2I PE モデル（[MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE)）は MiniMax-H3-Image の一部であり、同様に [MiniMax-H3-Image Community License Agreement](LICENSE) の対象となります。
- ライセンス第 IV 条に記載されている個別の書面による許諾は、[申請フォーム](https://platform.minimax.io/console/license) から申請してください。

## お問い合わせ

お問い合わせは [model@minimax.io](mailto:model@minimax.io) までお願いします。
