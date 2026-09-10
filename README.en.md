<sub>Park Junseong · Entry-level PM / PO / Service Planning</sub>

# Helping people finish<br>what they set out to do.

<img align="right" src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/portrait.jpg" width="144" alt="Park Junseong portrait" />

### Hello, I'm Junseong.

Shopping recommendations still leave shopping to prepare. After a trip, choosing which near-duplicate photos to keep can feel like another chore. Game ideas can stall while the creator prepares assets.

These are the problems behind my products. With experience in market research and content planning, I define product direction and user flows, then use AI tools to implement and review the experience.

[Resume](docs/resume.en.md) · [Product cases, Korean](docs/cases/README.md) · [한국어](README.md)

<br clear="all" />

---

## Three problems, three products

| Product | The job I want to make easier | What you can review |
| --- | --- | --- |
| **DdakDama** | Preparing a purchase after deciding what to buy | Comparison and cart-handoff flow, demo, public code |
| **Yeosachin (formerly Pictory)** | Choosing which travel photos to keep after a trip | Redesigned recommendation, comparison and trip-album screens; preparing for release |
| **Clunk** | Finding and preparing assets before starting game creation | Beta service, marketplace and file-inspection workflow |

## 01 · DdakDama
### From a shopping recommendation to purchase preparation.

**Why I built it.** Even after AI suggests a shopping list, people must search each item again, compare package sizes and prices, then fill a cart. I wanted to reduce the repeated work between the list and the store.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/ddakdama-compare.jpg" width="100%" alt="DdakDama implemented product-comparison screen" />
<sub>Demo using implemented UI and sample product data.</sub>

**The experience.** List input → candidate review → preflight → cart handoff and result review, across web, extension and ChatGPT entry points.

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

**A product decision.** Brightness and sharpness suggest candidates, not which memories matter. The user makes the final choice. Basic organization is free, without ad or AI-credit gates. Photos are processed on-device; cloud backup and deletion of gallery originals are not offered.

**My contribution and current stage.** Product direction, user flow, free-tier and trust boundaries, AI-assisted implementation and review. Redesigned screens and core photo/album flows are implemented; the app is preparing for release. Real Toss-device permissions and file saving remain to be verified. Reduced selection effort is a hypothesis, not a measured outcome.

[Case study, Korean](docs/cases/pictory.md) · [Product brief, Korean](docs/cases/pictory-brief.md) · [Repository](https://github.com/Artemis-ignis/pictory-apps-in-toss)

---

## 03 · Clunk
### Help game ideas get past asset preparation.

**Why I built it.** Creators need to find or make assets, inspect files and prepare them for their project. Those tasks are scattered across tools. I wanted to bring that preparation together so creators can move on to making their game.

<img src="https://raw.githubusercontent.com/Artemis-ignis/Artemis-ignis/main/docs/assets/pm-portfolio/clunk-home.png" width="100%" alt="Clunk live homepage: asset previews and marketplace, creation and inspection entry points" />
<sub>Live homepage capture, September 8, 2026.</sub>

**The experience.** Asset discovery and creation → preview → file inspection → download and use preparation.

**A product decision.** A visual preview alone does not finish the creator's task. I connected discovery with file evidence and reviewed file checks, rendering and human quality approval separately. Browser inspection also informed navigation, responsive-layout and scrolling improvements.

**My contribution.** Direction, requirements, priorities, quality criteria and review of AI-generated results. A beta service and recorded file-verification workflows are available. Creator interviews and real use tasks are the next validation step; compatibility with every asset and engine is not claimed.

[Case study, Korean](docs/cases/clunk.md) · [Live product](https://clunk.games) · [Public inspection tool](https://github.com/Artemis-ignis/clunk-mcp)

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
| Dongyang Mirae University · Business Information Systems, associate degree | 2017–2023 |
| FastCampus AI Product Manager Advanced Camp, Cohort 10 | In progress |

I am seeking entry-level PM/PO and service-planning opportunities in AI, commerce and content. I want to extend my hands-on building experience through customer research, team collaboration and post-launch analysis.

[Read my resume →](docs/resume.en.md)

<sub>Personal projects demonstrate planning, AI-assisted implementation and review. User growth, revenue and conversion will be added when measured.</sub>

## Product briefs

Reconstructed for this portfolio on September 10, 2026, using existing product screens and records. These describe requirements, scope reasoning and proposed validation, not historical PRDs or completed user studies.

[DdakDama](docs/cases/ddakdama-brief.md) · [Yeosachin](docs/cases/pictory-brief.md) · [Clunk](docs/cases/clunk-brief.md) — Korean
