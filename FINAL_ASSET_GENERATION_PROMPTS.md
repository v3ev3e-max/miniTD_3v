# 최종 에셋 생성 프롬프트 (TOP 15)

`TOP_PRIORITY_ASSETS.md`에서 선정한 15개 에셋(타워 5 / 적 5 / 투사체 5)을 실제 이미지 생성 모델에 바로 입력할 수 있는 Positive/Negative 프롬프트로 재작성했습니다.

**파일명, 타워/적 이름, 능력, 밸런스, 게임 컨셉은 전혀 변경하지 않았습니다.** 이 문서는 순수 외형(그래픽) 생성용입니다.

## 지원 모델별 사용법

- **Midjourney / Stable Diffusion XL / Flux Dev**: Positive Prompt를 쉼표로 구분된 태그 그대로 입력하고, Negative Prompt는 `--no` 파라미터(Midjourney) 또는 SDXL/Flux의 negative prompt 필드에 그대로 입력하면 됩니다.
- **ChatGPT Image Generation**: 쉼표 목록을 자연스러운 한 문단으로 읽어도 동일하게 작동합니다. Negative Prompt는 "다음 요소는 제외해줘"라는 문장으로 덧붙이면 됩니다 (ChatGPT는 별도 negative 필드가 없음).
- **Flux Kontext**: 기존 이미지를 편집/합성하는 모델이므로, 신규 생성 시에는 Positive Prompt를 그대로 텍스트-투-이미지 입력으로 사용하고, 추후 특정 타워의 변형(예: 업그레이드 이펙트 추가)이 필요할 때 Kontext의 참조 이미지 입력에 같은 Positive Prompt를 컨텍스트로 덧붙여 사용하세요.

모든 Positive Prompt는 `Top Down`, `Transparent Background`, `PNG Asset`, `Mobile Game Quality`, `Professional Game Asset`을 반드시 포함합니다.

---

# 타워

## 기본 타워 (basic)

파일명:
basic.png

Positive Prompt:

Top-down tower defense turret,
balanced all-purpose mechanical cannon,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
blue and steel construction,
animated energy core glowing in the central hub,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
compact rotating turret base, single sturdy barrel with a muzzle brake tip, reliable no-frills starter weapon silhouette, primary color #378ADD with dark accents #185FA5

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple towers,
UI elements,
frame,
border

## 저격 타워 (sniper)

파일명:
sniper.png

Positive Prompt:

Top-down tower defense turret,
precision long-range sniper cannon,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
purple anodized steel and matte black barrel construction,
animated glowing scope reticle with active laser rangefinder beam,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
초장거리 총열 (extra-long slender rifled barrel), 고배율 스코프 (high-magnification scope mounted on top), 삼각대 (metal tripod/bipod stabilizer legs), 정밀 사격 구조 (precision marksman chassis), primary color #6C4FD1 with dark accents #3D2A8C

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple towers,
UI elements,
frame,
border

## 기관총 타워 (gatling)

파일명:
gatling.png

Positive Prompt:

Top-down tower defense turret,
rapid-fire multi-barrel mechanical cannon,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
gunmetal steel construction,
animated spinning barrel motion blur with glowing heat-vent exhaust,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
회전 다연장 총열 (rotating multi-barrel cluster bundled together), 탄띠 급탄 (ammo belt feeding from a side-mounted ammo box), 과열 배기관 (overheating exhaust vents releasing heat haze), primary color #8A8F98 with dark accents #4A4F57

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple towers,
UI elements,
frame,
border

## 폭발 타워 (explosive)

파일명:
explosive.png

Positive Prompt:

Top-down tower defense turret,
heavy mortar-type mechanical cannon,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
reinforced orange-painted steel construction,
animated smoldering fuse spark with faint smoke wisps,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
박격포 (mortar-style lobbing barrel angled upward), 폭탄 저장고 (visible bomb/shell loaded in the breech), 화약통 (gunpowder keg strapped to the side of the chassis), primary color #E0672B with dark accents #93401A

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple towers,
UI elements,
frame,
border

## 냉기 타워 (frost)

파일명:
frost.png

Positive Prompt:

Top-down tower defense turret,
crystalline frost mechanical cannon,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
ice-encrusted cyan steel construction,
animated pulsing frozen core with drifting frost mist,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
얼음 결정 (jagged translucent ice crystal formations built into the barrel), 서리 효과 (frost mist swirling around the emitter), 냉각 코어 (glowing frozen core at the center), primary color #29B6C6 with dark accents #146B75

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple towers,
UI elements,
frame,
border

---

# 적

## 일반 몬스터 (normal)

파일명:
normal.png

Positive Prompt:

Top-down tower defense enemy character,
basic tower defense enemy creature,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed character design,
soft organic body construction,
animated subtle body sheen,
battle-ready menacing appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
가장 기본 실루엣 (small round basic blob-like body, plain and unassuming with no special features, simple and cute but slightly menacing), primary color #F0997B with dark accents #712B13

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple characters,
UI elements,
frame,
border

## 중장갑 몬스터 (armored)

파일명:
armored.png

Positive Prompt:

Top-down tower defense enemy character,
heavily armored tower defense enemy creature,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed character design,
riveted metallic armor construction,
animated metallic plating glint,
battle-ready menacing appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
중장갑 (thick riveted metallic beetle-shell plating covering the entire back), 두꺼운 금속 장갑 (heavy reinforced armor plates with visible seams and battle scratches), slow lumbering tanky stance, primary color #8A8F98 with dark accents #4A4F57

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple characters,
UI elements,
frame,
border

## 돌진 몬스터 (rush)

파일명:
rush.png

Positive Prompt:

Top-down tower defense enemy character,
fast sprinting tower defense enemy creature,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed character design,
aerodynamic wind-swept body construction,
animated speed motion trail glow,
battle-ready menacing appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
빠른 이동 구조 (built for high-speed sprinting, leaning forward as if charging), 날렵한 실루엣 (sleek aerodynamic triangular silhouette with motion streaks trailing behind), primary color #FF6B4A with dark accents #B23A22

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple characters,
UI elements,
frame,
border

## 재생 몬스터 (regen)

파일명:
regen.png

Positive Prompt:

Top-down tower defense enemy character,
regenerating tower defense enemy creature,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed character design,
soft organic bioluminescent body construction,
animated pulsing healing glow,
battle-ready menacing appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
녹색 재생 에너지 (pulsing green regenerative energy glowing through organic veins across a round blob body), 회복 오라 (soft healing aura radiating outward from the core), primary color #7ED957 with dark accents #3E7A28

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple characters,
UI elements,
frame,
border

## 분열 몬스터 (split)

파일명:
split.png

Positive Prompt:

Top-down tower defense enemy character,
splitting tower defense enemy creature,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed character design,
soft organic segmented body construction,
animated glowing dividing seam crackle,
battle-ready menacing appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
분열 가능한 생체 구조 (peanut-shaped organic body with a visible glowing dividing seam down the middle, straining as if about to split into two), primary color #C77DD9 with dark accents #7A3E8C

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple characters,
UI elements,
frame,
border

---

# 투사체

## 일반 발사체 (bullet)

파일명:
bullet.png

Positive Prompt:

Top-down tower defense projectile,
premium high-tech ammunition round,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed energy effects,
glowing energy core construction,
animated soft outer glow trail,
compact battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
고급 탄환 (small premium glowing energy bullet/orb with a soft radiant outer glow trail and bright hot core), neutral bright color with a white-yellow core (color is tinted per tower in-game)

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple projectiles,
UI elements,
frame,
border

## 저격 빔 (sniperBeam)

파일명:
sniperBeam.png

Positive Prompt:

Top-down tower defense projectile beam,
ultra-fast precision energy shot,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed energy effects,
glowing purple energy beam construction,
animated crisp instant-hit streak,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
초고속 에너지 탄 (thin razor-sharp instant-hit precision energy beam streak with a bright glowing core and purple tint, crisp edges conveying pinpoint accuracy), horizontal beam texture stretchable along its length

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple projectiles,
UI elements,
frame,
border

## 레이저 빔 (laserBeam)

파일명:
laserBeam.png

Positive Prompt:

Top-down tower defense projectile beam,
powerful continuous straight-line laser,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed energy effects,
glowing red energy beam construction,
animated radiant beam bloom with heat shimmer,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
강력한 직선 레이저 (wide continuous searing red energy laser beam with an intense glowing core and radiant outer bloom, piercing straight through everything in its path), horizontal beam texture stretchable along its length

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple projectiles,
UI elements,
frame,
border

## 번개 체인 (lightningChain)

파일명:
lightningChain.png

Positive Prompt:

Top-down tower defense projectile beam,
chaining electric lightning arc,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed energy effects,
glowing electric-yellow energy construction,
animated crackling spark branches,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
전기 스파크 (crackling micro-sparks branching off a jagged lightning path), 연쇄 번개 (jagged electric-yellow lightning bolt arc connecting two points, conveying a chain jumping between multiple targets), zigzag beam texture stretchable along its length

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple projectiles,
UI elements,
frame,
border

## 관통저격 빔 (pierceSniperBeam)

파일명:
pierceSniperBeam.png

Positive Prompt:

Top-down tower defense projectile beam,
powerful piercing energy penetrator beam,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed energy effects,
glowing sky-blue energy beam construction,
animated piercing energy fracture glow,
battle-ready appearance,
professional mobile game icon,
transparent background,
isolated asset,
Top Down,
Transparent Background,
PNG Asset,
Mobile Game Quality,
Professional Game Asset,
512x512,
ultra detailed,
sharp focus,
강력한 에너지 관통선 (thicker piercing energy beam streak in vivid sky blue that punches through and continues past multiple targets, energy fracture lines along its length), horizontal beam texture stretchable along its length

Negative Prompt:

low quality,
blurry,
realistic photo,
text,
watermark,
logo,
background scenery,
cropped,
cut off,
dark image,
ugly,
distorted,
extra objects,
multiple projectiles,
UI elements,
frame,
border

---

# 가장 먼저 생성해야 할 TOP5

기준: ① 화면 노출 빈도 → ② 시각적 임팩트 → ③ 게임 퀄리티 향상 효과 순.

| 순위 | 항목 | 파일명 | 선정 이유 |
|---|---|---|---|
| 1 | 일반 발사체 | bullet.png | 16종 타워 중 10종이 공유하는 발사체라 한 웨이브 내 등장 횟수 자체가 압도적. 가장 자주 눈에 띄는 단일 오브젝트를 고급 탄환으로 바꾸는 것이 전체 화면 인상을 가장 크게 바꿈 |
| 2 | 일반 몬스터 | normal.png | 스폰 가중치 50(전체 최고)으로 웨이브 1부터 끝까지 항상 화면에 존재. 가장 단순한 도형이라 개선 여지도 가장 큼 |
| 3 | 기본 타워 | basic.png | 모든 플레이어가 가장 먼저, 가장 많이 짓는 타워. 첫인상을 좌우 |
| 4 | 중장갑 몬스터 | armored.png | 스폰 가중치 2위, 현재 단순 사각형 실루엣이라 두꺼운 장갑 디테일 추가 시 개선 효과가 두드러짐 |
| 5 | 저격 타워 | sniper.png | 저비용·무제한 사용 가능으로 노출 빈도가 매우 높고, 긴 총열/스코프 디테일이 추가되면 시각적 임팩트가 큼 |
