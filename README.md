<img align="right" src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/portrait.jpg" width="128" alt="박준성 프로필 사진" />

# 박준성 · 신입 PM (AI 서비스)

AI 도구로 제품을 기획하고 출시해 운영합니다. 운영 중인 웹 게임, 공개 베타 확장 프로그램, Claude가 운영하는 유튜브 채널을 혼자 만들었고, 패스트캠퍼스 AI 심화캠프 팀 프로젝트에서는 설문과 가설 검증을 맡고 있습니다.

**[이력서 PDF](docs/pm-resume-ko.pdf)** · **[포트폴리오 PDF](docs/pm-portfolio-ko.pdf)** · [이력서 웹 버전](docs/resume.ko.md) · [English](README.en.md) · junsuopar@gmail.com

<br clear="all" />

| 116명 | 31번 | 4,403회 | 60명 |
| --- | --- | --- | --- |
| clunk.games 이번 주 플레이어 (9월 27일, 누적 119명) | clunk.games 4일 동안 배포 · 배포 전 자동 점검 331개 | Claude가 운영하는 쇼츠 4편 조회수 (9월 26일) | 팀 설문을 미리 점검한 LLM 가상 응답자 |

---

## 01 · clunk.games · 운영 중인 주간 랭킹 웹 게임

매일 0시에 새 블록이 나오고 모든 플레이어가 같은 블록으로 겨루는 웹 게임입니다. 탑 쌓기, 퍼즐, 건물 부수기 3종을 한국어와 영어로 운영하고, 순위는 월요일 0시에 새로 시작합니다.

<a href="https://clunk.games"><img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/clunk-games-home-20260927.jpg" width="100%" alt="clunk.games 홈 화면" /></a>

**게임 에셋 도구를 접고 게임 사이트로 바꾼 결정**
Clunk는 게임 에셋을 찾고 검사하는 도구로 먼저 출시했습니다. 측정된 매출이 0원이었고, 무료 에셋 팩과 경쟁하는 구독으로 월 1,000달러를 벌려면 유료 구독자가 약 143명 필요했습니다. 홈 한 화면에서는 마켓, 검사기, AI 제작, MCP 네 기능이 서로 경쟁했습니다. 이 세 가지를 근거로 9월 23일 도메인 첫 화면을 바로 플레이하는 게임으로 바꿨고, 나흘 뒤 이번 주 플레이어 116명, 랭킹전 508판이 됐습니다.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/clunk-pivot.jpg" width="100%" alt="에셋 도구에서 게임 사이트로 바꾼 근거" />

**랭킹을 믿을 수 있게 만든 규칙**
- 시즌마다 모든 플레이어에게 같은 블록을 같은 순서로 줍니다.
- 퍼즐 점수는 서버가 입력 기록을 다시 재생해 계산하고, 비정상적으로 높은 기록은 순위표에 올리기 전에 검토 대기로 둡니다.
- 9월 24일 새벽 한 IP가 계정 10개로 랭킹전 60판을 한 것을 발견하고, IP당 가입을 시간당 5개, 하루 8개로 제한했습니다. 이 때문에 사이트 수치는 정제된 외부 사용자 수로 쓰지 않습니다.

**9월 25일 6시간 장애**
순위를 볼 때마다 한 주 치 기록을 전부 읽는 쿼리가 DB 무료 읽기 한도(하루 500만 행)를 넘겨 서비스가 약 6시간 멈췄습니다. 플레이어별 최고 기록 테이블과 하루 한 번 저장하는 순위표로 바꾸고, 새 순위가 기존 순위와 같은지 110명 모두 대조한 뒤 다시 열었습니다.

**내가 맡은 일** · 방향 전환 결정, 게임 규칙과 랭킹 정책, 운영 대응, 결과 검수. 구현과 점검, 배포는 Claude Code와 서브에이전트가 맡았고 배포 전에는 폰과 PC 화면에서 자동 점검 331개를 거칩니다.

[게임하러 가기 →](https://clunk.games) · 소스 저장소는 비공개

---

## 02 · 딱담아 · ChatGPT 쇼핑 목록을 쿠팡 장바구니로

ChatGPT에 필요한 물건을 말하면 GPT-5.6이 쇼핑 목록으로 정리하고, 6자리 코드로 연결한 Chrome 확장 프로그램이 쿠팡에서 후보를 찾아 사용자가 승인한 뒤에만 장바구니에 담습니다. 결제와 비밀번호는 다루지 않습니다.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/ddakdama-flow.jpg" width="100%" alt="딱담아 동작 흐름: ChatGPT 앱, 연결 서버, Chrome 확장, 쿠팡 장바구니" />

**담기 전에 막아 둔 것**
- ‘100mg 240정’ 한 통을 240개로 읽는 오류를 테스트에서 찾아, 용량·함량·개수 판단을 규칙 코드로 옮겼습니다.
- 가격이 확인되지 않은 상품은 담지 않고, 한 번 더 승인해야 장바구니가 바뀝니다.
- 일부만 담기면 실패한 상품을 따로 보여 줍니다.

**검증 상태** · 단위 테스트 94개, Playwright E2E, 실제 쿠팡 상품 5종 확인, ChatGPT 앱 연결 확인. 실사용자 테스트는 아직 하지 않았습니다.

[설치 없이 써 보기 →](https://ddakdama.artemis-clunk.workers.dev/try) · [51초 데모 →](https://youtu.be/hpRkAGgw03c) · [저장소 →](https://github.com/Artemis-ignis/ddakdama)

---

## 03 · AI 심화캠프 팀 프로젝트 · 문제 검증부터 다시 세운 기획

이커머스 1팀 REEZEN(5명)에서 Gen Z가 온라인으로 옷을 살 때 어울림과 사이즈에 확신이 없어 구매를 포기한다는 가설을 검증하고 있습니다.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/camp-persona-simulation.jpg" width="100%" alt="Nemotron 페르소나 60명 LLM 설문 시뮬레이션" />

- **가상 응답자로 먼저 점검:** NVIDIA Nemotron 한국어 페르소나 데이터셋(통계청 통계 기반 가상 인물 100만 명)을 찾아 팀에 제안했습니다. 60명이 각자 그 인물로 설문 13문항에 답하는 LLM 시뮬레이션으로 배포 전에 가설을 점검했고, 멘토링에서 “너무 인상적”이라는 평가를 받았습니다.
- **설문 개편:** 팀 설문을 13개 섹션에서 7개로 다시 짜고 모든 문항을 가설 5개에 연결했습니다. 응답이 4~5점에 몰리는 중요도 척도 문항은 실제 행동을 묻는 문항으로 바꿨고, 개편안이 팀 최종 설문에 반영됐습니다.
- **인터뷰:** 사용자 인터뷰를 진행하고 로컬 Whisper로 받아써 가설별로 정리했습니다.
- **개인 실습에서 바꾼 순서:** 딱담아 기획을 캠프 실습에 적용하다가 기능 설명이 사용자 문제보다 앞서 있다는 것을 발견하고, 문제 정의, 구매 여정, 가설, 행동 설문 순서로 다시 세웠습니다.

---

## 04 · 어제의 나에게 · Claude가 운영하는 유튜브 쇼츠 채널

Claude가 매번 규칙 파일과 전날 메모를 읽고 대본, 코드 애니메이션, 업로드, 댓글 확인을 한 뒤 메모를 남깁니다. 월·수·금 20시와 일요일에 예약 실행되고, 4편은 사람 손을 거치지 않고 올라갔습니다. 1편(AI 이미지)은 반응이 약해 잘된 AI 영상과 비교한 뒤 2편부터 캐릭터를 코드로 움직였습니다. 9월 26일 기준 1편 856회, 2~4편은 각각 1,100회를 넘었습니다.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/yesterday-channel.jpg" width="100%" alt="어제의 나에게 예약 실행 흐름과 장면" />

[채널 →](https://www.youtube.com/@ignisbuilds)

---

## 05 · 넾다세일 광고 · 네이버 AI 광고제 출품작 21.8초

이틀 동안 18번째 버전까지 만들어 9월 26일에 냈습니다. 가상 배우와 배경은 Codex 이미지, 영상과 대사는 Seedance 2.5, 자막은 HyperFrames로 만들고 음악과 효과음은 코드로 합성했습니다. ‘넾다’가 ‘냅사’로 들린다는 피드백을 받고, 효과음이 ‘다’ 음절을 덮는 것을 찾아 위치를 옮긴 뒤 Whisper 받아쓰기로 확인했습니다.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/nepda-ad-storyboard.jpg" width="100%" alt="넾다세일 광고 장면 9컷과 제작 흐름" />

[광고 영상 →](https://youtube.com/shorts/9ie83icRAOI)

---

## 경력 · 학력

| 기간 | 내용 |
| --- | --- |
| 2026.08 – 2026.11 | 패스트캠퍼스 AI 심화캠프 10회차 (AI Product Manager Bootcamp) · 수강 중 |
| 2024.08 – 2024.09 | LPK Robotics · 설계 인턴 · 2D 도면, 3D 모델링, 간섭 검토 |
| 2022.06 – 2023.05 | 메타체인 · 게임기획 사업부 · 블록체인 게임 콘텐츠 기획, NFT·P2E 시장 조사, 투자 제안서 |
| 2017.03 – 2023.02 | 동양미래대학교 경영정보학과 · 전문학사 |

<sub>수치는 적어 둔 날짜에 사이트와 공개 페이지에서 확인한 값입니다. 예전 에셋 도구 시절 Clunk 사례는 [여기](docs/cases/clunk.md)에 남겨 두었습니다.</sub>
