<p align="center">
  <picture>
    <source media="(max-width: 640px)" srcset="./assets/readme/domado-readme-intro-mobile.svg" />
    <img src="./assets/readme/domado-readme-intro.svg" alt="DOMADO WORLD. 포트폴리오 건물·길드·대장간, 시장·우편함·분수, 연못·풍차·텃밭을 담은 마을의 각도별 픽셀 일러스트가 쉬지 않고 계속 회전합니다. 정면에서 폭포 왼쪽에는 목장, 오른쪽에는 던전이 보입니다. 모션 감소 설정에서는 정면 그림을 유지합니다." width="100%" />
  </picture>
</p>

<h1 align="center">DOMADO WORLD</h1>

<p align="center">
  <strong>소개·프로젝트·기술을 직접 탐색하는<br>픽셀 마을 포트폴리오</strong><br>
  박건호 · 백엔드 중심 풀스택 개발자<br>
  <sub>1인 기획 · 월드 설계 · 개발 · 최적화</sub>
</p>

<p align="center">
  <a href="https://domado.me"><strong>DOMADO 플레이</strong></a>
  ·
  <a href="#프로젝트-한눈에-보기"><strong>프로젝트 개요</strong></a>
  ·
  <a href="./docs/engineering-cases.md"><strong>엔지니어링 사례</strong></a>
  ·
  <a href="./docs/development-history.md"><strong>전체 개발 과정</strong></a>
  ·
  <a href="https://github.com/DO-MADO"><strong>GitHub 프로필</strong></a>
</p>

<br>

<p align="center">
DOMADO는 픽셀 마을을 탐험하며 소개·프로젝트·기술을 찾아보는 웹 포트폴리오입니다.<br>
게임을 하지 않고 포트폴리오나 모바일 카드로 바로 들어갈 수도 있습니다.<br>
기획부터 개발·배포까지 직접 맡아, 마을의 동선과 상호작용을 설계하고 화면과 게임 시스템을 구현했습니다.<br>
</p>

<br>
<br>

## 프로젝트 한눈에 보기

| 질문 | 답 |
| --- | --- |
| 무엇을 만들었나 | React·TypeScript·Canvas 2D로 만든 `672×448` 탐험형 포트폴리오 |
| 개발 기간 | 2025.11~2026.10 · 1인 기획·설계·개발·배포 |
| 핵심 기술 | React 19, TypeScript, Vite, Canvas 2D, Web Audio, Vercel Serverless |
| 담당 범위 | 제품 콘셉트, 정보 구조, 월드·상호작용, React UI, 모바일 분기, 서버리스 연동, 성능 계측 |

<br>
<br>

### DOMADO 월드의 세 가지 특징

- **마을이 곧 탐색 메뉴 :**
  - 길드·텃밭·풍차·보관소를 소개·기술·프로젝트·기록과 연결했습니다.<br>
  - 방문자는 걷고 대화하며 보고 싶은 정보를 고릅니다.<br>

- **직접 연결한 월드 시스템 :**
  - 별도 게임 엔진 없이 React·Canvas 2D로 이동·충돌·퀘스트·전투를 구현하고 낮·밤, 작물 성장, 사운드를 연결했습니다.<br>

- **탐험하지 않아도 열람할 수 있습니다.**<br>
  - 데스크톱·모바일 가로에서는 마을을 탐험합니다.<br>
  - 게임 없이 세로 스크롤 포트폴리오를 열거나 모바일 세로의 퀵메뉴 카드로 원하는 정보를 볼 수도 있습니다.<br>

<hr>

<br>
<br>

## 왜 포트폴리오를 게임으로 만들었나

프로젝트와 기술을 정리하는 것만으로는 제가 어떤 사람인지 충분히 표현하기 어렵다고 느꼈습니다.<br>
제가 좋아하는 레트로 게임을 바탕으로 제 취향과 감성을 담은 공간을 만들고 싶었고, 방문자가 모험하고 상호작용하며 저를 알아가는 과정 자체를 즐겼으면 했습니다.<br>
<br>
첫 구현은 부팅 화면과 드래그 창을 갖춘 레트로 OS였지만 메뉴를 열고 목록을 읽는 방식은 그대로였습니다.<br>
방문자가 직접 걷고 발견할 수 있도록 메뉴를 공간으로 바꾸고 **도마도 월드**를 만들었습니다.<br>
<br>
소개와 기술은 길드·텃밭에, 프로젝트와 기록은 풍차·보관소에 연결하고 길과 지형, 건물과 NPC, 이벤트를 하나씩 구상하며 마을을 구성했습니다.<br>
배경음악과 발걸음 소리도 장면과 행동에 맞춰 고르고 연결하며 마을의 분위기를 다듬었습니다.<br>
<br>
내용만 빠르게 확인하고 싶은 방문자를 위해 게임 없이 포트폴리오를 바로 읽는 경로도 함께 만들었습니다.<br>
<br>

## 탐험은 선택지로 남겼습니다

<p align="center">
  <picture>
    <source media="(max-width: 640px)" srcset="./assets/readme/domado-product-system-map-mobile.svg" />
    <img src="./assets/readme/domado-product-system-map.svg" alt="세 가지 대안 경로. 마을에서는 걷고 대화하며 정보 패널을 열고, 바로 보기는 세로 스크롤 포트폴리오를 엽니다. 모바일 세로에서는 8개 카드로 회전 없이 정보를 봅니다." width="100%" />
  </picture>
</p>

| 경로 | 데스크톱 | 모바일 세로 | 역할 |
| --- | :---: | :---: | --- |
| 마을 탐험하기 | O | O · 선택 후 가로 전환 | 걷고 대화하며 건물·주민에 연결된 기록 발견 |
| 포트폴리오 보기 | O | O | 게임 없이 포트폴리오 열람 |
| 세로 모드로 보기 | — | O | 화면을 돌리지 않고 카드 메뉴로 접근 |

정보 지점인 건물·안내 NPC는 상단 QuickMenu와 같은 React 패널 라우터를 사용합니다.<br>
일반 주민과 상인은 월드 안에서 사용자와 상호작용합니다.<br>
키보드 focus trap·Escape 복귀·감소 모션도 적용해 게임을 건너뛰어도 핵심 정보에 바로 들어갈 수 있습니다.<br>
<br>

<details>
<summary>실제 데스크톱·모바일 진입 모션 보기 · 2026년 8월 화면</summary>

당시 실행 화면을 평면화한 데모입니다.<br>
캡처의 `DOMADO PROJECT` 표기는 보존했으며, 현재 브랜드는 **DOMADO WORLD**입니다.<br>
모션은 한 번 재생한 뒤 최종 화면을 유지합니다.<br>

<p align="center">
  <img src="./assets/readme/domado-opening-reveal.svg" alt="2026년 8월 데스크톱 화면. 금색 이음선이 열리며 픽셀 마을과 진입 선택지가 나타납니다." width="100%" />
</p>
<p align="center">
  <img src="./assets/readme/domado-mobile-reveal.svg" alt="2026년 8월 모바일 화면. DOMADO 로고가 왼쪽 위로 이동하고 8개 카드 메뉴가 나타납니다." width="360" />
</p>

</details>

<br>
<br>

## 시스템 구조

마을·퀵 메뉴·모바일 카드는 같은 화면 연결 규칙을 사용합니다.<br>
`포트폴리오 보기`는 게임 초기화 없이 외부 세로 스크롤 포트폴리오를 iframe으로 엽니다.<br>
아래 구조는 2026년 10월 구현을 기준으로 정리했고, 성능·개발 연대기의 과거 뷰어 기록과 구분했습니다.<br>

<p align="center">
  <picture>
    <source media="(max-width: 640px)" srcset="./assets/readme/domado-tech-stack-mobile.svg" />
    <img src="./assets/readme/domado-tech-stack.svg" alt="Canvas는 프레임 상태를, React는 화면 상태를 소유합니다. onInteract와 openSection으로 패널을 열고 paused·renderSuspended를 월드로 전달합니다. 포트폴리오는 외부 iframe, Gemini는 서버리스 API, Supabase·EmailJS는 브라우저 직접 연동입니다." width="100%" />
  </picture>
</p>

<details>
<summary>텍스트 흐름도 보기</summary>

```mermaid
flowchart TB
    Visitor["방문자"] --> Entry["환경별 진입 선택"]
    Entry --> Game["가로 게임 월드"]
    Entry --> Direct["포트폴리오 보기"]
    Entry --> Mobile["모바일 세로 카드"]

    Game --> Canvas["Canvas GameWorld · 입력 / 업데이트 / 충돌 / 렌더"]
    Canvas --> Section["SectionId → App.openSection"]
    Mobile --> Section
    Quick["8개 퀵 메뉴"] --> Section
    Section --> Panels["PANELS 컴포넌트 레지스트리"]
    Section --> Viewer["PortfolioViewer · 외부 iframe"]
    Direct --> Viewer
    Viewer --> Portfolio["세로 스크롤 포트폴리오"]
    Section -. "paused / renderSuspended" .-> Canvas

    Panels --> API["ChatPanel → Vercel /api/gemini"]
    Panels --> Supabase["GuestbookPanel → Supabase"]
    Panels --> EmailJS["ContactPanel → EmailJS"]
```

</details>

| 경계 | 소유하는 상태 | 판단 |
| --- | --- | --- |
| React `App` | 진입, 패널, 퀘스트, 포트폴리오, 전체화면 | 화면 전환처럼 변경 빈도가 낮고 UI 일관성이 중요한 상태 |
| Canvas `GameWorld` | 좌표, 애니메이션, 충돌, 공격, 카메라 | 매 프레임 바뀌는 값을 React 렌더에서 분리 |
| 공용 라우터·레지스트리 | `SectionId`, `openSection`, `PANELS` | 월드·QuickMenu·MobileHome이 같은 패널 연결 규칙 사용 |
| 포트폴리오 연결 | `/portfolio`, iframe, history, postMessage | 외부 문서를 연결하고 메시지의 origin·source를 확인 |
| 서버리스 핸들러 | API 키, 입력 제한, 공급자 오류 변환 | 비밀은 서버에 두고 클라이언트가 처리할 오류 응답 형식을 정의 |
| 외부 서비스 연동 | 방명록과 연락 폼 요청 | 입력 검사·DOMPurify 뒤 Supabase·EmailJS로 브라우저에서 직접 연결 |

Canvas 상태는 근접 대상 변경처럼 실제 UI 표시가 바뀌는 순간에만 React로 전달합니다.<br>
패널 뒤 월드는 완성 프레임을 재사용합니다.<br>
전환막이나 회전 안내가 월드를 가리면 update/draw를 건너뛰지만, 이때 RAF 콜백 자체가 항상 사라지는 것은 아닙니다.<br>
React와 Canvas의 경계는 **변경 빈도와 상태 소유권**으로 정했습니다.<br>
Gemini는 서버리스 함수를, 방명록과 연락 폼은 브라우저에서 각각 Supabase·EmailJS를 사용합니다.<br>
<br>

## 대표 엔지니어링 판단

### 일곱 차례에 걸친 성능 병목 개선

사용자에게 먼저 영향을 주는 병목부터 고쳤습니다.<br>
**1~7차에서 대표 성능 지표 6개**를 골라 콘텐츠 표시·전송량·초기 실행·정지 렌더·플레이 중 프레임 안정성을 정리했습니다.<br>
각 항목의 전후만 비교하며, 서로 다른 차수의 감소율을 합산하지 않습니다.<br>

<p align="center">
  <picture>
    <source media="(max-width: 640px)" srcset="./assets/readme/domado-performance-mobile.svg" />
    <img src="./assets/readme/domado-performance.svg" alt="서로 다른 조건의 대표 성능 지표 6개. 7차 모바일 LCP 6.92→3.46초, 첫 화면 총 전송량 1,606,640→433,644B. 4차 당시 빌드의 메인 JS gzip 214,803→114,888B. 7차 데스크톱 PSI TBT 860→0ms, 개선 후 2회 동일. 6차 모바일 패널 정지 drawImage 36,720→238회/2초, 당시 3회 중앙값. 1차 120Hz 모바일의 20ms 초과 프레임 간격 22→0회/10초. 2026년 7~8월 기록이며 모바일 FCP는 2.10→2.40초로 증가했습니다." width="100%" />
  </picture>
</p>

7차 **모바일 LCP·전송량은 과거 빌드 각 5회 중앙값**입니다.<br>
**데스크톱 TBT는 별도 비교로, 당시 배포 PSI에서 개선 후 2회 모두 0ms**였습니다.<br>
4차 JS는 2026년 8월 4일 당시 빌드 기록입니다.<br>
6차는 패널 일시정지 중 호출 수의 당시 3회 중앙값입니다.<br>
1차는 120Hz 모바일의 10초 구간에서 20ms를 넘은 프레임 간격의 빈도입니다.<br>
게임 FPS나 발열·배터리 개선율을 뜻하지 않습니다.<br>
<br>

구형 뷰어의 영상 준비 시간, 회전 대기 렌더 중단, 오디오·이미지 최적화도 [1~7차 측정 환경·결과·한계](./docs/engineering-cases.md#1-일곱-차례의-성능-개선)에 유지했습니다.<br>
1·6차의 상세 기기 환경과 원시 trace는 보존되지 않았습니다.<br>

#### 초기 월드 로드는 첫 선택 뒤에

데스크톱 시작 화면 뒤에서 GameWorld가 바로 마운트돼 픽셀 아트 로드와 Canvas 합성을 시작했고, 반복 update/draw를 멈춰도 첫 초기화 비용은 그대로 남았습니다.<br>
<br>

첫 화면에서는 GameWorld를 마운트하지 않도록 바꿨습니다.<br>
게임을 고른 뒤 2.8초 전환 화면에서 월드를 준비하게 했습니다.<br>
포트폴리오와 모바일 카드 경로는 게임 초기화를 건너뜁니다.<br>
전체 Galmuri 로드도 첫 선택 뒤로 미루고 공용 월드 SVG의 브라우저 전송량은 `334,820→184,596B`로 줄였습니다.<br>
<br>

<details>
<summary>7차 상세 측정값과 남은 비용 보기</summary>

2026년 8월 25일 데스크톱 배포 PSI에서 TBT는 `860ms → 0ms`로 줄었고, 개선 후 독립 측정 2회 모두 0ms였습니다.<br>
성능 점수는 `70 → 100`이었으며 개선 후 2회 모두 100점이었습니다.<br>
<br>

같은 날 모바일 배포 PSI는 개선 후 2회 모두 94점, LCP 2.9초, TBT 0ms였습니다.<br>
아래 로컬 모바일 과거 빌드 비교와는 측정 환경이 다릅니다.<br>
<br>

모바일 세로 경로는 수정 전에도 GameWorld를 마운트하지 않았습니다.<br>
아래 LCP·전송량은 글꼴 로드 시점과 자산 압축을 포함한 7차 변경 묶음의 결과이며, 월드 초기화 유예 하나의 효과로 해석하지 않습니다.<br>
<br>

2026년 8월 25~26일, 수정 전후 프로덕션 빌드를 같은 모바일 Lighthouse 환경에서 각각 5회 실행했습니다.<br>
아래는 중앙값입니다.<br>

| 모바일 Lighthouse 13.4.1 · 5회 중앙값 | 수정 전 | 수정 후 | 변화 |
| --- | ---: | ---: | ---: |
| 성능 점수 | 75 | 88 | +13 |
| LCP | 6.92초 | 3.46초 | -3.46초 · -50.0% |
| 총 전송량 | 1,606,640B | 433,644B | -73.0% |
| TBT | 0ms | 0ms | 변화 없음 |
| 메인 스레드 작업 | 781ms | 697ms | -10.8% |
| FCP | 2.10초 | 2.40초 | +0.30초 · 느려짐 |

LCP와 전송량은 줄었지만 FCP는 0.30초 느려졌습니다.<br>
수정 후 LCP 3.46초도 더 줄여야 합니다.<br>
실제 사용자 지표가 아닌 동일 조건 실험실 비교이며 자세한 환경과 한계는 [7차 성능 사례](./docs/engineering-cases.md#7차--시작-화면의-네트워크와-메인-스레드)에 정리했습니다.<br>
<br>

GameWorld의 마운트는 늦췄지만 동기 import된 게임 코드는 메인 청크에 남아 있습니다.<br>
초기화 유예와 JavaScript 청크 분리를 같은 개선으로 설명하지 않습니다.<br>

</details>

<br>
<br>

### Gemini 호출을 브라우저 밖으로 옮긴 이유

초기 버전은 `VITE_*` 환경 변수의 Gemini 키를 브라우저에서 읽었습니다.<br>
빌드 결과에 비밀이 포함되지 않도록 Gemini 호출은 Vercel Serverless Function에서 처리했습니다.<br>

- `POST`만 받고 JSON을 파싱하며 Origin과 host가 모두 있으면 두 값을 대조합니다.<br>
- raw 요청의 Content-Length와 문자열 길이에 상한을 두고 질문은 500자, 이전 대화는 4개, 메시지는 600자로 제한합니다.<br>
- 키와 시스템 지식은 서버에서만 사용하고 응답은 `no-store`로 보냅니다.<br>
- 공급자의 `429 / 404 / 그 밖의 upstream 실패`를 구분해 클라이언트에 제한·오프라인 상태로 표시합니다.<br>

Gemini 호출의 **비밀 관리·입력 제한·실패 응답 처리**를 서버 인터페이스 하나에 모았습니다.<br>
<br>

### 모바일 화면과 입력 정책

- 월드 좌표와 `672×448` backing store는 하나만 유지했습니다.<br>
- 모바일 가로는 폭 전체를 보여 주고 세로축만 플레이어를 추적합니다.<br>
- 플로팅 조이스틱과 상황별 단일 액션으로 입력 밀도를 줄였습니다.<br>
- 세로 화면에서는 게임을 조작하는 대신 8개 카드로 정보를 볼 수 있습니다.<br>
- Safari 문제를 동적 viewport, font swap, WebKit 재래스터링으로 나눠 수정했습니다.<br>

<p align="center">
  <img src="./assets/readme/mobile-landscape.png" alt="DOMADO 모바일 가로 화면의 카메라 월드, 플로팅 조이스틱, 단일 액션과 퀵 메뉴" width="100%" />
</p>

증상은 실제 iPhone에서 확인했고 `390×844 / 844×390 / 844×290` 조건의 좌표·흐름 회귀 검사는 Chromium 자동화로 보완했습니다.<br>
모바일 확인 조건은 [모바일 사례](./docs/engineering-cases.md#3-고정-픽셀-월드를-모바일에-유지하기)에, 확인한 기기와 Safari 검증 한계는 [Safari 사례](./docs/engineering-cases.md#4-iphone-safari-viewport-font-swap-raster를-분리하기)에 기록했습니다.<br>
<br>

### 그 밖의 트러블슈팅

| 문제 | 원인과 적용한 해결 | 상세 기록 |
| --- | --- | --- |
| 짧은 효과음의 중복 decode와 장면 전환 중 BGM 겹침 | 필요 시 decode, Promise·AudioBuffer 재사용, 사용자 입력 재시도와 GainNode 교차 전환 적용 | [오디오 수명 주기](./docs/engineering-cases.md#5-오디오를-화면-상태의-수명-주기로-다루기) |
| 장애물 사이 NPC가 반대 방향만 반복하며 끼임 | 재현 검사를 만든 뒤 NPC 전용 회피 영역과 축별 우회, 방향 유지 시간을 추가 | [NPC 이동](./docs/engineering-cases.md#6-npc-끼임-재현부터-이동-정책까지) |
| 미사용 유료 원본이 `public/`을 통해 함께 배포될 위험 | 실행 참조와 allowlist를 감사하고 추적 자산을 `1,008→126`개로 축소 | [에셋 배포 경계](./docs/engineering-cases.md#8-라이선스-에셋을-런타임-월드로-통합하기) |

<br>
<br>

## 직접 설계한 범위와 외부 자산

<p align="center">
  <picture>
    <source media="(max-width: 640px)" srcset="./assets/readme/domado-contribution-map-mobile.svg" />
    <img src="./assets/readme/domado-contribution-map.svg" alt="직접 설계한 제품·UX·인터페이스, 월드·픽셀 가공, 게임 시스템·사운드. 외부 픽셀 원화는 Cute Fantasy by Kenmi, 음원은 CC0·Pixabay 출처입니다." width="100%" />
  </picture>
</p>

| 영역 | 직접 설계·구현한 범위 | 사용한 외부 원본 |
| --- | --- | --- |
| 제품·UX | 콘셉트, 정보 구조, 환경별 진입 분기, 퀵 메뉴, 온보딩 | — |
| 월드 | 구역·동선·깊이·충돌·상호작용, 타일 조합과 오토타일 규칙 | Cute Fantasy by Kenmi 픽셀 아트 |
| 픽셀 파이프라인 | sprite crop, 투명색 처리, 재색상, 회전·반전, 합성, 9-slice | 라이선스 원본 스프라이트·타일셋 |
| 게임 시스템 | 이동, 대화, 조사, 퀘스트, 전투, 낮·밤, 작물, NPC·동물 상태 | — |
| 인터페이스 | React 패널, 외부 포트폴리오 연결, 모바일 8카드 홈, 반응형 분기 | — |
| 사운드 | 출처 확인, 선별, 재인코딩, 재생 시점, buffer 재사용, 교차 전환 | CC0·Pixabay 라이선스 BGM/SFX |

픽셀 원화와 음악은 표에 적은 외부 원본을 사용했습니다.<br>
원본을 선별·가공하고 좌표·깊이·상태·충돌·오디오 수명 주기를 설계했습니다.<br>
이를 하나의 월드로 통합한 작업이 직접 기여한 범위입니다.<br>
<br>

이 저장소에는 공개 가능한 화면·구조·검증 기록만 담았습니다.<br>
유료 원본과 이를 포함한 구현 저장소 이력은 공개하지 않으며 세부 출처와 이용 범위는 [NOTICE](./NOTICE.md)에 기록했습니다.<br>
<br>

## 전체 개발 과정

| 기간 | 전환점 | 결과 |
| --- | --- | --- |
| 2025.11~2026.02 | 레트로 OS형 포트폴리오 | 창·앱 구조와 Supabase·EmailJS·Gemini·오디오 연동 구축 |
| 2026.07.09~13 | OS 셸 폐기, Canvas 월드 전환 | 콘텐츠는 보존하고 이동·충돌·대화·전투·공용 패널을 새로 설계 |
| 07.13~08.02 | 모바일과 살아 있는 마을 | 카메라·조이스틱·퀘스트·낮밤·농장·포트폴리오 뷰어·온보딩 구현 |
| 08.04~25 | 전달 비용·실기기·배포 마감 | 7차 성능 개선, 서버리스 오류 계약, iPhone Safari, 공개 자산 경계 정리 |
| 09~10월 | 포트폴리오 연결·브랜드 정리 | 외부 세로 스크롤 포트폴리오 iframe 연동, history·메시지 계약, DOMADO WORLD 표기 |

각 전환점을 선택한 근거는 [전체 개발 연대기](./docs/development-history.md)에 남겼습니다.<br>
<br>

## 검증

아래는 2026년 8월 비공개 구현 저장소에서 남긴 검증 기록입니다.<br>
이 문서 저장소에는 앱 소스와 실행용 `package.json`이 없습니다.<br>

- `npx tsc --noEmit`과 production build 통과
- 모바일 세로 8카드 경로에서 8개 카드와 콘솔 오류 0 확인
- 7차 변경 뒤 게임·포트폴리오 진입과 `390×844→844×390` 회전 확인

당시 TypeScript 검사 파일 40개 중 29개가 통과했고, 11개는 최종 구현과 기대값이 어긋나 실패했습니다.<br>
구현과 기대값 중 어느 쪽을 고칠지는 추가 판정이 필요합니다.<br>
브라우저 전체 시나리오도 모두 다시 실행하지는 않았습니다.<br>
검증 범위와 남은 작업은 [엔지니어링 사례의 마지막 절](./docs/engineering-cases.md#9-검증-상태와-다음-작업)에 기록했습니다.<br>
<br>

## 상세 기록

- [제품 방향이 바뀐 전체 개발 연대기](./docs/development-history.md)
- [성능·상태 경계·모바일·Safari·오디오·NPC·서버리스 사례](./docs/engineering-cases.md)
- [외부 픽셀 아트·음악·효과음 고지](./NOTICE.md)

<br>
<br>

---

<p align="center">
  <strong>게임으로 둘러보거나, 포트폴리오로 바로 들어가 보세요.</strong><br>
  <br>
  <a href="https://domado.me"><strong>DOMADO 플레이</strong></a>
  ·
  <a href="https://github.com/DO-MADO"><strong>GitHub 프로필 · 박건호</strong></a>
</p>

<p align="center">
  © 2026 DO-MADO. 자체 작성 텍스트·기획·편집 구성의 권리를 보유합니다.<br>
  외부 픽셀 원화와 음원의 권리는 각 원저작자 및 <a href="./NOTICE.md">NOTICE</a>의 라이선스를 따릅니다.<br>
</p>
