<div align="center">
  <img width="100%" src="assets/minimax-h3-image.jpg" alt="MiniMax H3 image, 오픈 웨이트">
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
  <a href="README.ko.md"><strong>한국어</strong></a> |
  <a href="README.ja.md">日本語</a>
</p>

<h1 align="center">MiniMax-H3-Image</h1>

<p align="center"><b><i>One idea with open weights. A world of uses.</i></b></p>

<p align="center">
  <a href="#프롬프트-작성-스킬">프롬프트 작성 스킬</a> ·
  <a href="#쇼케이스">쇼케이스</a> ·
  <a href="#온라인-사용">온라인 사용</a> ·
  <a href="#개요">개요</a> ·
  <a href="#로컬-실행">로컬 실행</a> ·
  <a href="#프롬프트-작성-팁">프롬프트 작성 팁</a> ·
  <a href="#라이선스">라이선스</a>
</p>

## 프롬프트 작성 스킬

`h3-image-prompt-writing` 스킬은 짧은 아이디어, 브리프 또는 여러 장의 참조 이미지로 MiniMax-H3-Image용 완전한 프롬프트를 작성하고, MiniMax API로 이미지까지 생성할 수 있습니다. Claude Code, Codex, Cursor 등 `SKILL.md`를 읽을 수 있는 모든 에이전트에서 동작합니다. [skills CLI](https://github.com/vercel-labs/skills)로 설치합니다:

```bash
npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --skill h3-image-prompt-writing
```

그다음 에이전트에게 요청하면 됩니다. 예:

```text
h3-image-prompt-writing으로 비 내리는 야시장을 담은 3:4 포스터를 만들어 주세요.
제목은 "雨夜集市"로 하고, 이미지까지 생성해 주세요.
```

이미지를 생성하려면 `MINIMAX_API_KEY`가 필요하며, 중국 플랫폼에서는 `MINIMAX_API_BASE=https://api.minimax.cn`도 설정합니다. 자세한 내용은 [`skills/README.md`](skills/README.md)를 참고하세요.

## 쇼케이스

<!-- BEGIN showcase-grid -->
<table>
<tr><th colspan="4" align="left">오픈소스 고급 역량</th></tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#16명의-군상-여섯-장면"><img src="assets/showcase/tiles/multi-ref-group-a-output.jpg" alt="16명의 군상, 여섯 장면"></a><br><sub><a href="SHOWCASE.ko.md#16명의-군상-여섯-장면">16명의 군상, 여섯 장면</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#다중-참조-의상-배색"><img src="assets/showcase/tiles/multi-ref-outfit-color-output.jpg" alt="다중 참조 의상 배색"></a><br><sub><a href="SHOWCASE.ko.md#다중-참조-의상-배색">다중 참조 의상 배색</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#참조-이미지-10장으로-만든-거실"><img src="assets/showcase/tiles/furniture-room-output.jpg" alt="참조 이미지 10장으로 만든 거실"></a><br><sub><a href="SHOWCASE.ko.md#참조-이미지-10장으로-만든-거실">참조 이미지 10장으로 만든 거실</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#논문-페이지로-만든-생물학-그림"><img src="assets/showcase/tiles/bio-figure-output.jpg" alt="논문 페이지로 만든 생물학 그림"></a><br><sub><a href="SHOWCASE.ko.md#논문-페이지로-만든-생물학-그림">논문 페이지로 만든 생물학 그림</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#레서판다-인포그래픽"><img src="assets/showcase/tiles/red-panda-infographic.jpg" alt="레서판다 인포그래픽"></a><br><sub><a href="SHOWCASE.ko.md#레서판다-인포그래픽">레서판다 인포그래픽</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#인원-선발-추리-문제"><img src="assets/showcase/tiles/staffing-logic-puzzle.jpg" alt="인원 선발 추리 문제"></a><br><sub><a href="SHOWCASE.ko.md#인원-선발-추리-문제">인원 선발 추리 문제</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#전기-오토바이-분해도"><img src="assets/showcase/tiles/e-motorcycle-exploded.jpg" alt="전기 오토바이 분해도"></a><br><sub><a href="SHOWCASE.ko.md#전기-오토바이-분해도">전기 오토바이 분해도</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#제트-엔진-분해도"><img src="assets/showcase/tiles/jet-engine-exploded.jpg" alt="제트 엔진 분해도"></a><br><sub><a href="SHOWCASE.ko.md#제트-엔진-분해도">제트 엔진 분해도</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#모카포트-설계도"><img src="assets/showcase/tiles/moka-pot-blueprint.jpg" alt="모카포트 설계도"></a><br><sub><a href="SHOWCASE.ko.md#모카포트-설계도">모카포트 설계도</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#개미형-육족-메카-선화"><img src="assets/showcase/tiles/ant-hexapod-mech-lineart.jpg" alt="개미형 육족 메카 선화"></a><br><sub><a href="SHOWCASE.ko.md#개미형-육족-메카-선화">개미형 육족 메카 선화</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#사족-메카-cad-도면"><img src="assets/showcase/tiles/quadruped-mech-cad.jpg" alt="사족 메카 CAD 도면"></a><br><sub><a href="SHOWCASE.ko.md#사족-메카-cad-도면">사족 메카 CAD 도면</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#메카-야수-분해-cad-도면"><img src="assets/showcase/tiles/mech-monster-exploded-cad.jpg" alt="메카 야수 분해 CAD 도면"></a><br><sub><a href="SHOWCASE.ko.md#메카-야수-분해-cad-도면">메카 야수 분해 CAD 도면</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#천장-레일-배송기"><img src="assets/showcase/tiles/ceiling-rail-courier.jpg" alt="천장 레일 배송기"></a><br><sub><a href="SHOWCASE.ko.md#천장-레일-배송기">천장 레일 배송기</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#휠-레그-배송-로봇"><img src="assets/showcase/tiles/wheel-leg-robot.jpg" alt="휠-레그 배송 로봇"></a><br><sub><a href="SHOWCASE.ko.md#휠-레그-배송-로봇">휠-레그 배송 로봇</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#직각-거울"><img src="assets/showcase/tiles/mirror-reflection.jpg" alt="직각 거울"></a><br><sub><a href="SHOWCASE.ko.md#직각-거울">직각 거울</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#투사광-속의-손"><img src="assets/showcase/tiles/projection-hand-shadow.jpg" alt="투사광 속의 손"></a><br><sub><a href="SHOWCASE.ko.md#투사광-속의-손">투사광 속의 손</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#게임-지도에서-3d-게임-화면으로"><img src="assets/showcase/tiles/game-map-to-3d.jpg" alt="게임 지도에서 3D 게임 화면으로"></a><br><sub><a href="SHOWCASE.ko.md#게임-지도에서-3d-게임-화면으로">게임 지도에서 3D 게임 화면으로</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#펠리컨-졸업-피라미드"><img src="assets/showcase/tiles/pelican-graduation-pyramid.jpg" alt="펠리컨 졸업 피라미드"></a><br><sub><a href="SHOWCASE.ko.md#펠리컨-졸업-피라미드">펠리컨 졸업 피라미드</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#펠리컨-크리스마스트리"><img src="assets/showcase/tiles/pelican-christmas-tree.jpg" alt="펠리컨 크리스마스트리"></a><br><sub><a href="SHOWCASE.ko.md#펠리컨-크리스마스트리">펠리컨 크리스마스트리</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#펠리컨-균형-잡기"><img src="assets/showcase/tiles/pelican-challenge-3.jpg" alt="펠리컨 균형 잡기"></a><br><sub><a href="SHOWCASE.ko.md#펠리컨-균형-잡기">펠리컨 균형 잡기</a></sub></td>
</tr>
<tr><th colspan="4" align="left">창작 활용</th></tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#변방의-기수"><img src="assets/showcase/tiles/frontier-rider.jpg" alt="변방의 기수"></a><br><sub><a href="SHOWCASE.ko.md#변방의-기수">변방의 기수</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#사막의-대집회"><img src="assets/showcase/tiles/desert-gathering.jpg" alt="사막의 대집회"></a><br><sub><a href="SHOWCASE.ko.md#사막의-대집회">사막의 대집회</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#차가운-색의-광물-황야-항공샷"><img src="assets/showcase/tiles/cold-mineral-aerial.jpg" alt="차가운 색의 광물 황야 항공샷"></a><br><sub><a href="SHOWCASE.ko.md#차가운-색의-광물-황야-항공샷">차가운 색의 광물 황야 항공샷</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#적갈색-광물-황야-항공샷"><img src="assets/showcase/tiles/desert-mineral-aerial.jpg" alt="적갈색 광물 황야 항공샷"></a><br><sub><a href="SHOWCASE.ko.md#적갈색-광물-황야-항공샷">적갈색 광물 황야 항공샷</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#숲속-원형-극장"><img src="assets/showcase/tiles/forest-amphitheater.jpg" alt="숲속 원형 극장"></a><br><sub><a href="SHOWCASE.ko.md#숲속-원형-극장">숲속 원형 극장</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#운해-위의-궁전"><img src="assets/showcase/tiles/mountain-temple.jpg" alt="운해 위의 궁전"></a><br><sub><a href="SHOWCASE.ko.md#운해-위의-궁전">운해 위의 궁전</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#부채꼴-화염을-쏘는-마법사"><img src="assets/showcase/tiles/fire-mage-vfx.jpg" alt="부채꼴 화염을 쏘는 마법사"></a><br><sub><a href="SHOWCASE.ko.md#부채꼴-화염을-쏘는-마법사">부채꼴 화염을 쏘는 마법사</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#폭발의-두-단계"><img src="assets/showcase/tiles/explosion-two-state.jpg" alt="폭발의 두 단계"></a><br><sub><a href="SHOWCASE.ko.md#폭발의-두-단계">폭발의 두 단계</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#중갑-기사-캐릭터-시트"><img src="assets/showcase/tiles/armored-knight-sheet.jpg" alt="중갑 기사 캐릭터 시트"></a><br><sub><a href="SHOWCASE.ko.md#중갑-기사-캐릭터-시트">중갑 기사 캐릭터 시트</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#사자왕-얼굴-클로즈업"><img src="assets/showcase/tiles/lion-king-face.jpg" alt="사자왕 얼굴 클로즈업"></a><br><sub><a href="SHOWCASE.ko.md#사자왕-얼굴-클로즈업">사자왕 얼굴 클로즈업</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#숲속의-용"><img src="assets/showcase/tiles/forest-dragon.jpg" alt="숲속의 용"></a><br><sub><a href="SHOWCASE.ko.md#숲속의-용">숲속의 용</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#1인칭-슈팅-장면"><img src="assets/showcase/tiles/fps-wasteland.jpg" alt="1인칭 슈팅 장면"></a><br><sub><a href="SHOWCASE.ko.md#1인칭-슈팅-장면">1인칭 슈팅 장면</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#텍스처-없는-렌더링에서-영화-스틸로"><img src="assets/showcase/tiles/moon-rover-render.jpg" alt="텍스처 없는 렌더링에서 영화 스틸로"></a><br><sub><a href="SHOWCASE.ko.md#텍스처-없는-렌더링에서-영화-스틸로">텍스처 없는 렌더링에서 영화 스틸로</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#협곡의-수력발전소-매트-페인팅"><img src="assets/showcase/tiles/hydro-station-canyon.jpg" alt="협곡의 수력발전소, 매트 페인팅"></a><br><sub><a href="SHOWCASE.ko.md#협곡의-수력발전소-매트-페인팅">협곡의 수력발전소, 매트 페인팅</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#버려진-역"><img src="assets/showcase/tiles/abandoned-station.jpg" alt="버려진 역"></a><br><sub><a href="SHOWCASE.ko.md#버려진-역">버려진 역</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#폐허가-된-공업-단지"><img src="assets/showcase/tiles/industrial-ruins.jpg" alt="폐허가 된 공업 단지"></a><br><sub><a href="SHOWCASE.ko.md#폐허가-된-공업-단지">폐허가 된 공업 단지</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#얼어붙은-만의-난파선"><img src="assets/showcase/tiles/frozen-shipwreck-bay.jpg" alt="얼어붙은 만의 난파선"></a><br><sub><a href="SHOWCASE.ko.md#얼어붙은-만의-난파선">얼어붙은 만의 난파선</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#전투-조종사"><img src="assets/showcase/tiles/combat-pilot.jpg" alt="전투 조종사"></a><br><sub><a href="SHOWCASE.ko.md#전투-조종사">전투 조종사</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#극지-의상-코스튬-보드"><img src="assets/showcase/tiles/polar-costume-board.jpg" alt="극지 의상 코스튬 보드"></a><br><sub><a href="SHOWCASE.ko.md#극지-의상-코스튬-보드">극지 의상 코스튬 보드</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#붉은-황야의-헬멧"><img src="assets/showcase/tiles/helmet-key-art.jpg" alt="붉은 황야의 헬멧"></a><br><sub><a href="SHOWCASE.ko.md#붉은-황야의-헬멧">붉은 황야의 헬멧</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#sf-전투기"><img src="assets/showcase/tiles/scifi-fighter.jpg" alt="SF 전투기"></a><br><sub><a href="SHOWCASE.ko.md#sf-전투기">SF 전투기</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#개조-머슬카"><img src="assets/showcase/tiles/modded-muscle-car.jpg" alt="개조 머슬카"></a><br><sub><a href="SHOWCASE.ko.md#개조-머슬카">개조 머슬카</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#안개-낀-농장-다큐멘터리-필름-사진"><img src="assets/showcase/tiles/farm-documentary-film.jpg" alt="안개 낀 농장, 다큐멘터리 필름 사진"></a><br><sub><a href="SHOWCASE.ko.md#안개-낀-농장-다큐멘터리-필름-사진">안개 낀 농장, 다큐멘터리 필름 사진</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#필름으로-찍은-피크닉"><img src="assets/showcase/tiles/picnic-film.jpg" alt="필름으로 찍은 피크닉"></a><br><sub><a href="SHOWCASE.ko.md#필름으로-찍은-피크닉">필름으로 찍은 피크닉</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#필름-클로즈업-인물-사진"><img src="assets/showcase/tiles/film-portrait-closeup.jpg" alt="필름 클로즈업 인물 사진"></a><br><sub><a href="SHOWCASE.ko.md#필름-클로즈업-인물-사진">필름 클로즈업 인물 사진</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#오래된-휴대폰-스냅"><img src="assets/showcase/tiles/iphone7-snapshot.jpg" alt="오래된 휴대폰 스냅"></a><br><sub><a href="SHOWCASE.ko.md#오래된-휴대폰-스냅">오래된 휴대폰 스냅</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#직광-플래시-필름-인물-사진"><img src="assets/showcase/tiles/flash-film-portrait.jpg" alt="직광 플래시 필름 인물 사진"></a><br><sub><a href="SHOWCASE.ko.md#직광-플래시-필름-인물-사진">직광 플래시 필름 인물 사진</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#할머니의-생일-홈비디오"><img src="assets/showcase/tiles/grandma-birthday-dv.jpg" alt="할머니의 생일, 홈비디오"></a><br><sub><a href="SHOWCASE.ko.md#할머니의-생일-홈비디오">할머니의 생일, 홈비디오</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#해-질-녘-옥상"><img src="assets/showcase/tiles/rooftop-bedsheets.jpg" alt="해 질 녘 옥상"></a><br><sub><a href="SHOWCASE.ko.md#해-질-녘-옥상">해 질 녘 옥상</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#차를-마시기-전-잠깐"><img src="assets/showcase/tiles/tea-portrait.jpg" alt="차를 마시기 전 잠깐"></a><br><sub><a href="SHOWCASE.ko.md#차를-마시기-전-잠깐">차를 마시기 전 잠깐</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#새벽의-플라밍고"><img src="assets/showcase/tiles/flamingo-salt-lake.jpg" alt="새벽의 플라밍고"></a><br><sub><a href="SHOWCASE.ko.md#새벽의-플라밍고">새벽의 플라밍고</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#이발-의자에-앉은-구름"><img src="assets/showcase/tiles/surreal-cloud-barber-chair.jpg" alt="이발 의자에 앉은 구름"></a><br><sub><a href="SHOWCASE.ko.md#이발-의자에-앉은-구름">이발 의자에 앉은 구름</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#달-자르기"><img src="assets/showcase/tiles/surreal-long-table.jpg" alt="달 자르기"></a><br><sub><a href="SHOWCASE.ko.md#달-자르기">달 자르기</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#서양배-탈의실"><img src="assets/showcase/tiles/surreal-pear-dressing-room.jpg" alt="서양배 탈의실"></a><br><sub><a href="SHOWCASE.ko.md#서양배-탈의실">서양배 탈의실</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#종이-오리기-콜라주"><img src="assets/showcase/tiles/blue-collage.jpg" alt="종이 오리기 콜라주"></a><br><sub><a href="SHOWCASE.ko.md#종이-오리기-콜라주">종이 오리기 콜라주</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#스티커-자국-타이포그래피-포스터"><img src="assets/showcase/tiles/sticker-type-poster.jpg" alt="스티커 자국 타이포그래피 포스터"></a><br><sub><a href="SHOWCASE.ko.md#스티커-자국-타이포그래피-포스터">스티커 자국 타이포그래피 포스터</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#픽셀-아트-흰-고양이-포스터"><img src="assets/showcase/tiles/pixel-white-cat.jpg" alt="픽셀 아트 흰 고양이 포스터"></a><br><sub><a href="SHOWCASE.ko.md#픽셀-아트-흰-고양이-포스터">픽셀 아트 흰 고양이 포스터</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#원앙-고전-거장풍-유화"><img src="assets/showcase/tiles/baroque-mandarin-ducks.jpg" alt="원앙, 고전 거장풍 유화"></a><br><sub><a href="SHOWCASE.ko.md#원앙-고전-거장풍-유화">원앙, 고전 거장풍 유화</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#어부와-펠리컨-카라바조풍"><img src="assets/showcase/tiles/caravaggio-pelican.jpg" alt="어부와 펠리컨, 카라바조풍"></a><br><sub><a href="SHOWCASE.ko.md#어부와-펠리컨-카라바조풍">어부와 펠리컨, 카라바조풍</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#탁구-경기-카라바조풍"><img src="assets/showcase/tiles/caravaggio-ping-pong.jpg" alt="탁구 경기, 카라바조풍"></a><br><sub><a href="SHOWCASE.ko.md#탁구-경기-카라바조풍">탁구 경기, 카라바조풍</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#쑤저우-정원의-원앙-인상파-유화"><img src="assets/showcase/tiles/impressionist-suzhou-garden.jpg" alt="쑤저우 정원의 원앙, 인상파 유화"></a><br><sub><a href="SHOWCASE.ko.md#쑤저우-정원의-원앙-인상파-유화">쑤저우 정원의 원앙, 인상파 유화</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#태양-중세-채식-필사본"><img src="assets/showcase/tiles/illuminated-manuscript-a.jpg" alt="태양, 중세 채식 필사본"></a><br><sub><a href="SHOWCASE.ko.md#태양-중세-채식-필사본">태양, 중세 채식 필사본</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#옥토끼-중세-채식-필사본"><img src="assets/showcase/tiles/illuminated-manuscript-b.jpg" alt="옥토끼, 중세 채식 필사본"></a><br><sub><a href="SHOWCASE.ko.md#옥토끼-중세-채식-필사본">옥토끼, 중세 채식 필사본</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#우주정거장-수리-둔황-벽화"><img src="assets/showcase/tiles/dunhuang-space-station.jpg" alt="우주정거장 수리, 둔황 벽화"></a><br><sub><a href="SHOWCASE.ko.md#우주정거장-수리-둔황-벽화">우주정거장 수리, 둔황 벽화</a></sub></td>
</tr>
<tr>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#펠리컨-그림자극"><img src="assets/showcase/tiles/shadow-puppet-pelican.jpg" alt="펠리컨 그림자극"></a><br><sub><a href="SHOWCASE.ko.md#펠리컨-그림자극">펠리컨 그림자극</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#회로와-꽃-공필화-직물-문양"><img src="assets/showcase/tiles/gongbi-circuit-textile.jpg" alt="회로와 꽃, 공필화 직물 문양"></a><br><sub><a href="SHOWCASE.ko.md#회로와-꽃-공필화-직물-문양">회로와 꽃, 공필화 직물 문양</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#거울-앞의-펠리컨-공필화"><img src="assets/showcase/tiles/gongbi-pelican-mirror.jpg" alt="거울 앞의 펠리컨, 공필화"></a><br><sub><a href="SHOWCASE.ko.md#거울-앞의-펠리컨-공필화">거울 앞의 펠리컨, 공필화</a></sub></td>
<td align="center" valign="top" width="25%"><a href="SHOWCASE.ko.md#금빛-불꽃-동양-판타지-일러스트"><img src="assets/showcase/tiles/eastern-fantasy-lineart.jpg" alt="금빛 불꽃, 동양 판타지 일러스트"></a><br><sub><a href="SHOWCASE.ko.md#금빛-불꽃-동양-판타지-일러스트">금빛 불꽃, 동양 판타지 일러스트</a></sub></td>
</tr>
</table>

이미지를 선택하면 큰 이미지와 프롬프트를 볼 수 있습니다.
<!-- END showcase-grid -->

## 온라인 사용

| | 글로벌 | 중국 |
| --- | --- | --- |
| 웹 앱 | [hailuoai.video](https://hailuoai.video/) | [hailuoai.com](https://hailuoai.com/) |
| 데스크톱 앱 | [agent.minimax.io](https://agent.minimax.io/) | [agent.minimax.cn](https://agent.minimax.cn) |
| API 플랫폼 | [platform.minimax.io](https://platform.minimax.io/docs/guides/image-generation) | [platform.minimax.cn](https://platform.minimax.cn/docs/guides/image-generation) |
| API 레퍼런스 | [텍스트-이미지 생성](https://platform.minimax.io/docs/api-reference/image-generation-h3-generations) · [이미지 편집](https://platform.minimax.io/docs/api-reference/image-generation-h3-edits) · [프롬프트 확장](https://platform.minimax.io/docs/api-reference/image-generation-h3-context-ir) | [텍스트-이미지 생성](https://platform.minimax.cn/docs/api-reference/image-generation-h3-generations) · [이미지 편집](https://platform.minimax.cn/docs/api-reference/image-generation-h3-edits) · [프롬프트 확장](https://platform.minimax.cn/docs/api-reference/image-generation-h3-context-ir) |

## 개요

MiniMax-H3-Image는 [MiniMax H3](https://huggingface.co/MiniMaxAI/MiniMax-H3) 계열의 최고 수준 오픈소스 이미지 생성 및 편집 모델로, 텍스트-이미지 생성과 다중 이미지 편집을 하나의 checkpoint에서 수행합니다.

- **실용적인 비용으로 생성하는 16 MP 이미지**: 모든 화면비에서 약 16 MP 이미지를 업스케일러 없이 6 샘플링 스텝으로 직접 생성합니다.
- **풍부한 디테일과 높은 사실감**: 흔히 보는 “AI 느낌”에서 벗어난 이미지를 생성합니다.
- **오픈소스 모델 가운데 가장 강력한 지시 이행**: 최대 16장의 참조 이미지를 지원합니다.

### 사양

MiniMax API의 사양입니다. 로컬 서버의 필드는 [요청 파라미터](#요청-파라미터)를 참고하세요.

| 파라미터 | 사양 |
| --- | --- |
| 모델 ID | `MiniMax-H3-Image` |
| 작업 | 텍스트-이미지 생성, 이미지 편집 |
| 이미지 크기 | `width` + `height` 또는 `area` + `aspect_ratio`로 지정합니다. 기본값은 `auto`이며, 4K 면적에 화면비를 자동으로 정합니다 |
| 출력 면적 | `1K`, `2K` 또는 **`4K`(가장 좋은 결과 👍)**. `width` × `height`를 직접 지정하면 655,360~20,000,000 픽셀 범위를 지원합니다 |
| 화면비 | 1:3~3:1 |
| 프롬프트 | 최대 32,000자이며, 4,096 토큰을 넘는 부분은 잘립니다 |
| 참조 이미지 | 최대 16장. 각 이미지는 64 MiB 이하, 변의 길이 128~8192 픽셀, 화면비 1:4~4:1이어야 합니다 |
| 참조 이미지 형식 | JPG, PNG, WebP, HEIC, HEIF. HTTP(S) URL, Base64 또는 MiniMax 파일 ID로 보냅니다 |
| 요청당 이미지 수 | 1~10장 |
| 프롬프트 확장 | 텍스트-이미지 생성에서는 기본으로 켜져 있으며 끌 수 있고, 이미지 편집에서는 항상 켜져 있습니다. 확장된 프롬프트를 반환받을 수 있습니다 |
| 출력 | PNG(기본값), JPEG 또는 WebP이며, `output_compression`은 0~100입니다. URL(기본값) 또는 Base64로 반환합니다 |
| 아직 지원하지 않는 기능 | 마스크 기반 인페인팅, 투명 배경, 사용자 지정 seed, 미리보기 이미지 |

### 모델 목록

| 모델 | 역할 | 정밀도 | 크기 | Hugging Face |
| --- | --- | --- | --- | --- |
| **MiniMax-H3-Image** | 텍스트-이미지 생성 및 이미지 편집 | BF16 (DiT) | 68.65 GB | [MiniMaxAI/MiniMax-H3-Image](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image) |
| **MiniMax-H3-Image-PE** (선택 사항) | 텍스트-이미지 생성용 프롬프트 확장 모델 | NVFP4 | 17.9 GB | [MiniMaxAI/MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE) |

### 모델 아키텍처

MiniMax-H3-Image는 H3-Base 설계에서 오디오 브랜치를 제거한 구조를 따릅니다. 텍스트 프롬프트와 참조 이미지는 H3 텍스트 인코더로 인코딩되며, 참조 이미지는 이미지 VAE로도 인코딩됩니다. 모든 토큰은 하나의 패킹된 시퀀스를 이루어 단일 스트림 Transformer에 입력되고, Transformer는 목표 이미지의 latent를 예측합니다. VAE는 이 latent를 디코딩해 이미지를 만듭니다.

- **텍스트 인코더**: MiniMax-H3의 Qwen3-VL 텍스트 인코더 전체를 변경 없이 사용합니다. DiT는 이 인코더의 50번째 레이어 hidden state를 읽습니다.
- **이미지 VAE**: CNN 인코더와 2D ViT 디코더(24개 레이어)로 구성되며, 공간 다운샘플링 계수는 16x, latent 채널은 24개입니다. DiT는 2x2 패치로 latent를 patchify하므로 Transformer 토큰 하나가 32x32 픽셀에 해당합니다.
- **확산 Transformer**: 33.1B 파라미터의 dense 단일 스트림 Transformer로, 50개 레이어(hidden size 5376, 어텐션 헤드 56개, FFN 크기 14336)와 3D 멀티모달 RoPE를 사용하며 H3-Omni-Transformer와 같은 구조입니다. 가중치는 BF16이고, 임베딩 레이어, timestep 레이어, 출력 레이어는 FP32입니다.

## 로컬 실행

### 다운로드

| 구성 요소 | 내용 | 크기 |
| --- | --- | --- |
| `transformer/` | DiT 가중치. | 66.28 GB |
| `pdd_fused_heads.safetensors`, `pdd_config.json` | Transformer의 출력 레이어를 대체하는 스텝별 출력 헤드와 샘플링 스케줄입니다. | 12 MB |
| `vae/` | 이미지 VAE, FP32. | 2.34 GB |
| `tokenizer/`, `processor/` | MiniMax-H3와 동일한 Qwen3-VL tokenizer 및 processor입니다. | 23 MB |
| 텍스트 인코더 | 원본 checkpoint에는 포함되어 있지 않습니다. `model_index.json`이 [`MiniMaxAI/MiniMax-H3`](https://huggingface.co/MiniMaxAI/MiniMax-H3)의 `text_encoder/` 폴더에서 불러옵니다. MiniMax-H3를 이미 받아 두었다면 다시 다운로드하지 않습니다. | 66.7 GB |

Hugging Face 저장소에는 이 원본 checkpoint와 diffusers 형식이 함께 올라가 있으며 전체 용량은 약 204 GB입니다. SGLang과 vLLM-Omni에는 원본 checkpoint와 MiniMax-H3 텍스트 인코더만 필요하며, 합계 약 135 GB입니다:

```bash
hf download MiniMaxAI/MiniMax-H3-Image model_index.json "pdd_*" "processor/*" "tokenizer/*" \
  "transformer/*" "vae/*"
hf download MiniMaxAI/MiniMax-H3 --include "text_encoder/*"
# optional prompt expander
hf download MiniMaxAI/MiniMax-H3-Image-PE
```

diffusers는 `ModularPipeline.from_pretrained("MiniMaxAI/MiniMax-H3-Image")`로 필요한 파일을 직접 가져옵니다.

### 배포

모델 서빙에는 다음 추론 프레임워크를 권장합니다:

- [SGLang](https://docs.sglang.io/) - [cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3-Image) 참고
- [vLLM-Omni](https://github.com/vllm-project/vllm-omni) - [vllm-omni 레시피](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image) 참고
- [diffusers](https://github.com/huggingface/diffusers) - [diffusers 문서](https://huggingface.co/docs/diffusers/main/en/api/pipelines/minimax_h3_image) 참고
- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) - [Comfy 튜토리얼](https://docs.comfy.org/tutorials/image/minimax/minimax-h3-image) 참고, [T2I 템플릿](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/image_minimax_h3_image_t2i.json) / [Edit 템플릿](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/image_minimax_h3_image_edit.json) 사용

#### SGLang

main 브랜치에서 SGLang과 diffusion 의존성을 설치합니다([설치 가이드](https://docs.sglang.io/docs/sglang-diffusion/installation) 참고):

```bash
git clone https://github.com/sgl-project/sglang.git
cd sglang
python3 -m pip install -e 'python[diffusion]'
```

GPU 1개에서 서버를 시작할 수 있으며(가용 메모리가 130 GiB 미만이면 SGLang이 일부 모델 구성 요소를 오프로드합니다), 지연 시간을 줄이려면 시퀀스 병렬화(Ulysses)로 각 요청을 여러 GPU에 나누어 처리합니다:

```bash
sglang serve --model-path MiniMaxAI/MiniMax-H3-Image --host 0.0.0.0 --port 30000 --warmup-mode off
# 4 GPUs
sglang serve --model-path MiniMaxAI/MiniMax-H3-Image --host 0.0.0.0 --port 30000 --warmup-mode off \
  --num-gpus 4 --ulysses-degree 4
```

로컬에 있는 MiniMax-H3 텍스트 인코더를 사용하려면 `--text-encoder-path <path to text_encoder>`를 추가하세요. [SGLang cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3-Image)에는 B300부터 12 GB 카드까지 다른 GPU용 레시피가 있습니다.

#### vLLM-Omni

vLLM 0.33.0을 설치한 뒤 vLLM-Omni를 소스에서 설치합니다:

```bash
uv venv --python 3.12 --seed && source .venv/bin/activate
uv pip install vllm==0.33.0 --torch-backend=cu130
git clone https://github.com/vllm-project/vllm-omni.git && cd vllm-omni && uv pip install -e .
```

시퀀스 병렬화(Ulysses)로 GPU 4개를 사용하거나 GPU 1개로 서빙합니다. B200, B300은 약 135 GiB 메모리에 모델 전체를 올리고, H200 1개에서는 텍스트 인코더를 오프로드합니다:

```bash
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 \
  --num-gpus 4 --usp 4 --text-encoder-tp-size 4
# one B200 or B300
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 --num-gpus 1
# one H200: offload the text encoder
vllm serve MiniMaxAI/MiniMax-H3-Image --omni --host 0.0.0.0 --port 8000 --num-gpus 1 \
  --diffusion-offload-config '{"mode":"layer","components":["text_encoder"]}'
```

AMD Instinct 등 다른 GPU의 구성은 [vLLM-Omni 레시피](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image)를 참고하세요.

### 요청 파라미터

SGLang에서 텍스트-이미지 생성 요청은 JSON으로 `/v1/images/generations`에, 이미지 편집 요청은 multipart form data로 `/v1/images/edits`에 보냅니다. 두 요청 모두 `data[0].b64_json`으로 PNG를 반환합니다. vLLM-Omni는 필드가 조금 다르므로 [레시피](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3-Image)를 참고하세요.

| 필드 | 텍스트-이미지 생성 | 이미지 편집 | 비고 |
| --- | --- | --- | --- |
| `prompt` | 필수 | 필수 | 입력 그대로 사용하며 4096 토큰을 넘으면 잘립니다 |
| `size` | 필수 | 필수 | `WIDTHxHEIGHT`. 반환되는 이미지는 정확히 이 크기입니다. [이미지 크기](#이미지-크기) 참고 |
| `image` | — | 파일 1개 이상 | 업로드 순서대로 프롬프트의 `<Picture 1>`, `<Picture 2>`, ...가 됩니다 |
| `seed` | 권장 | 권장 | 정수 |
| `generator_device` | `cpu` 권장 | `cpu` 권장 | 어느 머신에서든 같은 seed로 같은 초기 노이즈를 얻습니다 |
| `response_format` | `b64_json` | `b64_json` | |
| `min_generation_area` | 선택 | 선택 | 최소 생성 면적(픽셀 단위), 1024-16777216, 기본값 4194304(2048x2048). 이보다 작은 `size`는 같은 화면비의 더 큰 캔버스에서 생성한 뒤 LANCZOS로 원래 크기로 줄입니다. 이 동작을 끄려면 1024를 전달합니다. 아래 표의 모든 크기는 기본값보다 큽니다 |
| `num_inference_steps` | 생략 또는 6 | 생략 또는 6 | 다른 값은 HTTP 400을 반환합니다 |
| `guidance_scale` | 생략 또는 1 | 생략 또는 1 | 다른 값은 HTTP 400을 반환합니다 |
| `negative_prompt` | 지원하지 않음 | 지원하지 않음 | 요청이 거부됩니다 |

### 이미지 크기

실제로 잘 동작하는 범위는 약 4 MP에서 20 MP이며, 대체로 16 MP 전후에서 가장 좋은 결과를 냅니다. 자주 쓰는 16 MP 크기:

| 화면비 | 크기(너비 x 높이) |
| --- | --- |
| 1:1 | 4096x4096 |
| 4:3 / 3:4 | 4736x3552 / 3552x4736 |
| 3:2 / 2:3 | 5024x3360 / 3360x5024 |
| 16:9 / 9:16 | 5472x3072 / 3072x5472 |
| 21:9 | 6272x2688 |

다른 화면비에서는 약 16 MP를 유지하고 가로와 세로를 모두 32의 배수로 맞추세요. [`examples/context_ir.py`](examples/context_ir.py)의 `size_for()`로 계산할 수 있습니다:

```bash
cd MiniMax-H3-Image/examples
python3 -c "from context_ir import size_for; print(size_for('5:4'))"   # 4576x3648
```

### 전체 워크플로

MiniMax API는 생성 전에 **H3-Image-Context-IR**로 어떤 언어로 쓴 짧은 프롬프트든 이미지 전체를 영어로 자세히 설명한 글로 확장합니다. 로컬 서버는 프롬프트를 그대로 사용하므로 아래 예시처럼 먼저 확장해야 합니다. [`examples/`](examples)의 스크립트는 위의 SGLang 서버에서 API 결과를 재현하며, Python 표준 라이브러리만 사용합니다:

```bash
git clone https://github.com/MiniMax-AI/MiniMax-H3-Image.git
cd MiniMax-H3-Image/examples
export MINIMAX_API_BASE="https://api.minimax.io"   # China: https://api.minimax.cn
export MINIMAX_API_KEY="<api-key>"
```

`t2i.py`와 `edit.py`는 `http://127.0.0.1:30000`으로 요청을 보냅니다. 다른 주소를 쓰려면 `--url`을 지정하세요.

#### case-T2I

[`instruction.t2i.txt`](examples/instruction.t2i.txt)를 사용합니다.

<table>
<thead>
<tr><th colspan="2">단계</th><th>요청</th><th>결과</th></tr>
</thead>
<tbody>
<tr><td rowspan="3">프롬프트 향상</td><td>H3-Image-Context-IR (MiniMax API)</td><td><code>python3 context_ir.py t2i</code> (<a href="examples/context_ir.py">스크립트</a>)</td><td><code>revised_prompt.txt</code>, <code>revised_size.txt</code>; 예시 실행 결과: <a href="examples/revised_prompt.t2i.txt"><code>revised_prompt.t2i.txt</code></a>, <a href="examples/revised_size.t2i.txt"><code>revised_size.t2i.txt</code></a> (4736x3552)</td></tr>
<tr><td>로컬 대안: <a href="https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE">MiniMax-H3-Image-PE</a></td><td>PE 저장소의 <code>scripts/expand_prompt.py</code></td><td><code>expanded_caption</code>을 <code>revised_prompt.txt</code>로, <code>aspect_ratio</code>에 해당하는 크기를 <code>revised_size.txt</code>로 저장</td></tr>
<tr><td>에이전트 대안: <a href="#프롬프트-작성-스킬">h3-image-prompt-writing</a></td><td>스킬을 사용해 <code>instruction.t2i.txt</code>에 대한 프롬프트와 화면비를 작성하도록 에이전트에게 요청</td><td>프롬프트를 <code>revised_prompt.txt</code>로, 해당 화면비의 <a href="#이미지-크기">크기</a>를 <code>revised_size.txt</code>로 저장</td></tr>
<tr><td colspan="2">MiniMax-H3-Image 생성: 로컬 SGLang</td><td><code>python3 t2i.py --prompt revised_prompt.txt --size $(cat revised_size.txt)</code> (<a href="examples/t2i.py">스크립트</a>)</td><td><code>t2i.png</code></td></tr>
<tr><td colspan="2">E2E API 참조: MiniMax API 직접 호출로 수행한 텍스트-이미지 생성</td><td><code>python3 api_generate.py t2i</code> (<a href="examples/api_generate.py">스크립트</a>)</td><td><code>api_t2i.png</code></td></tr>
</tbody>
</table>

<p align="center">
<img src="assets/workflow_t2i.jpg" alt="왼쪽: 향상된 프롬프트로 로컬 SGLang에서 생성한 t2i.png. 오른쪽: MiniMax API에서 생성한 api_t2i.png. 두 이미지 모두 낡은 나무 테이블 위에 빵, 채소, 치즈가 차려진 팜투테이블 만찬을 위에서 내려다본 장면" width="100%"/>
</p>
<p align="center"><em>로컬 SGLang에서 생성한 t2i.png(왼쪽)와 MiniMax API에서 생성한 api_t2i.png(오른쪽), 4736x3552(H3-Image-Context-IR이 선택한 4:3)</em></p>

#### case-Edit

[`instruction.edit.txt`](examples/instruction.edit.txt)를 사용하며,
참조 이미지 [`reference1.png`](examples/reference1.png)를
`<Picture 1>`로 지정합니다.

| 단계 | 요청 | 결과 |
| --- | --- | --- |
| 프롬프트 향상: H3-Image-Context-IR (MiniMax API) | `python3 context_ir.py edit` ([스크립트](examples/context_ir.py)) | `revised_prompt.txt`, `revised_size.txt`; 예시 실행 결과: [`revised_prompt.edit.txt`](examples/revised_prompt.edit.txt), [`revised_size.edit.txt`](examples/revised_size.edit.txt) (4096x4096) |
| 프롬프트 향상, 에이전트 대안: [h3-image-prompt-writing](#프롬프트-작성-스킬) | 스킬을 사용해 `reference1.png`에 맞게 `instruction.edit.txt`를 다시 쓰도록 에이전트에게 요청 | 프롬프트를 `revised_prompt.txt`로, `4096x4096`을 `revised_size.txt`로 저장 |
| MiniMax-H3-Image 생성: 로컬 SGLang | `python3 edit.py --prompt revised_prompt.txt --size $(cat revised_size.txt)` ([스크립트](examples/edit.py)) | `edit.png` |
| E2E API 참조: MiniMax API 직접 호출로 수행한 이미지 편집 | `python3 api_generate.py edit` ([스크립트](examples/api_generate.py)) | `api_edit.png` |

<p align="center">
<img src="assets/workflow_edit.jpg" alt="왼쪽: 남성이 헤드폰을 쓰고 있는 팟캐스트 진행자 두 명의 참조 이미지 reference1.png. 가운데: 향상된 프롬프트로 로컬 SGLang에서 생성한 edit.png. 오른쪽: MiniMax API에서 생성한 api_edit.png. 두 결과 모두 헤드폰이 사라지고 두 진행자가 MONEY TALKS 표지판 위에서 주먹을 맞대고 있음" width="100%"/>
</p>
<p align="center"><em>참조 이미지 reference1.png(왼쪽), 로컬 SGLang에서 생성한 edit.png(가운데), MiniMax API에서 생성한 api_edit.png(오른쪽), 4096x4096(H3-Image-Context-IR이 선택한 1:1)</em></p>

## 프롬프트 작성 팁

공식 사용자 가이드의 팁으로, MiniMax API와 로컬 서버 모두에 적용됩니다. [프롬프트 작성 스킬](#프롬프트-작성-스킬)은 이 팁에 따라 프롬프트를 작성합니다.

- **스타일보다 작업을, 세부 사항보다 레이아웃을 먼저 씁니다.** 이미지의 용도와 내용, 그다음 레이아웃을 쓰고, 스타일은 "고급스러운 느낌" 같은 말 대신 색상, 재질, 조명 같은 눈에 보이는 디테일로 표현합니다.
- **표시할 텍스트는 모두 따옴표로 씁니다.** 위치와 줄바꿈도 지정하고, 텍스트가 필요 없으면 "이미지에 텍스트, 문자, 숫자를 넣지 않음"이라고 씁니다.
- **차트와 교육용 이미지에는 정확한 데이터를 제공합니다.** 단위와 기간을 쓰고, 예시 데이터는 그렇다고 명시합니다.
- **참조 이미지마다 역할을 지정합니다.** 바뀌는 것과 유지되는 것도 씁니다. 예: "왼쪽 컵을 파란색으로 바꾸고, 모양, 재질, 위치, 크기는 그대로 유지."
- **그리드는 행과 열로 지정합니다.** "2×3"이 아니라 "2행 3열"처럼 씁니다.

## 라이선스

- MiniMax-H3-Image는 [MiniMax-H3-Image Community License Agreement](LICENSE)에 따라 배포됩니다.
- T2I PE 모델([MiniMax-H3-Image-PE](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image-PE))은 MiniMax-H3-Image의 일부이므로 마찬가지로 [MiniMax-H3-Image Community License Agreement](LICENSE)가 적용됩니다.
- 라이선스 제IV조에 명시된 별도의 서면 승인은 [신청서](https://platform.minimax.io/console/license)를 통해 요청합니다.

## 문의

[model@minimax.io](mailto:model@minimax.io)로 문의해 주세요.
