<img align="right" src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/portrait.jpg" width="128" alt="Park Junseong" />

# Park Junseong · Associate PM (AI products)

I plan, ship, and run products with AI tools. On my own I built a weekly-ranking web game that is live, a Chrome extension in public beta, and a YouTube channel that Claude runs on a schedule. In a five-person bootcamp team project I own the survey and hypothesis testing.

**[Resume PDF (Korean)](docs/pm-resume-ko.pdf)** · **[Portfolio PDF (Korean)](docs/pm-portfolio-ko.pdf)** · [Resume](docs/resume.en.md) · [한국어](README.ko.md) · junsuopar@gmail.com

<br clear="all" />

| 116 | 31 | 4,403 | 60 |
| --- | --- | --- | --- |
| clunk.games players this week (Sep 27; 119 all-time) | clunk.games deploys in 4 days · 331 automated checks before each deploy | views on 4 Shorts run by Claude (Sep 26) | LLM personas that pre-tested the team survey |

---

## 01 · clunk.games · a live weekly-ranking web game

A new block set drops at midnight every day and every player stacks the same blocks. Three games (tower, puzzle, smash) run in Korean and English, and rankings reset every Monday.

<a href="https://clunk.games"><img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/clunk-games-home-20260927.jpg" width="100%" alt="clunk.games home" /></a>

- **Pivot decision.** Clunk launched as a game-asset tool. Measured revenue was zero, reaching US$1,000 a month against free asset packs needed about 143 paying subscribers, and four features competed on one home screen. On Sep 23 I turned the domain into a play-first game site. Four days later: 116 players and 508 ranked runs that week.
- **Fair rankings.** Same block order for everyone each season; puzzle scores are recomputed on the server from replayed inputs; unusually high scores wait for review. After spotting one IP with 10 accounts and 60 ranked runs, I capped sign-ups at 5 per hour and 8 per day per IP. Site numbers are therefore not reported as clean external users.
- **Incident.** On Sep 25 a query that re-read a week of records on every ranking view exceeded the free DB read quota and took the site down for about six hours. I moved rankings to a best-score table plus a daily snapshot and checked all 110 ranks against the old results before reopening.

[Play →](https://clunk.games) · source is private

## 02 · DdakDama · from a ChatGPT shopping list to a Coupang cart

GPT-5.6 turns a chat into a shopping list; a Chrome extension paired by a 6-digit code finds Coupang candidates and adds them only after the user approves. It never handles payment or passwords.

- A test caught the list parser reading "100mg, 240 tablets" as 240 items, so quantity decisions moved into rule-based code.
- Items without a confirmed price are skipped; partial failures are listed separately.
- 94 unit tests, Playwright E2E, 5 real Coupang products checked. No real-user test yet.

[Try without installing →](https://ddakdama.artemis-clunk.workers.dev/try) · [51s demo →](https://youtu.be/hpRkAGgw03c) · [Repo →](https://github.com/Artemis-ignis/ddakdama)

## 03 · Bootcamp team project · hypothesis testing first

Team REEZEN (5 people) tests whether Gen Z shoppers abandon online clothing purchases because they are unsure about fit and style.

- Proposed NVIDIA's Nemotron Korean persona dataset (1M synthetic people based on official statistics). 60 personas answered the 13-question survey through an LLM simulation before launch; the mentor called it "really impressive."
- Rebuilt the team survey from 13 sections to 7 and tied every question to one of five hypotheses; the revision became the final survey.
- Ran a user interview and transcribed it locally with Whisper.

## 04 · 어제의 나에게 · a YouTube Shorts channel run by Claude

Claude reads a rules file and yesterday's notes, then writes, animates, uploads, and checks comments on a Mon/Wed/Fri + Sunday schedule. Episode 4 went up with no human edit. After a weak first episode I switched to code-driven character animation; episodes 2–4 each passed 1,100 views. [Channel →](https://www.youtube.com/@ignisbuilds)

## 05 · Naver AI ad contest entry · 21.8 seconds

Made in two days and submitted as version 18. Codex images, Seedance 2.5 video, HyperFrames captions, and code-synthesized audio. When a key word sounded wrong, I traced it to a sound effect masking a syllable, moved it, and confirmed with Whisper. [Watch →](https://youtube.com/shorts/9ie83icRAOI)

## Experience · education

| Period | |
| --- | --- |
| 2026.08 – 2026.11 | Fastcampus AI Product Manager Bootcamp (in progress) |
| 2024.08 – 2024.09 | LPK Robotics · design intern |
| 2022.06 – 2023.05 | MetaChain · game planning (blockchain game content, market research, pitch decks) |
| 2017.03 – 2023.02 | Dongyang Mirae University · Management Information Systems (associate degree) |
