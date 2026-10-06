# Park Junseong · Associate PM (AI products)

junsuopar@gmail.com · [GitHub](https://github.com/Artemis-ignis) · [clunk.games](https://clunk.games) · [한국어](resume.ko.md)

I plan, implement, and review three personal products with AI tools. In the ongoing REEZEN team project, I work on survey and interview evidence to revisit the problem hypothesis.

## Products

### clunk.games · live · solo · Aug 2026 – present
Weekly-ranking web games (tower, puzzle, smash) where everyone plays the same daily blocks · Korean and English
- **Ranking and operations:** set weekly fairness rules, server-side score review, and abuse-response limits; after the Sep 25 outage, matched all 110 existing ranks before reopening.
- **Site metric:** on Oct 6, the site showed 132 cumulative players who completed at least one ranked game; this week's leaderboard had no records yet. The count is not de-duplicated customers.
- **Fairness:** same block order per season, server-side score replay, review hold for outliers, per-IP sign-up caps of five per hour and eight per day after finding one IP with 10 accounts.
- **Incident:** a six-hour outage on Sep 25 from exceeding the free DB read quota; moved to a best-score table plus daily snapshot and matched all 110 ranks before reopening.

### DdakDama · public beta · solo · Jul 2026 – present
ChatGPT app + Chrome extension that turns a chat shopping list into a Coupang cart after user approval
- Moved quantity decisions to rule-based code after a test caught "240 tablets" read as 240 items; unpriced items skipped; partial failures listed.
- 94 unit tests, Playwright E2E, 5 real products checked; no real-user test yet.

### Bootcamp team project (REEZEN) · 5 people · Sep 2026 – present
- Proposed NVIDIA Nemotron Korean personas; 60 LLM personas answered the 13-question survey before launch.
- Rebuilt the survey from 13 sections to 7, each question tied to one of five hypotheses; adopted as final.
- Personally conducted one of five team interviews and analyzed all five; held the conclusion open because the Oct 2 summary differed from the earlier analysis.
- The mentor's suggested metric and narrower scope remain undecided by the team.

### Yeosachin (formerly Pictory) · preparing for release · solo · Sep 2026 – present
A travel-photo selection flow that helps users compare similar shots and save their own picks into an album.
- Shows brightness, sharpness, and similar-photo candidates while leaving the final choice to the user.
- Basic organization is free; photos are processed on-device.
- UI and flow are implemented; Toss permissions/file saving, selection time, and repeat use remain untested.

### Naver AI ad contest entry · solo · Sep 2026
21.8-second ad made in two days (version 18) with Codex, Seedance 2.5, HyperFrames, and code-synthesized audio.

## Experience
- **MetaChain** · game planning · Jun 2022 – May 2023 · blockchain game content, NFT/P2E market research, pitch decks
- **LPK Robotics** · design intern · Aug – Sep 2024 · 2D drawings, 3D modeling, interference checks

## Education
- Fastcampus AI Product Manager Bootcamp · Aug – Nov 2026 (in progress)
- Dongyang Mirae University · Management Information Systems · associate degree · 2017 – 2023

[Back to profile](../README.en.md)
