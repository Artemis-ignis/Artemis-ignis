<img align="right" src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/portrait.jpg" width="128" alt="Park Junseong" />

# Park Junseong · Associate PM (AI products)

I define user problems, product scope, and acceptance criteria, then use AI tools to implement and review the work. This portfolio separates my role and verified evidence across three personal products and an ongoing REEZEN team project.

**[Resume PDF (Korean)](docs/pm-resume-ko.pdf)** · **[Portfolio PDF (Korean)](docs/pm-portfolio-ko.pdf)** · [Resume web version](docs/resume.en.md) · [한국어](README.ko.md) · junsuopar@gmail.com

<br clear="all" />

| 132 | 110/110 | 5 | 13→7 |
| --- | --- | --- | --- |
| Clunk cumulative players completing a ranked game (site value, Oct 6) | Existing ranks matched after the Sep 25 outage | Total REEZEN interview participants | Sections in the revised REEZEN survey |

Clunk’s 132 is the site’s own completed-ranked-game count, not a de-duplicated customer count. When checked on Oct 6, this week’s leaderboard had no records yet.

---

## 01 · Clunk · operating a weekly-ranking web game

Three games—tower, puzzle, and smash—share a weekly leaderboard. Every player receives the same daily block sequence.

<a href="https://clunk.games"><img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/clunk-games-home-20260927.jpg" width="100%" alt="Clunk weekly-ranking game home, captured Sep 27, 2026" /></a>

**Product rules and operations**
- Puzzle scores are recalculated on the server by replaying input records. Unusually high scores wait for review before appearing on the leaderboard.
- After finding multiple ranking accounts behind one IP, I set sign-up limits of five per hour and eight per day per IP. Site play counts are not reported as clean external users.
- On Sep 25, a query that re-read a week of records on every leaderboard view exceeded the free database read quota and took the site down for about six hours. I moved reads to a best-score table and daily rank snapshots, then matched all 110 existing ranks before reopening.

**My role** · Game and ranking rules, abuse-response policy, incident response, and recovery review. AI tools supported implementation, automated checks, and deployment.

[Live site →](https://clunk.games) · [Detailed case →](docs/cases/clunk.md) · Source repository is private.

---

## 02 · Ddakdama · from a ChatGPT shopping list to a Coupang cart

Users review product candidates from a ChatGPT shopping list, then approve items in a Chrome extension before they reach the Coupang cart. The product never handles payment or passwords.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/ddakdama-flow.jpg" width="100%" alt="Ddakdama list, product review, and cart handoff" />

**Accuracy and recovery**
- A test caught “one bottle of 100mg, 240 tablets” being read as 240 items, so quantity interpretation moved into rule-based code.
- Items without confirmed prices are not added automatically; partial failures are listed for review.
- Verified 94 unit tests, Playwright E2E, five real Coupang products, and ChatGPT app connection. No real-user task or purchase-time improvement has been measured.

[Try without installing →](https://ddakdama.artemis-clunk.workers.dev/try) · [51-second demo →](https://youtu.be/hpRkAGgw03c) · [Repo →](https://github.com/Artemis-ignis/ddakdama) · [Case →](docs/cases/ddakdama.md)

---

## 03 · Yeosachin (formerly Pictory) · choosing travel photos

A photo-organizing app is being reshaped around choosing which similar travel photos to keep in an album. Recommendations surface candidates; the user makes the final choice.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/yeosachin-home.png" width="72%" alt="Yeosachin redesign home screen" />

**My role** · Product focus and flow, free scope, privacy and file-handling rules, plus AI-assisted implementation and review.

The redesign is being prepared for release. Toss app permissions and file saving, selection-time impact, and repeat use have not been validated; no user outcome is claimed.

[Case →](docs/cases/pictory.md) · [Brief →](docs/cases/pictory-brief.md) · [Repo →](https://github.com/Artemis-ignis/pictory-apps-in-toss)

---

## 04 · REEZEN · ongoing e-commerce team project

The team started with a hypothesis that Gen Z shoppers delay clothing purchases because fit and size are uncertain. In the Oct 2 summary of five team interviews, reasons for delaying a purchase included no immediate need, season, expected wear frequency, and value for price; zero of five cited uncertainty about whether an item would suit them. The same summary said discovery was fine but comparing prices for the same item took time.

A Sep 30 interview analysis instead described all five as getting stuck at the confirmation stage. The summaries appear to use different questions or aggregation rules, so I left the discrepancy open rather than presenting a final problem statement. Five exploratory interviews do not represent the broader market.

**My role** · Proposed the Nemotron Korean synthetic-persona dataset and used 60 LLM responses to pre-check the survey flow; these are not real-user validation. Proposed reducing the survey from 13 to 7 sections and branches from 5 to 1, replacing importance scales with behavior questions; the final team survey adopted the revision. I personally conducted one of the five interviews, analyzed all five, and wrote a Sep 30 proposal to explore recurring shopping problems before narrowing the target.

At the Oct 2 mentoring session, the mentor recommended selecting one metric and narrowing the problem and category. Those remain team decisions, not completed choices. The survey denominator is omitted because project documents disagree.

[Case and current status →](docs/cases/reezen.md)

---

## Experience · education

| Period | |
| --- | --- |
| 2026.08 – 2026.11 | Fastcampus AI Product Manager Bootcamp · in progress |
| 2024.08 – 2024.09 | LPK Robotics · design intern · 2D drawings, 3D modeling, interference review |
| 2022.06 – 2023.05 | MetaChain · game planning · blockchain game content, NFT/P2E research, pitch materials |
| 2017.03 – 2023.02 | Dongyang Mirae University · Management Information Systems, associate degree |

<sub>Metrics and status are dated snapshots. See the [case index](docs/cases/README.md) for project materials.</sub>
