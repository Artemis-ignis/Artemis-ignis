<!-- ARTEMIS-IGNIS-TOP:START -->
<p align="center">
  <img src="docs/assets/artemis-ignis-emblem-top.jpg?v=20260605-top-emblem" alt="Artemis-Ignis emblem" width="420" />
</p>
<!-- ARTEMIS-IGNIS-TOP:END -->

<h1 align="center">Artemis-Ignis</h1>
<p align="center"><strong>AI Product Manager(프로덕트 매니저) · AI Product Builder(프로덕트 빌더)</strong></p>
<p align="center">
모호한 사용자 문제를 검증 가능한 제품 가설로 바꾸고, 가장 작은 End-to-End(처음부터 끝까지 이어지는) 범위를 정해 실제로 동작하는 AI 제품까지 만들어 검증합니다.
</p>

<p align="center">
  <a href="README.md">English profile</a>
</p>

## 제품을 보는 기준

저는 제품을 세 가지 질문으로 봅니다.

1. **사용자 가치** — 우리가 바꾸려는 실제 사용자 행동과 불편은 무엇인가?
2. **사업성** — 이 제품이 지속 가능한 사업이 될 만큼 충분한 가치를 만들 수 있는가?
3. **구현 가능성** — 지금 가진 자원으로 실제로 만들고, 운영하고, 검증하고, 개선할 수 있는가?

기능 목록이나 화면 목업에서 끝내기보다 **문제 정의 → 가설 → 범위 설정 → 구현 → 검증 → 개선**까지 연결하는 것을 중요하게 생각합니다.

## 대표 제품

| 제품 | 해결하려는 문제 | 제품 / PM 관점의 역할 | 상태 |
| --- | --- | --- | --- |
| **[Clunk](https://github.com/Artemis-ignis/clunk)** · [서비스](https://clunk.games) | 게임 제작자는 생성 도구, 에셋 검사, 마켓, 엔진 연동을 따로 오가며 ‘이 에셋을 실제 게임에 써도 되는가’를 판단할 근거가 부족합니다. | 생성 → 검사 → 마켓 탐색 → 에이전트 연동까지 하나의 제품 흐름으로 설계했습니다. 시장 가설, 에셋 감사, 문구 감사, 제품 경계, 품질 기준, 검증 후 의사결정을 PM 포트폴리오로 기록합니다. | **실서비스 / 지속 개발** |
| **[딱담아](https://github.com/Artemis-ignis/ddakdama)** | AI가 장보기 목록을 추천해도 사용자는 다시 상품을 검색하고, 용량·수량을 해석하고, 후보를 비교하고, 장바구니를 직접 다시 만들어야 합니다. | 자연어 장보기 목록 → 상품 후보 비교 → 검증된 장바구니 전달 흐름을 설계했습니다. 상품 정체성, 포장 단위, 요청 수량, 최종 사용자 승인을 분리해 다룹니다. | **공개 프로토타입** |
| **[픽토리](https://github.com/Artemis-ignis/pictory-apps-in-toss)** | 사진 정리는 반복적이지만, 이미지 분류에는 개인정보와 신뢰 문제가 있고 수익화까지 붙이면 제품 경계가 더 복잡해집니다. | Apps in Toss(앱인토스) 미니앱으로 로컬 우선 처리, 민감 이미지 보호, 사용량 제한, 보상형 접근, 구독 권한, 출시 전 검증 기준까지 제품 범위에 포함했습니다. | **앱인토스 제품 개발** |
| **[Artemis Orchestration App](https://github.com/Artemis-ignis/artemis-orchestration-app)** | 여러 모델과 에이전트를 함께 쓰면 채팅, 파일, 라우팅, 실행 상태, 로그가 흩어져 전체 작업 흐름을 이해하기 어렵습니다. | 채팅·파일·오케스트레이션·로그·런타임 상태를 한 화면에서 확인할 수 있는 Local-first(로컬 우선) 작업공간을 만들었습니다. | **오픈소스 / 지속 개발** |

### Clunk — PM Case Study(제품 사례)

Clunk는 제가 제품을 어떻게 정의하고 검증하는지 가장 잘 보여주는 프로젝트입니다.

단순히 ‘AI로 게임 에셋을 생성하는 기능’으로 보지 않고, 더 큰 Job(사용자가 달성하려는 일)인 **“아이디어를 실제 게임에 넣어도 되는 신뢰 가능한 에셋으로 바꾸는 과정”**을 제품 문제로 다시 정의했습니다.

저장소에는 별도의 **[PM 포트폴리오](https://github.com/Artemis-ignis/clunk/tree/main/docs/portfolio)**가 있으며 문제 정의, 제품 판단, 시장 가설, 품질 감사, AI 실패 사례, 운영 제약, 검증 후 변경 사항을 기록하고 있습니다.

## 일하는 방식

```text
사용자 행동 관찰
    ↓
문제 정의
    ↓
제품 가설 수립
    ↓
가장 작은 End-to-End 범위 설정
    ↓
구현 / 프로토타이핑
    ↓
실제 근거로 검증
    ↓
문제 기록 → 학습 → 반복 개선
```

**Problem Statement(문제 정의), JTBD(고객이 달성하려는 일), User Journey(사용자 여정), MVP(최소기능제품) 범위, Acceptance Criteria(수용 기준), 실패 경계, 출시 체크리스트, 검증 근거**를 중요하게 봅니다. AI 제품에서는 모델의 불확실성, Human-in-the-loop(사람의 최종 검토), 개인정보, 도구 권한, 실패 시 복구 방식도 구현 세부사항이 아니라 제품 의사결정이라고 생각합니다.

## 제품 역량

**제품 탐색 · 전략**
- 문제 정의, 5 Whys(5번 왜), JTBD, 페르소나, 사용자 여정 설계
- Lean Canvas(린 캔버스), PSF/PMF(문제-해결 적합성/제품-시장 적합성) 사고, 가치 제안과 비즈니스 모델 가설
- MVP 범위 설정, 우선순위, 제품 요구사항, 수용 기준

**AI 제품 설계**
- LLM(대규모 언어 모델), Agent(에이전트), Orchestration(오케스트레이션), MCP 기반 제품 흐름
- Human-in-the-loop, 실패 복구, 검증, 안전 경계 설계
- 모델의 기술적 능력을 사용자가 이해하고 통제할 수 있는 제품 경험으로 변환

**실행 · 기술 이해**
- TypeScript, React, Node.js, Python, Cloudflare, GitHub Actions
- 제품 QA(품질 검증), Release Gate(출시 기준), CI(지속적 통합), 문서화와 재현 가능한 검증
- 직접 프로토타입을 만들고 엔지니어링과 시스템 수준에서 협업할 수 있는 구현 이해도

## 배경

한 분야만 경험하기보다 사업, 현장 제약, 기술을 모두 경험한 것이 제 제품 관점의 기반입니다.

- **이커머스 운영** — 펫푸드 온라인 스토어를 직접 운영하며 상품 소싱, 상세페이지, SEO, 고객 응대, 운영까지 End-to-End로 경험했습니다. 핵심 공급사 의존도가 높을 때 사업 구조가 얼마나 취약해지는지도 직접 경험했습니다.
- **로봇 · 기계설계** — 2D 도면, 3D 모델링, 어셈블리, 간섭 검토를 수행하며 ‘만들 수 있는가’를 먼저 확인하는 습관을 익혔습니다.
- **Web3 · 메타버스 신사업 기획** — 신시장 조사, 사내 교육자료, 투자 제안서, 프로젝트 사이트와 SNS 런칭 과정에 참여했습니다.
- **AI 제품 개발** — 현재는 AI-native(AI 중심) 제품 기획, 빠른 검증, 사용자 가치와 실제 기술 실행을 연결하는 제품 개발에 집중하고 있습니다.

## 현재 집중하는 것

- **Clunk**를 AI 게임 에셋 제품·마켓플레이스로 발전시키고 실제 시장 가설을 검증하는 일
- 에이전트가 행동하되 사용자가 결과를 이해하고, 검증하고, 통제할 수 있는 AI 제품 설계
- AI Product Management(제품 관리) 교육과 프로젝트를 통해 제품 탐색, 데이터 기반 의사결정, End-to-End PM 실행 역량을 강화하는 일

## 링크

- **GitHub:** [Artemis-ignis](https://github.com/Artemis-ignis)
- **Clunk:** [clunk.games](https://clunk.games)
- **Clunk PM 포트폴리오:** [docs/portfolio](https://github.com/Artemis-ignis/clunk/tree/main/docs/portfolio)
- **Support:** [Ko-fi](https://ko-fi.com/artemisignis)

<!-- ARTEMIS-IGNIS-FOOTER-BANNER:START -->
<p align="center">
  <img src="docs/assets/artemis-ignis-footer-banner.png?v=20260605-footer-banner" alt="Artemis-Ignis banner" width="100%" />
</p>
<!-- ARTEMIS-IGNIS-FOOTER-BANNER:END -->
