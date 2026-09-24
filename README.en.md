<sub>Park Junseong · Entry-level PM / PO / Service Planning</sub>

# Helping people finish<br>what they set out to do.

<img align="right" src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/portrait.jpg" width="144" alt="Park Junseong portrait" />

### Hello, I'm Junseong.

Shopping recommendations still leave shopping to prepare. After a trip, choosing which near-duplicate photos to keep can feel like another chore. Even a short game is more fun when friends can compete on the same terms and show the result.

These are the problems behind my products. With experience in market research and content planning, I define the problem, user flow and completion criteria, then use AI tools as implementation support and review the result.

[Resume](docs/resume.en.md) · [Product cases, Korean](docs/cases/README.md) · [한국어](README.md)

<br clear="all" />

---

## Three problems, three products

| Product | The job I want to make easier | What you can review |
| --- | --- | --- |
| **DdakDama** | Preparing a purchase after deciding what to buy | Comparison and cart-handoff flow, demo, public code |
| **Yeosachin (formerly Pictory)** | Choosing which travel photos to keep after a trip | Redesigned recommendation, comparison and trip-album screens; preparing for release |
| **Clunk** | Competing with friends on the same terms in a quick game and sharing the result | Two free weekly-ranking games live · clean external user count and retention not yet verified |

## 01 · DdakDama
### From a shopping recommendation to purchase preparation.

**Why I built it.** Even after AI suggests a shopping list, people must search each item again, compare package sizes and prices, then fill a cart. I wanted to reduce the repeated work between the list and the store.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/ddakdama-compare.jpg" width="100%" alt="DdakDama implemented product-comparison screen" />
<sub>Demo using implemented UI and sample product data.</sub>

**The experience.** List input → candidate review → preflight → cart handoff and result review, across the web, GPTs and the Chrome extension as separate surfaces.

**A product decision.** Speed is only useful when the cart contains the intended products. I separated product identity, package contents and purchase quantity, and kept uncertain candidates reviewable. Partial failure leaves a recovery path.

**My contribution.** Problem framing, user flow, quantity and completion criteria, AI-assisted implementation and review. The connected flow and demo are available; purchase-preparation time and task completion are future user-study measures.

[Case study, Korean](docs/cases/ddakdama.md) · [51-second demo](https://youtu.be/hpRkAGgw03c) · [Repository](https://github.com/Artemis-ignis/ddakdama)

---

## 02 · Yeosachin (formerly Pictory)
### A friend who helps you choose your travel photos.

**Why I am refocusing it.** After a trip, similar shots pile up. Comparing them one by one can delay making an album. I am narrowing Pictory's general photo-organization concept to a specific job: choosing the moments worth keeping from a trip.

<p align="center"><img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/yeosachin-home.png" width="60%" alt="Yeosachin implemented travel-photo home screen" /></p>
<sub>September 10, 2026 pre-release implementation. Actual home screen; the companion illustration is AI-generated brand artwork.</sub>

**The experience.** Select travel photos → review suggested and similar shots → keep favorites in a named trip album.

**A product decision.** Brightness and sharpness suggest candidates, not which memories matter. The user makes the final choice. Basic organization is free, without ad or AI-credit gates. Basic classification runs on-device; when the user explicitly chooses the AI path, selected ordinary photos are resized to 384px JPEG before being sent to Gemini for recommendation. Cloud backup and deletion of gallery originals are not offered.

**My contribution and current stage.** Product direction, user flow, free-tier and trust boundaries, AI-assisted implementation and review. Redesigned screens and core photo/album flows are implemented; the app is preparing for release. Real Toss-device permissions and file saving remain to be verified. Reduced selection effort is a hypothesis, not a measured outcome.

[Case study, Korean](docs/cases/pictory.md) · [Product brief, Korean](docs/cases/pictory-brief.md) · [Repository](https://github.com/Artemis-ignis/pictory-apps-in-toss)

---

## 03 · Clunk
### A free web game where everyone stacks the same blocks each week.

**Why I built it.** Casual games are everywhere, but few give friends a fair way to compete and show off the result. Every Monday a new tower opens, everyone gets the same blocks in the same order, and each run ends with a shareable result image.

**Why the product changed.** Clunk started as a tool for finding, inspecting and applying game assets. There was no measured revenue, a subscription competing with free asset packs would have needed too many paying users, and the home page asked visitors to choose between a marketplace, an inspector, AI creation and MCP at once. In September 2026 I turned clunk.games into a site of games you can play immediately, keeping the earlier asset features in place.

<a href="https://clunk.games/en"><img src="docs/assets/pm-portfolio/clunk-games-home-20260924.png" width="100%" alt="clunk.games home: Season #1 weekly ranking and the build-this-week's-tower button" /></a>
<sub>Live site capture, September 24, 2026. Some game-card art is AI-generated.</sub>

**Product decisions.** Rankings only matter if conditions are fair: each season uses the same block order, unusually high scores are held for review, and Clunk Puzzle replays the move log on the server instead of trusting the client score. After the first public post I found one IP creating several accounts for ranked runs and added per-IP sign-up limits. Until a game rating is issued, the games run free and non-commercial, with no paid items or ads.

**My contribution.** The pivot decision; game rules, weekly ranking and fairness policy; the sharing flow and free-release scope; and review of AI-assisted game and site work. Season #1 is live. Right after a community post the site counted 61 new players, 49 distinct IPs and 208 ranked runs, but multi-account play is mixed in, so I do not claim a clean external user count or retention yet. There is no revenue.

[Play this week's tower](https://clunk.games/en) · [Clunk Puzzle](https://clunk.games/puzzle) · [Earlier asset-tool case study, Korean](docs/cases/clunk.md)

<sub>Clunk source remains private; this portfolio presents shareable screens and product decisions.</sub>

---

## Experience I bring to a team

- **Research into execution:** at MetaChain, I worked on emerging-market research, internal education, proposals, content and launch materials.
- **Ideas into working flows:** in personal projects, I define requirements, use AI tools to implement them, inspect the results and follow up on changes.
- **Attention to practical constraints:** drawings, 3D modeling and assembly checks at LPK Robotics helped me understand the gap between intent and implementation.

| Experience | Period |
| --- | --- |
| MetaChain · game content planning and marketing | Jun 2022–May 2023 |
| LPK Robotics · design intern | Aug–Sep 2024 |
| Dongyang Mirae University · Business Information Systems, associate degree | Mar 2017–Feb 2023 |
| FastCampus AI Product Manager Advanced Camp, Cohort 10 | In progress |

I am seeking entry-level PM/PO and service-planning opportunities in AI, commerce and content. I want to extend my hands-on building experience through customer research, team collaboration and post-launch analysis.

**How I use AI and evidence.** I own problem framing, user and priority decisions, completion criteria and quality judgment. AI tools assist with code, documents and visual material. I verify the result with browser, file and test evidence, and do not present unmeasured users, revenue, conversion or time savings as outcomes.

[Read my resume →](docs/resume.en.md)

<sub>Personal projects demonstrate planning, AI-assisted implementation and review. User growth, revenue and conversion will be added when measured.</sub>

## Product briefs

Reconstructed for this portfolio on September 10, 2026, using existing product screens and records. These describe requirements, scope reasoning and proposed validation, not historical PRDs or completed user studies.

[DdakDama](docs/cases/ddakdama-brief.md) · [Yeosachin](docs/cases/pictory-brief.md) · [Clunk, earlier version](docs/cases/clunk-brief.md) — Korean
