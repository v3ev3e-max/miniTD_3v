# 최우선 그래픽 에셋 (플레이 중 최다 노출 15종)

이 문서는 `index.html`의 실제 코드(`TOWER_DEFS`, `ENEMY_TYPES`, 투사체 렌더링 코드)만을 근거로 추출했으며, 추측으로 채운 항목은 없습니다.

**선정 기준**: 웨이브 제한(`unlockWave`) 없이 초반부터 사용 가능한지, 비용이 낮아 대량으로 지어지는지(타워), 스폰 가중치 `weight`가 높은지(적), 실제 렌더링 코드에서 몇 개의 타워가 공유해서 쓰는 발사체인지(투사체) — 즉 "게임 화면에 실제로 얼마나 자주 그려지는가"를 코드 수치로 판단했습니다.

기존 이름 / 능력 / 밸런스 / 게임성은 전혀 건드리지 않으며, 아래는 **외형 개선용 이미지 에셋**입니다.

---

# 타워

우선순위 근거: 5종 모두 `unlockWave`가 없어 게임 시작부터 사용 가능하고, 16종 타워 중 비용이 가장 낮은 축(100~2,000골드)이라 한 판에서 가장 많이 건설·노출됩니다.

## 기본 (basic)

파일명:
basic.png

사용 목적:
모든 플레이어가 게임 시작과 동시에 짓는 1티어 기본 공격 타워 (비용 100골드, 공격력 14, 사거리 95, 특수능력 없음). 초반 화력의 근간이자 게임 전체에서 가장 많이 배치되는 타워.

AI 생성 프롬프트:

Top-down tower defense turret,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a compact single-barrel automated gun turret on a rotating round base, simple sturdy chassis with a muzzle brake tip, small blue-tinted muzzle flash glow, primary color #378ADD with dark accents #185FA5 — reliable, no-frills starter weapon silhouette

## 저격 (sniper)

파일명:
sniper.png

사용 목적:
전체 타워 중 최장 사거리(180)를 가진 단일 대상 정밀 공격 타워 (비용 250골드, 공격력 38, 지상/공중 모두 공격 가능). 저비용에 언락 조건이 없어 초반부터 다수 배치되는 핵심 타워.

AI 생성 프롬프트:

Top-down tower defense turret,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

긴 총열(long slender rifled barrel), 고배율 스코프(high-magnification scope with glowing lens reticle), 정밀 사격 구조(precision sniper chassis), 금속 삼각대(metal tripod/bipod stabilizer legs), 레이저 거리측정기(laser rangefinder beam emitter on the scope) — primary color #6C4FD1 with dark accents #3D2A8C

## 기관총 (gatling)

파일명:
gatling.png

사용 목적:
초당 공격속도가 가장 빠른(rate 100ms) 다연장 속사 타워 (비용 500골드, 공격력 18). 저체력 다수 몹을 빠르게 정리하는 실전형 화력의 핵심.

AI 생성 프롬프트:

Top-down tower defense turret,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

회전 다연장 총열(rotating multi-barrel cluster), 탄띠 급탄 장치(ammo belt feeding from a side ammo box), 고속 사격 구조(rapid-fire mechanism with visible spin blur), 과열 배기관(overheating exhaust vents releasing heat haze) — primary color #8A8F98 with dark accents #4A4F57

## 폭발 (explosive)

파일명:
explosive.png

사용 목적:
스플래시 범위 피해(splash 70)를 가진 근접 광역 타워 (비용 1,200골드, 공격력 80). 밀집한 몹 무리를 한 번에 처리하는 초중반 핵심 광역기.

AI 생성 프롬프트:

Top-down tower defense turret,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

박격포 구조(mortar-style lobbing barrel), 폭탄 저장고(visible bomb/shell rack), 화약통(gunpowder keg strapped to the chassis), 중장갑 포신(heavily reinforced blast-proof barrel plating) — primary color #E0672B with dark accents #93401A

## 냉기 (frost)

파일명:
frost.png

사용 목적:
적 이동속도를 50% 감소시키는(slow 0.5, 1.7초 지속) 제어형 타워 (비용 2,000골드, 공격력 44). 다른 타워의 화력 집중 시간을 벌어주는 필수 유틸리티 타워.

AI 생성 프롬프트:

Top-down tower defense turret,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

얼음 결정(jagged translucent ice crystal formations), 서리 이펙트(frost mist swirling around the barrel), 냉각 코어(glowing frozen core at the center) — primary color #29B6C6 with dark accents #146B75

---

# 적

우선순위 근거: `ENEMY_TYPES`의 `weight`(스폰 가중치) 상위 5종이며, 전부 웨이브 13 이전에 해금되어 게임 대부분의 구간에서 지속적으로 등장합니다.

## 일반 (normal)

파일명:
normal.png

사용 목적:
웨이브 1부터 등장(weight 50, 전체 최고 가중치), 체력·속도 배율 모두 1.0으로 특수 능력이 전혀 없는 기준 몹. 모든 웨이브 구성의 뼈대이자 화면에 가장 많이 등장하는 개체.

AI 생성 프롬프트:

Top-down enemy game character,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a small round basic blob creature, plain and unassuming silhouette with no special features — primary color #F0997B with dark accents #712B13

## 중장갑 (armored)

파일명:
armored.png

사용 목적:
체력 2.3배·속도 절반(hp 2.3, speed 0.55)의 탱커형 몹, 웨이브 4부터 등장(weight 20, 2위). 관통포 외 모든 타워의 데미지가 40% 감소하는 저항 특성.

AI 생성 프롬프트:

Top-down enemy game character,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

두꺼운 장갑(thick riveted metallic beetle-shell plating covering the whole body), slow lumbering tanky stance — primary color #8A8F98 with dark accents #4A4F57

## 돌진 (rush)

파일명:
rush.png

사용 목적:
체력 절반·속도 1.9배(hp 0.5, speed 1.9)의 고속 돌파형 몹, 웨이브 6부터 등장(weight 18, 3위). 빠르게 처치하지 못하면 그대로 통과.

AI 생성 프롬프트:

Top-down enemy game character,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

날렵한 실루엣(sleek aerodynamic triangular body leaning forward as if sprinting), motion streak trails behind it conveying high speed — primary color #FF6B4A with dark accents #B23A22

## 재생 (regen)

파일명:
regen.png

사용 목적:
초당 체력 2% 자연 회복(hp 0.9, speed 1.0)하는 지속형 몹, 웨이브 9부터 등장(weight 14, 공동 4위). 화력을 끊임없이 집중하지 않으면 다시 차오름.

AI 생성 프롬프트:

Top-down enemy game character,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

녹색 재생 에너지(pulsing green regenerative energy glowing through organic veins on a round blob body) — primary color #7ED957 with dark accents #3E7A28

## 분열 (split)

파일명:
split.png

사용 목적:
사망 시 약한 자식 2마리로 분열(hp 0.75, speed 1.0)하는 몹, 웨이브 13부터 등장(weight 14, 공동 4위). 처치해도 위협이 완전히 사라지지 않음.

AI 생성 프롬프트:

Top-down enemy game character,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

분열 가능한 생체 구조(peanut-shaped body with a visible glowing dividing seam down the middle, straining as if about to split in two) — primary color #C77DD9 with dark accents #7A3E8C

---

# 투사체

**실제 코드 확인 사항**: 16종 타워 중 기본/기관총/미사일터렛/폭발/냉기/광전사/관통포/독/플라즈마/초신성 10종은 전부 `G.projectiles`의 **동일한 원형 발사체 객체 하나를 공유**하며 `t.dark` 색상으로만 구분됩니다 (즉 미사일·독구름·플라즈마 전용 발사체는 코드상 존재하지 않습니다 — 전부 "일반 발사체" 항목이 담당). 저격/관통저격수/레이저/번개 4종만 `G.lasers` 즉발 라인으로 별도 렌더링됩니다. 아래 5종이 실제 코드에 존재하는 투사체 자산의 전부입니다(블랙홀 흡입장은 발사체가 아닌 지속 필드라 이번 우선순위에서 제외).

## 일반 발사체 (bullet)

파일명:
bullet.png

사용 목적:
기본/기관총/미사일터렛/폭발/냉기/광전사/관통포/독/플라즈마/초신성 — 16종 중 10종이 공유하는 이동형 발사체. 한 웨이브에서 압도적으로 가장 많이 그려지는 단일 시각 오브젝트.

AI 생성 프롬프트:

Top-down tower defense projectile,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a small glowing energy bullet/orb with a soft radiant outer glow trail and bright hot core, neutral bright color with white-yellow core (tinted per-tower in-game)

## 저격 빔 (sniperBeam)

파일명:
sniperBeam.png

사용 목적:
저격 타워 전용 즉발 히트스캔 라인 이펙트. 저격 타워가 저비용·무제한 사용 가능이라 게임 내내 자주 발사됨.

AI 생성 프롬프트:

Top-down tower defense projectile,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a thin razor-sharp instant-hit precision energy beam streak with a bright glowing core and purple tint, crisp edges conveying pinpoint accuracy, horizontal beam texture stretchable along its length

## 번개 체인 (lightningChain)

파일명:
lightningChain.png

사용 목적:
번개 타워 전용, 최대 5타겟까지 연쇄로 튀는 전기 이펙트. 중간 비용대 타워로 중후반 내내 자주 등장.

AI 생성 프롬프트:

Top-down tower defense projectile,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a jagged crackling electric-yellow lightning bolt arc with branching micro-sparks along its jagged path, zigzag beam texture stretchable along its length

## 레이저 빔 (laserBeam)

파일명:
laserBeam.png

사용 목적:
레이저 타워 전용, 사거리 방향 일직선의 모든 적을 동시에 관통하는 연속 빔. 고비용 타워지만 시각적 임팩트가 가장 크고 게임의 상징적 이펙트.

AI 생성 프롬프트:

Top-down tower defense projectile,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a wide continuous searing red energy laser beam with an intense glowing core and radiant outer bloom, horizontal beam texture stretchable along its length

## 관통저격 빔 (pierceSniperBeam)

파일명:
pierceSniperBeam.png

사용 목적:
관통저격수 전용, 최대 2명까지 관통하는 상위 히트스캔 빔. 저격 계열의 강화판으로 중반 이후 자주 등장.

AI 생성 프롬프트:

Top-down tower defense projectile,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
premium game asset,
stylized AAA mobile game art,
vivid lighting,
strong highlights,
clean readable silhouette,
detailed mechanical parts,
visual effects integrated,
transparent background,
PNG asset,
512x512,
professional game icon quality,
Top Down,
Transparent Background,
Mobile Game Quality,

a thicker piercing energy beam streak in vivid sky blue punching through and continuing past multiple targets, energy fracture lines along its length, horizontal beam texture stretchable along its length

---

# 가장 먼저 생성해야 하는 10개 이미지 (TOP10)

기준: ① 게임 화면 노출 빈도 → ② 시각적 임팩트 → ③ 그래픽 개선 효과(현재 도형이 얼마나 단순한지) 순으로 정렬.

| 순위 | 항목 | 파일명 | 선정 이유 |
|---|---|---|---|
| 1 | 일반 발사체 | projectiles/bullet.png | 10종 타워가 공유, 웨이브당 등장 수 자체가 압도적으로 많음 |
| 2 | 일반 몹 | enemies/normal.png | weight 50(전체 최고), 웨이브 1부터 매 웨이브 등장 |
| 3 | 기본 타워 | towers/basic.png | 모든 플레이어가 가장 먼저, 가장 많이 짓는 타워 |
| 4 | 중장갑 몹 | enemies/armored.png | weight 20(2위), 현재 단순 사각형이라 개선 효과 큼 |
| 5 | 저격 타워 | towers/sniper.png | 저비용·무제한이라 노출 빈도 매우 높음 |
| 6 | 돌진 몹 | enemies/rush.png | weight 18(3위), 역동적 실루엣으로 개선 임팩트 큼 |
| 7 | 기관총 타워 | towers/gatling.png | 저비용·상시 사용, 회전 총열 디테일 개선 효과 큼 |
| 8 | 저격 빔 | projectiles/sniperBeam.png | 저격 타워와 함께 매우 자주 발사됨 |
| 9 | 재생 몹 | enemies/regen.png | weight 14(공동 4위), 발광 이펙트로 개선 임팩트 큼 |
| 10 | 폭발 타워 | towers/explosive.png | 초중반 핵심 광역 타워, 박격포/폭발 이펙트 개선 효과 큼 |
