# 에셋 누락 리포트

`assets/ui/` 폴더에는 UI 아이콘 26종이 SVG로 이미 생성되어 있습니다. 나머지 카테고리(타워/적/보스/투사체/타일)는 아직 비어 있어 게임은 `AssetManager`의 폴백 로직에 따라 기존 절차적(Canvas 도형) 렌더링으로 정상 동작합니다.

`AI_ASSET_PROMPTS.md`의 프롬프트로 이미지를 생성한 뒤, 아래 표의 "파일 경로"에 그대로 저장하면 **코드 수정 없이** 자동 적용됩니다. `AssetManager`는 PNG를 먼저 찾고, 없으면 같은 이름의 SVG를 자동으로 대신 사용합니다.

> **파일명 수정 안내**: 이 리포트의 파일 경로는 원래부터 실제 코드와 일치했지만(`AI_ASSET_PROMPTS.md`는 반대로 `tower_`, `ui_` 같은 접두어가 붙은 잘못된 파일명을 안내하고 있었습니다), 혹시 잘못된 이름으로 이미지를 만들어둔 것이 있다면 아래 경로(접두어 없음)로 다시 이름을 맞춰주세요.

---

## 없는 타워 이미지 (16개, `assets/towers/`)

| 타워 | 파일 경로 | 상태 |
|---|---|---|
| 기본 | assets/towers/basic.png | 없음 (도형 렌더링 유지) |
| 저격 | assets/towers/sniper.png | 없음 (도형 렌더링 유지) |
| 기관총 | assets/towers/gatling.png | 없음 (도형 렌더링 유지) |
| 미사일터렛 | assets/towers/missile.png | 없음 (도형 렌더링 유지) |
| 폭발 | assets/towers/explosive.png | 없음 (도형 렌더링 유지) |
| 냉기 | assets/towers/frost.png | 없음 (도형 렌더링 유지) |
| 광전사 | assets/towers/berserker.png | 없음 (도형 렌더링 유지) |
| 관통포 | assets/towers/piercer.png | 없음 (도형 렌더링 유지) |
| 관통저격수 | assets/towers/pierceSniper.png | 없음 (도형 렌더링 유지) |
| 번개 | assets/towers/lightning.png | 없음 (도형 렌더링 유지) |
| 지휘관 | assets/towers/commander.png | 없음 (도형 렌더링 유지) |
| 독 | assets/towers/poison.png | 없음 (도형 렌더링 유지) |
| 레이저 | assets/towers/laser.png | 없음 (도형 렌더링 유지) |
| 플라즈마 | assets/towers/plasma.png | 없음 (도형 렌더링 유지) |
| 블랙홀 | assets/towers/blackhole.png | 없음 (도형 렌더링 유지) |
| 초신성 | assets/towers/nova.png | 없음 (도형 렌더링 유지) |

## 없는 적 이미지 (13개, `assets/enemies/`)

| 적 | 파일 경로 | 상태 |
|---|---|---|
| 일반 | assets/enemies/normal.png | 없음 (도형 렌더링 유지) |
| 중장갑 | assets/enemies/armored.png | 없음 (도형 렌더링 유지) |
| 돌진 | assets/enemies/rush.png | 없음 (도형 렌더링 유지) |
| 비행 | assets/enemies/flying.png | 없음 (도형 렌더링 유지) |
| 재생 | assets/enemies/regen.png | 없음 (도형 렌더링 유지) |
| 도둑 | assets/enemies/thief.png | 없음 (도형 렌더링 유지) |
| 분열 | assets/enemies/split.png | 없음 (도형 렌더링 유지) |
| 철갑 | assets/enemies/ironclad.png | 없음 (도형 렌더링 유지) |
| 거인 | assets/enemies/titan.png | 없음 (도형 렌더링 유지) |
| 복제자 | assets/enemies/cloner.png | 없음 (도형 렌더링 유지) |
| 은신 | assets/enemies/phantom.png | 없음 (도형 렌더링 유지) |
| 흡혈 | assets/enemies/vampire.png | 없음 (도형 렌더링 유지) |
| 보급상자 | assets/enemies/crate.png | 없음 (도형 렌더링 유지) |

## 없는 보스 이미지 (4개, `assets/bosses/`)

| 보스 | 파일 경로 | 상태 |
|---|---|---|
| 기갑형 (juggernaut) | assets/bosses/juggernaut.png | 없음 (도형 렌더링 유지) |
| 소환형 (summoner) | assets/bosses/summoner.png | 없음 (도형 렌더링 유지) |
| 지휘관형 (warlord) | assets/bosses/warlord.png | 없음 (도형 렌더링 유지) |
| 미니보스 | assets/bosses/miniboss.png | 없음 (도형 렌더링 유지) |

## 없는 투사체 이미지 (6개, `assets/projectiles/`)

| 투사체 | 파일 경로 | 상태 |
|---|---|---|
| 일반 발사체 | assets/projectiles/bullet.png | 없음 (원형 도형 렌더링 유지) — **코드에 실제 연동됨** |
| 저격 빔 | assets/projectiles/sniperBeam.png | 없음 — 카탈로그에는 포함되어 있으나 **현재 렌더링 코드는 연동되지 않음** (하단 참고) |
| 관통저격 빔 | assets/projectiles/pierceSniperBeam.png | 없음 — 위와 동일 |
| 레이저 빔 | assets/projectiles/laserBeam.png | 없음 — 위와 동일 |
| 번개 체인 | assets/projectiles/lightningChain.png | 없음 — 위와 동일 |
| 블랙홀 흡입장 | assets/projectiles/blackholeField.png | 없음 — 위와 동일 |

> 참고: `bullet`(일반 발사체)만 실제로 `AssetManager`와 연동되어 이미지가 생기면 즉시 적용됩니다. 나머지 4종(저격/관통저격/레이저/번개)은 매 프레임 위치·각도·길이가 달라지는 즉발 라인/빔 이펙트(`G.lasers`)라서, 고정 프레임 이미지보다 회전/신축 텍스처 매핑이 필요해 이번 1차 작업 범위에서는 절차적 렌더링(발광 라인)을 그대로 유지했습니다. 추후 확장 시 `ctx.save()+ctx.translate()+ctx.rotate()+ctx.drawImage()`로 빔 길이만큼 늘려 그리는 방식으로 추가 가능합니다.

## 없는 타일(필드) 이미지 (12개, `assets/tiles/`)

| 테마 | 기본 타일 | 보조 타일(체크무늬) | 경로 타일 |
|---|---|---|---|
| Green Meadow | assets/tiles/greenMeadow_board.png | assets/tiles/greenMeadow_boardAlt.png | assets/tiles/greenMeadow_path.png |
| Abyss Ocean | assets/tiles/abyssOcean_board.png | assets/tiles/abyssOcean_boardAlt.png | assets/tiles/abyssOcean_path.png |
| Fantasy Kingdom | assets/tiles/fantasyKingdom_board.png | assets/tiles/fantasyKingdom_boardAlt.png | assets/tiles/fantasyKingdom_path.png |
| Infernal Rift | assets/tiles/infernalRift_board.png | assets/tiles/infernalRift_boardAlt.png | assets/tiles/infernalRift_path.png |

모두 없음 — 절차적 단색 타일 + 장식(grass/wave/sparkle/crack) 렌더링 유지.

## UI 이미지 (26개, `assets/ui/`) — **전부 SVG로 존재함**

Brawl Stars 스타일(둥근 배지 + 굵은 실루엣 + 글로시 하이라이트)의 SVG 26종이 이미 생성되어 있습니다.

| 아이콘 | 파일 경로 | 상태 |
|---|---|---|
| 배속 전환 | assets/ui/speed.svg | 존재 — DOM 자동 교체 연동됨 |
| 타워 합성 | assets/ui/fusion.svg | 존재 — DOM 자동 교체 연동됨 |
| 업그레이드 | assets/ui/upgrade.svg | 존재 — DOM 자동 교체 연동됨 |
| 연구소 | assets/ui/lab.svg | 존재 — DOM 자동 교체 연동됨 |
| 자동선택 | assets/ui/auto.svg | 존재 — DOM 자동 교체 연동됨 |
| 처치수 | assets/ui/kills.svg | 존재 — DOM 자동 교체 연동됨 |
| 패시브 | assets/ui/passive.svg | 존재 — DOM 자동 교체 연동됨 |
| 트로피 | assets/ui/trophy.svg | 존재 — DOM 자동 교체 연동됨 |
| 확대 | assets/ui/zoom.svg | 존재 — DOM 자동 교체 연동됨 |
| 나가기 | assets/ui/exit.svg | 존재 — DOM 자동 교체 연동됨 |
| 오토플레이 | assets/ui/bot.svg | 존재 — DOM 자동 교체 연동됨 |
| 딜 미터기 | assets/ui/dps.svg | 존재 — DOM 자동 교체 연동됨 |
| 타이틀 로고 | assets/ui/title.svg | 존재 — DOM 자동 교체 연동됨 |
| 일시정지/재생 | assets/ui/pause.svg, assets/ui/play.svg | 존재 — 단, **자동 이미지 교체는 미연동** (하단 참고) |
| 음악 켜짐/꺼짐 | assets/ui/musicOn.svg, assets/ui/musicOff.svg | 존재 — 위와 동일 |
| 효과음 켜짐/꺼짐 | assets/ui/soundOn.svg, assets/ui/soundOff.svg | 존재 — 위와 동일 |
| 라이트/다크 모드 | assets/ui/sun.svg, assets/ui/moon.svg | 존재 — 위와 동일 |
| 코인/닫기/공격력/사거리/타워 표시 | assets/ui/coin.svg, close.svg, sword.svg, target.svg, turret.svg | 존재 — 현재 UI에서 버튼으로 직접 쓰이지 않아 미연동 |

> 참고: 일시정지/재생, 음악, 효과음, 라이트/다크 모드 아이콘은 게임 상태(재생 중/일시정지, 음소거 여부, 테마)에 따라 **두 가지 SVG를 실시간으로 전환**하는 별도 로직이 있어, 이번 1차 작업에서는 상태 전환 로직과의 충돌을 피하기 위해 이미지 자동 교체 대상에서 제외했습니다(파일 자체는 존재하며 향후 연동 가능). 나머지 정적 아이콘(합성/업그레이드/연구소/자동선택 등 13개)은 `initIcons()`에서 `AssetManager.onReady()`로 이미지 유무를 비동기 확인해 있으면 즉시 `<img>`로 교체합니다. `AssetManager`는 PNG를 먼저 찾고 없으면 SVG를 자동으로 대신 로드하므로, 나중에 PNG를 추가하면 자동으로 PNG가 우선 적용됩니다.

---

## 요약

- 총 카탈로그 등록 에셋: 16(타워) + 13(적) + 4(보스) + 6(투사체) + 12(타일) + 26(UI) = **77개**
- 현재 존재: **26개** (UI 아이콘 전부, SVG) / 51개 누락 (타워·적·보스·투사체·타일)
- 실제 렌더링 코드와 완전히 연동되어 파일만 넣으면 바로 적용되는 카테고리: 타워, 적, 보스, 타일, 발사체(bullet), 정적 UI 아이콘 13종(이미 SVG로 적용 중)
- 파일은 존재하지만 DOM 교체 로직이 아직 없는 카테고리: 상태 전환형 UI 아이콘 4쌍(8개), 미사용 UI 글리프 5개
- 절차적 렌더링만 유지되는 카테고리(향후 확장 여지): 빔형 투사체 4종
