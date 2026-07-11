# AI 이미지 생성 프롬프트 모음

이 문서는 `index.html`의 실제 코드(`TOWER_DEFS`, `ENEMY_TYPES`, `BOSS_TYPES`, `FIELD_THEMES`, `ICONS` 등)를 기준으로 추출한 전체 게임 오브젝트 목록과, 각 오브젝트를 AI 이미지 생성기(예: Midjourney, DALL·E, Stable Diffusion)에 넣을 프롬프트입니다.

이미지를 생성한 뒤 지정된 파일명 그대로 해당 `assets/` 하위 폴더에 넣으면, 코드 수정 없이 `AssetManager`가 자동으로 감지해 렌더링에 적용합니다 (없으면 기존 도형 렌더링 유지).

> **파일명 수정 안내**: 이전 버전 문서는 `tower_basic.png`, `ui_speed.png`처럼 폴더명을 파일명에 접두어로 붙였으나, 실제 `AssetManager` 코드는 `assets/<폴더>/<파일명>` 형태(예: `assets/towers/basic.png`, `assets/ui/speed.png` — 접두어 없음)를 찾습니다. 이 문서는 실제 코드에 맞게 파일명을 수정했습니다(접두어 제거). 아래 각 항목의 "파일명"은 해당 카테고리 폴더 안에 그대로 넣을 파일 이름입니다.
>
> **UI 아이콘은 PNG 대신 SVG로 이미 생성되어 있습니다** (`assets/ui/*.svg`, Brawl Stars 스타일). `AssetManager`는 이제 PNG를 먼저 찾고, 없으면 같은 이름의 SVG를 자동으로 대신 사용합니다. 즉 나중에 PNG를 만들어 넣으면 PNG가 우선 적용되고, PNG가 없으면 지금 만든 SVG가 계속 쓰입니다.

공통 지침:
- 배경은 반드시 투명(transparent PNG)
- 시점은 탑다운(top-down) 또는 3/4 쿼터뷰로 통일
- 하나의 오브젝트만 중앙에 배치, 여백 최소화
- 실루엣이 명확해서 축소해도 알아보기 쉬울 것 (readable silhouette)
- 색상은 원작 코드의 `color`/`dark` 값과 일치시킬 것 (아래 각 항목에 헥스코드 표기)
- **품질 기준**: highly polished mobile game art, Clash Royale quality, Brawl Stars quality, stylized AAA mobile game art, premium game asset — 장난감 같은 저채도 도형이 아니라 실제 상업 모바일 게임(클래시 로얄/브롤스타즈)에 바로 쓸 수 있는 수준의 완성도를 요구합니다.
- **라이팅/디테일 기준**: vivid lighting, strong highlights, detailed mechanical parts, visual effects integrated — 광원/하이라이트가 뚜렷하고, 기계 부품(포신·관절·리벳 등)이 구체적으로 묘사되며, 이펙트(빛·연기·스파크 등)가 오브젝트에 자연스럽게 녹아들어야 합니다.
- **타워는 공격 속성이 외형에 드러나야 함**: 각 타워 프롬프트에 해당 타워의 실제 공격 방식(총열 형태, 발사체 종류, 이펙트)을 구체적인 기계 구조로 명시했습니다 (예: 저격=긴 총열+스코프, 기관총=회전 총열+탄띠, 폭발=박격포+화약통, 미사일=로켓 포드, 냉기=얼음 결정, 번개=코일+스파크, 독=독액 탱크+독성 증기, 플라즈마=에너지 코어).

---

# 타워

## 기본 (basic)

파일명:
basic.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a compact automated gun turret on a rotating round base, a single sturdy barrel with a muzzle brake tip, simple but sturdy mechanical silhouette representing a reliable starter weapon,
primary color #378ADD (blue) with dark accents #185FA5,
matching the original tower concept: basic starter turret, single gun barrel, standard rapid-fire attack,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (small muzzle flash glow),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 저격 (sniper)

파일명:
sniper.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a tall precision sniper turret with an extra-long slender rifled barrel, a prominent scope/optic mounted on top with a glowing lens reticle, stabilizing bipod struts at the base, sleek angular chassis conveying long-range precision,
primary color #6C4FD1 (purple) with dark accents #3D2A8C,
matching the original tower concept: long-range precision sharpshooter tower, single devastating precision shot,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (scope lens glint, faint muzzle glow),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 기관총 (gatling)

파일명:
gatling.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a rugged multi-barrel gatling gun turret with a cluster of rotating barrels bundled together, a visible spinning mechanism and feed mechanism, an ammo belt draping from a side-mounted ammo box into the receiver, industrial riveted metal housing,
primary color #8A8F98 (steel gray) with dark accents #4A4F57,
matching the original tower concept: rapid-fire multi-barrel machine gun turret, extremely fast rate of fire,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (motion blur on spinning barrels, spark trails),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 미사일터렛 (missile)

파일명:
missile.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a boxy anti-air missile launcher turret with a multi-tube rocket pod loaded with several guided missiles, visible missile fins and warhead tips peeking from the launch tubes, targeting radar dish on the side, aimed skyward,
primary color #3ADE8F (green) with dark accents #1B6B44,
matching the original tower concept: anti-air only guided missile turret that targets flying enemies exclusively,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (rocket exhaust glow, targeting radar sweep),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 폭발 (explosive)

파일명:
explosive.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a heavy mortar-style cannon turret with a wide short thick barrel angled for lobbing shots, a bulky bomb/shell loaded and visible in the breech, a barrel-shaped gunpowder keg strapped to the side of the chassis, reinforced blast-resistant plating,
primary color #E0672B (orange) with dark accents #93401A,
matching the original tower concept: explosive splash-damage mortar cannon, area-of-effect bombardment,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (smoldering fuse spark, faint smoke wisps),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 냉기 (frost)

파일명:
frost.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a crystalline frost turret built from jagged translucent ice crystal formations, an icy blue barrel encrusted with frost and hanging icicles, a constant chilling frost mist/fog effect swirling around the emitter, frozen crystalline core glowing at the center,
primary color #29B6C6 (cyan) with dark accents #146B75,
matching the original tower concept: slowing frost/ice tower that chills and slows enemies,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (frost mist, ice crystal glint, frozen breath vapor),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 광전사 (berserker)

파일명:
berserker.png

이미지 프롬프트:
Top-down tower defense game turret asset,
an aggressive spiked battle turret bristling with jagged blade-like armor plates, a menacing crimson battle-rage aura that intensifies and glows brighter, scarred and battle-worn chassis conveying feral intensity,
primary color #B8232F (blood red) with dark accents #4A0D12,
matching the original tower concept: berserker tower that grows fiercer and stronger with every accumulated kill,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (rage aura glow, ember particles),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 관통포 (piercer)

파일명:
piercer.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a reinforced armor-piercing cannon turret with a long tapered drill-tipped barrel built to punch through heavy plating, golden metallic trim and reinforced recoil dampeners, a sharpened penetrator spike visible at the muzzle,
primary color #C9A227 (gold) with dark accents #6E5610,
matching the original tower concept: armor-piercing cannon devastatingly effective against heavily armored enemies,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (metallic shine, piercing spark on the tip),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 관통저격수 (pierceSniper)

파일명:
pierceSniper.png

이미지 프롬프트:
Top-down tower defense game turret asset,
an elite long-range piercing sniper turret with an extra-long tapered precision barrel even longer than the standard sniper, an advanced multi-lens scope array glowing sky blue, stabilizing bipod and recoil compensator, futuristic marksman design built to punch through multiple targets,
primary color #4FA8D8 (sky blue) with dark accents #215A78,
matching the original tower concept: advanced piercing sniper that shoots through and hits multiple enemies in a line,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (scope lens glow, piercing energy trail),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 번개 (lightning)

파일명:
lightning.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a tesla-coil style turret with a coiled copper electric barrel wound in spiraling rings, crackling yellow electric sparks arcing between exposed conductor nodes, a glowing tesla core radiating static energy,
primary color #F0B90B (electric yellow) with dark accents #8C6E05,
matching the original tower concept: chain-lightning tower that jumps and arcs between multiple targets,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (crackling electric spark arcs, static glow aura),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 지휘관 (commander)

파일명:
commander.png

이미지 프롬프트:
Top-down tower defense game support turret asset,
a non-attacking command tower with a rotating radar dish and banner totem instead of a weapon barrel, an emanating supportive green pulse-ring aura that boosts nearby units, authoritative command-post design with antenna and insignia details,
primary color #3D9970 (green) with dark accents #1F4D3A,
matching the original tower concept: support tower with no direct attack, boosts nearby towers' attack speed,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (pulsing support aura rings),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 독 (poison)

파일명:
poison.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a toxic turret built around a bulbous glass/metal poison tank sloshing with glowing green venom, a thick nozzle-barrel dripping viscous toxic ooze, corroded valves leaking wisps of noxious toxic vapor into the air,
primary color #5FA83D (toxic green) with dark accents #34611F,
matching the original tower concept: poison tower that applies a lingering damage-over-time toxin,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (toxic vapor wisps, dripping venom glow),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 레이저 (laser)

파일명:
laser.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a futuristic energy turret with a faceted crystalline red focusing lens at the barrel tip, an internal glowing energy core visible through vents, a sleek sci-fi emitter housing radiating continuous piercing laser light,
primary color #E24B4A (red) with dark accents #8C1F1F,
matching the original tower concept: laser tower that fires a continuous piercing beam through every enemy in a straight line,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (glowing lens flare, energy core pulse),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 플라즈마 (plasma)

파일명:
plasma.png

이미지 프롬프트:
Top-down tower defense game turret asset,
a heavy sci-fi plasma cannon turret built around a glowing magenta-pink plasma energy core suspended in a containment ring, a thick reinforced barrel channeling superheated plasma, energy conduits pulsing along the chassis,
primary color #D1479B (magenta) with dark accents #832C61,
matching the original tower concept: high-damage splash-damage plasma cannon,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (glowing plasma core, energy containment ring flicker),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 블랙홀 (blackhole)

파일명:
blackhole.png

이미지 프롬프트:
Top-down tower defense game turret asset,
an exotic gravity-well tower with no visible barrel, instead a swirling dark purple singularity ring hovering and slowly rotating above an ornate anti-gravity base, faint distortion warping the space around it, arcane energy conduits feeding the singularity,
primary color #4A2E7A (deep purple) with dark accents #1C1230,
matching the original tower concept: rare gravity tower that pulls in enemies (max 2 buildable per game),
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (gravitational distortion warp, swirling singularity glow),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

## 초신성 (nova)

파일명:
nova.png

이미지 프롬프트:
Top-down tower defense game turret asset,
an endgame superweapon turret with a massive heavily-plated cannon barrel, a radiant crimson supernova core blazing at its center, cracked energy vents releasing intense heat, imposing scale conveying ultimate late-game power,
primary color #FF3864 (crimson) with dark accents #7A0F27,
matching the original tower concept: ultimate endgame tower with the largest splash damage, unlocked very late game,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (radiant supernova glow, heat shimmer),
transparent background,
PNG asset,
vibrant colors,
professional game art

권장 크기:
512x512

---

# 적

## 일반 (normal)

파일명:
normal.png

이미지 프롬프트:
Top-down enemy game asset,
a small round basic blob-like creature with no special features, simple and cute but menacing, plain and unassuming compared to specialized enemies,
primary color #F0997B (salmon) with dark accents #712B13,
matching the original enemy concept: standard basic monster with no abilities,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (soft body sheen),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 중장갑 (armored)

파일명:
armored.png

이미지 프롬프트:
Top-down enemy game asset,
a heavily armored beetle-like creature with thick riveted metallic plating on its back, slow and tanky, reinforced carapace with visible seams and battle scratches,
primary color #8A8F98 (steel gray) with dark accents #4A4F57,
matching the original enemy concept: high-HP armored beetle, slow-moving, resistant to most towers except armor-piercing ones,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (metallic sheen, plating glint),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 돌진 (rush)

파일명:
rush.png

이미지 프롬프트:
Top-down enemy game asset,
a sleek aerodynamic triangular creature leaning forward as if sprinting at high speed, dynamic motion streaks trailing behind it, wind-swept angular form,
primary color #FF6B4A (orange-red) with dark accents #B23A22,
matching the original enemy concept: fast low-HP creature that rushes forward at high speed,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (speed motion trail glow),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 비행 (flying)

파일명:
flying.png

이미지 프롬프트:
Top-down enemy game asset,
a small bat-like flying creature with translucent membranous wings spread wide, hovering with a subtle motion blur on the wingtips,
primary color #5AC8FA (sky blue) with dark accents #1D6FA5,
matching the original enemy concept: flying monster that only certain anti-air towers can target,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (translucent wing glow, soft hover shimmer),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 재생 (regen)

파일명:
regen.png

이미지 프롬프트:
Top-down enemy game asset,
a round organic blob creature with a pulsing healing green glow emanating from within, regenerative organic texture with soft veins of light,
primary color #7ED957 (bright green) with dark accents #3E7A28,
matching the original enemy concept: monster that continuously regenerates health over time,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (pulsing healing glow, regenerative particle sparkle),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 도둑 (thief)

파일명:
thief.png

이미지 프롬프트:
Top-down enemy game asset,
a sneaky diamond-shaped creature clutching a bulging gold coin sack, mischievous glinting eyes, agile and cunning silhouette,
primary color #FFD23F (gold-yellow) with dark accents #8C6E05,
matching the original enemy concept: thief monster that steals gold when it reaches the base,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (gold coin glint sparkle),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 분열 (split)

파일명:
split.png

이미지 프롬프트:
Top-down enemy game asset,
a peanut-shaped creature with a visible glowing dividing seam down the middle, straining as if about to split into two,
primary color #C77DD9 (light purple/pink) with dark accents #7A3E8C,
matching the original enemy concept: monster that splits into two weaker children on death,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (glowing seam crack, energy leak effect),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 철갑 (ironclad)

파일명:
ironclad.png

이미지 프롬프트:
Top-down enemy game asset,
a hexagonal fortress-like creature encased in extremely thick riveted iron plating, near-impenetrable armored hull with reinforced bolts,
primary color #B8C4D9 (pale steel) with dark accents #4A5568,
matching the original enemy concept: extremely armored monster immune to slow effects, resistant to most towers,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (metallic armor shine, rivet highlight),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 거인 (titan)

파일명:
titan.png

이미지 프롬프트:
Top-down enemy game asset,
a massive rocky boulder-like giant creature, slow and towering, deeply cracked stone texture with glowing molten fissures,
primary color #6B4226 (brown) with dark accents #2E1B0F,
matching the original enemy concept: giant slow-moving monster that costs 2 lives if it reaches the base,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (glowing cracked fissures, dust particle trail),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 복제자 (cloner)

파일명:
cloner.png

이미지 프롬프트:
Top-down enemy game asset,
a peanut-shaped creature glowing with unstable pink energy, crackling with volatile splitting energy, more intense and dangerous version of a splitting monster,
primary color #FF6FB5 (pink) with dark accents #8C2E5E,
matching the original enemy concept: monster that splits into three children on death (stronger version of split),
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (unstable energy crackle, glowing split fractures),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 은신 (phantom)

파일명:
phantom.png

이미지 프롬프트:
Top-down enemy game asset,
a translucent ghostly hooded specter with glowing purple eyes, semi-transparent wispy trailing edges fading into mist,
primary color #B39DDB (light purple) with dark accents #4A3B6B,
matching the original enemy concept: ghost monster that periodically turns invisible and untargetable,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (ghostly glow, translucent fade effect),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 흡혈 (vampire)

파일명:
vampire.png

이미지 프롬프트:
Top-down enemy game asset,
a dark cloaked creature with a sharp triangular hood and glowing red eyes, a draining crimson life-energy aura swirling around it,
primary color #8B0000 (dark red) with dark accents #3A0000,
matching the original enemy concept: vampire monster that heals when nearby monsters die,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (draining life-energy aura glow),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

## 보급상자 (crate)

파일명:
crate.png

이미지 프롬프트:
Top-down enemy game asset,
a sturdy wooden supply crate with metal reinforcement bands and rivets, a pulsing golden glowing outline signaling a bonus reward,
primary color #D4A017 (gold) with dark accents #7A5A0A,
matching the original enemy concept: rare bonus supply crate that drops a large gold reward when destroyed,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game character art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (golden pulse glow, sparkle particles),
transparent background,
mobile game style,
high quality

권장 크기:
512x512

---

# 보스

## 기갑형 보스 (juggernaut)

파일명:
juggernaut.png

이미지 프롬프트:
Top-down boss enemy game asset,
a massive heavily-armored juggernaut boss creature, a menacing star-shaped crown of spikes on its back, thick battle-worn plating, imposing and unstoppable presence,
primary color #E24B4A (red) with dark accents #791F1F,
matching the original boss concept: armored boss that uses EMP (stuns nearby towers), rush (speed burst charge), and shield defensive skills,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (EMP energy crackle, charging rush glow),
transparent background,
mobile game style,
high quality,
epic boss presence

권장 크기:
768x768

## 소환형 보스 (summoner)

파일명:
summoner.png

이미지 프롬프트:
Top-down boss enemy game asset,
a mystical summoner boss creature with a crown of spikes, swirling purple summoning energy circling around it, arcane runes glowing faintly on its form,
primary color #9B59B6 (purple) with dark accents #4A235A,
matching the original boss concept: summoner boss that conjures additional minion enemies during battle,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (swirling summoning vortex, arcane rune glow),
transparent background,
mobile game style,
high quality,
epic boss presence

권장 크기:
768x768

## 지휘관형 보스 (warlord)

파일명:
warlord.png

이미지 프롬프트:
Top-down boss enemy game asset,
a commanding warlord boss creature with a crown of spikes, a radiant golden protective aura shield radiating outward to allies, regal battle armor conveying leadership,
primary color #E8940C (orange-gold) with dark accents #7A4B05,
matching the original boss concept: warlord boss that grants protective shields to nearby allied monsters,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
detailed mechanical parts,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (golden shield aura radiance),
transparent background,
mobile game style,
high quality,
epic boss presence

권장 크기:
768x768

## 미니보스 (miniboss)

파일명:
miniboss.png

이미지 프롬프트:
Top-down mini-boss enemy game asset,
a smaller but still imposing star-crowned creature, reinforced armor plating, tougher than a regular monster but less epic in scale than a full boss,
primary color #FF9F1C (orange) with dark accents #7A4B0A,
matching the original mini-boss concept: reinforced enemy appearing every 5 waves, weaker than a full boss,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (subtle power aura glow),
transparent background,
mobile game style,
high quality

권장 크기:
640x640

---

# 투사체

## 일반 발사체 (bullet)

파일명:
bullet.png

이미지 프롬프트:
Top-down tower defense projectile asset,
a small glowing energy bullet/orb with a soft radiant outer glow trail and a bright hot core,
neutral bright color with a bright white-yellow core (color is tinted per tower in-game),
matching the original concept: generic projectile fired by most standard towers (basic, gatling, missile, explosive, frost, berserker, piercer, poison, plasma, nova),
highly polished mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (motion glow trail, energy core pulse),
transparent background,
mobile game style,
high quality,
small compact asset

권장 크기:
128x128

## 저격 빔 (sniper beam)

파일명:
sniperBeam.png

이미지 프롬프트:
Top-down tower defense projectile asset,
a thin, razor-sharp instant-hit precision energy beam streak with a bright glowing core and purple tint, crisp edges conveying pinpoint accuracy,
matching the original concept: instant hitscan line from the sniper tower to its target,
highly polished mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (energy core glow, trailing light particles),
transparent background,
mobile game style,
high quality,
horizontal beam texture, tileable/stretchable along its length

권장 크기:
256x64

## 관통저격 빔 (pierce sniper beam)

파일명:
pierceSniperBeam.png

이미지 프롬프트:
Top-down tower defense projectile asset,
a thicker piercing energy beam streak in vivid sky blue that appears to punch through and continue past multiple targets, energy fracture lines along its length,
matching the original concept: piercing hitscan beam from the pierce sniper tower that hits up to 2 enemies in a line,
highly polished mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (piercing energy fracture glow),
transparent background,
mobile game style,
high quality,
horizontal beam texture, tileable/stretchable along its length

권장 크기:
256x64

## 레이저 빔 (laser beam)

파일명:
laserBeam.png

이미지 프롬프트:
Top-down tower defense projectile asset,
a wide continuous searing red energy laser beam with an intense glowing core and radiant outer bloom,
matching the original concept: continuous piercing beam from the laser tower that hits every enemy along a straight line,
highly polished mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (intense beam bloom, heat shimmer),
transparent background,
mobile game style,
high quality,
horizontal beam texture, tileable/stretchable along its length

권장 크기:
256x64

## 번개 체인 (lightning chain)

파일명:
lightningChain.png

이미지 프롬프트:
Top-down tower defense projectile asset,
a jagged crackling electric-yellow lightning bolt arc connecting two points, branching micro-sparks along its jagged path,
matching the original concept: chain lightning segment jumping between up to 5 targets,
highly polished mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (crackling spark branches, electric glow),
transparent background,
mobile game style,
high quality,
horizontal zigzag beam texture, tileable/stretchable along its length

권장 크기:
256x64

## 블랙홀 흡입장 (blackhole field, 참고용 - 투사체 아님)

파일명:
blackholeField.png

이미지 프롬프트:
Top-down tower defense effect asset,
a swirling dark purple gravitational vortex ring with visible space distortion warping and light being pulled inward,
matching the original concept: continuous pull+damage aura field around the blackhole tower (not a discrete projectile, rendered as a persistent circular field),
highly polished mobile game art,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
visual effects integrated (gravitational light-bending distortion),
transparent background,
mobile game style,
high quality

권장 크기:
384x384

---

# 필드 (타일)

각 테마마다 board(밝은 타일) / boardAlt(어두운 타일, 체크무늬용) / path(경로 타일) 3종이 필요합니다. 타일은 이음매 없이 반복(seamless tile) 가능해야 합니다.

## Green Meadow - 기본 타일

파일명:
greenMeadow_board.png

이미지 프롬프트:
Seamless top-down grass tile texture for a tower defense game,
lush green meadow ground with subtle grass blade details and natural material variation,
base color #1e3a24 (dark mode) / #eaf7e2 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Green Meadow - 보조 타일

파일명:
greenMeadow_boardAlt.png

이미지 프롬프트:
Seamless top-down grass tile texture for a tower defense game,
slightly darker shade of meadow grass to create a checkerboard variation, matching material detail,
base color #254a2c (dark mode) / #d7ecc9 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Green Meadow - 경로 타일

파일명:
greenMeadow_path.png

이미지 프롬프트:
Seamless top-down dirt path tile texture for a tower defense game,
worn brown dirt trail that monsters walk along, small pebbles and footprints, well-trodden ground detail,
base color #6b4a2c (dark mode) / #c99a5b (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Abyss Ocean - 기본 타일

파일명:
abyssOcean_board.png

이미지 프롬프트:
Seamless top-down deep ocean floor tile texture for a tower defense game,
dark blue abyssal seabed with subtle wave ripple patterns and faint caustic light dapples,
base color #0b2f45 (dark mode) / #dff3f7 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Abyss Ocean - 보조 타일

파일명:
abyssOcean_boardAlt.png

이미지 프롬프트:
Seamless top-down deep ocean floor tile texture for a tower defense game,
slightly lighter teal-blue seabed shade to create a checkerboard variation, matching material detail,
base color #0e3a54 (dark mode) / #c9e9f0 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Abyss Ocean - 경로 타일

파일명:
abyssOcean_path.png

이미지 프롬프트:
Seamless top-down glowing current/trench path tile texture for a tower defense game,
a bright teal bioluminescent ocean current trail that monsters swim along, glowing energy streaks,
base color #0a6e6a (dark mode) / #4fd1c5 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Fantasy Kingdom - 기본 타일

파일명:
fantasyKingdom_board.png

이미지 프롬프트:
Seamless top-down enchanted castle courtyard tile texture for a tower defense game,
purple magical stone floor with faint glowing arcane engravings,
base color #2b1f45 (dark mode) / #f3ecff (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Fantasy Kingdom - 보조 타일

파일명:
fantasyKingdom_boardAlt.png

이미지 프롬프트:
Seamless top-down enchanted castle courtyard tile texture for a tower defense game,
slightly darker purple magical stone shade to create a checkerboard variation, matching material detail,
base color #38295a (dark mode) / #e6d9ff (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Fantasy Kingdom - 경로 타일

파일명:
fantasyKingdom_path.png

이미지 프롬프트:
Seamless top-down golden cobblestone road tile texture for a tower defense game,
a royal golden brick road that monsters march along, ornate fantasy kingdom engravings,
base color #caa23a (dark mode) / #e0b84a (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Infernal Rift - 기본 타일

파일명:
infernalRift_board.png

이미지 프롬프트:
Seamless top-down scorched hellish ground tile texture for a tower defense game,
dark cracked volcanic rock with glowing ember light seeping through the cracks,
base color #2a1210 (dark mode) / #fbe2d8 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Infernal Rift - 보조 타일

파일명:
infernalRift_boardAlt.png

이미지 프롬프트:
Seamless top-down scorched hellish ground tile texture for a tower defense game,
slightly different shade of cracked volcanic rock to create a checkerboard variation, matching material detail,
base color #3a1613 (dark mode) / #f5c9b8 (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

## Infernal Rift - 경로 타일

파일명:
infernalRift_path.png

이미지 프롬프트:
Seamless top-down molten lava rift path tile texture for a tower defense game,
a glowing orange-red lava crack that monsters crawl along, radiant heat glow,
base color #b8451f (dark mode) / #e0653a (light mode),
highly polished mobile game environment art,
premium game asset,
stylized AAA mobile game tile art,
vivid lighting,
strong material detail,
tileable, flat lighting, no shadows,
PNG asset

권장 크기:
128x128

---

# UI 아이콘

모든 UI 아이콘은 단순하고 읽기 쉬운 실루엣을 유지하되, 클래시 로얄/브롤스타즈 수준의 정제된 마무리(미세한 베벨, 하이라이트, 그림자)를 적용한 프리미엄 아이콘으로 제작합니다.

## 배속 전환 (speed)

파일명:
speed.svg

이미지 프롬프트:
Polished flat game UI icon,
two overlapping play/fast-forward triangles indicating speed toggle,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 일시정지 (pause)

파일명:
pause.svg

이미지 프롬프트:
Polished flat game UI icon,
two vertical bars representing a pause button,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 재생 (play)

파일명:
play.svg

이미지 프롬프트:
Polished flat game UI icon,
a single right-pointing triangle play button,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 타워 합성 (fusion)

파일명:
fusion.svg

이미지 프롬프트:
Polished flat game UI icon,
two overlapping circles representing merging/fusion,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 연구소 (lab)

파일명:
lab.svg

이미지 프롬프트:
Polished flat game UI icon,
a science flask/beaker shape representing a research lab, with a glowing liquid inside,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 소리 켜짐 (soundOn)

파일명:
soundOn.svg

이미지 프롬프트:
Polished flat game UI icon,
a speaker icon with sound waves indicating sound is on,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 소리 꺼짐 (soundOff)

파일명:
soundOff.svg

이미지 프롬프트:
Polished flat game UI icon,
a speaker icon with an X or crossed line indicating sound is muted,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 음악 켜짐 (musicOn)

파일명:
musicOn.svg

이미지 프롬프트:
Polished flat game UI icon,
a musical note icon indicating background music is on,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 음악 꺼짐 (musicOff)

파일명:
musicOff.svg

이미지 프롬프트:
Polished flat game UI icon,
a musical note icon with a crossed line indicating music is muted,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 라이트 모드 (sun)

파일명:
sun.svg

이미지 프롬프트:
Polished flat game UI icon,
a sun icon with radiating rays representing light mode,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 다크 모드 (moon)

파일명:
moon.svg

이미지 프롬프트:
Polished flat game UI icon,
a crescent moon icon representing dark mode,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 업그레이드 (upgrade)

파일명:
upgrade.svg

이미지 프롬프트:
Polished flat game UI icon,
an upward arrow merging into a shield or block shape representing upgrade,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 골드 (coin)

파일명:
coin.svg

이미지 프롬프트:
Polished flat game UI icon,
a round gold coin icon with a glossy metallic shine,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 닫기 (close)

파일명:
close.svg

이미지 프롬프트:
Polished flat game UI icon,
an X close/cancel icon,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 공격력 (sword)

파일명:
sword.svg

이미지 프롬프트:
Polished flat game UI icon,
a small sword icon representing attack power, with a glinting blade edge,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 사거리 (target)

파일명:
target.svg

이미지 프롬프트:
Polished flat game UI icon,
a target/crosshair icon representing range,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 타워 표시 (turret)

파일명:
turret.svg

이미지 프롬프트:
Polished flat game UI icon,
a small top-down turret silhouette icon,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 자동선택 (auto)

파일명:
auto.svg

이미지 프롬프트:
Polished flat game UI icon,
a circular refresh/auto-cycle arrows icon,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 처치수 (kills)

파일명:
kills.svg

이미지 프롬프트:
Polished flat game UI icon,
a small trophy or skull-crossbones icon representing kill count,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 패시브 (passive)

파일명:
passive.svg

이미지 프롬프트:
Polished flat game UI icon,
a star/sparkle icon representing passive bonuses, with a soft glow,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 트로피 (trophy)

파일명:
trophy.svg

이미지 프롬프트:
Polished flat game UI icon,
a trophy cup icon representing rankings, with a glossy golden shine,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 확대 (zoom)

파일명:
zoom.svg

이미지 프롬프트:
Polished flat game UI icon,
a magnifying glass icon representing zoom,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 나가기 (exit)

파일명:
exit.svg

이미지 프롬프트:
Polished flat game UI icon,
a door with an exit arrow icon,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 오토플레이 (bot)

파일명:
bot.svg

이미지 프롬프트:
Polished flat game UI icon,
a small robot face icon representing autoplay, with glowing eye lights,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 딜 미터기 (dps)

파일명:
dps.svg

이미지 프롬프트:
Polished flat game UI icon,
a small bar chart icon with ascending bars representing a DPS meter,
clean minimal readable silhouette with a subtle bevel and highlight,
highly polished mobile game UI art,
Brawl Stars quality UI polish,
premium mobile game UI asset,
vivid accent lighting,
transparent background,
monochrome or two-tone,
mobile game UI quality

권장 크기:
128x128

## 타이틀 로고 (title)

파일명:
title.svg

이미지 프롬프트:
Premium game logo icon for a tower defense mobile game,
a stylized tower/turret silhouette with a target ring, vivid gold-to-red gradient (#F0B90B to #E24B4A) with strong highlight sheen,
clean, iconic, memorable mark suitable as an app icon or title screen emblem,
highly polished mobile game art,
Clash Royale quality,
Brawl Stars quality,
stylized AAA mobile game branding,
premium game asset,
vivid lighting,
strong highlights,
readable silhouette,
transparent background,
professional game branding quality

권장 크기:
256x256
