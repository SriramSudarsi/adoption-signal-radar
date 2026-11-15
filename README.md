# Adoption Signal Radar: DAP Market Intelligence Prototype

**Prepared by Sriram Sudarsi, PGP-SM, IIM Lucknow**

A one-page market-intelligence tool for the leadership team or founder's office of a digital adoption platform (DAP) or SaaS company. It answers four questions:

1. **How big is the market, and where is it growing?** Market size, growth and industry shares, each with its source.
2. **Which companies need digital adoption help now, and why?** US companies with public, dated signals such as SAP S/4HANA migrations, AI rollouts to employees, mergers, new tech leaders and visible adoption pain.
3. **Who matters, and how could we reach them?** Executives named in public sources, plus warm-intro routes through partners, industry events and alumni networks.
4. **What should the business do next?** A one-screen Founder's Brief with recommended actions (illustrative) and KPIs to track.

Open `index.html` in any modern browser. There is no build step, no server and no tracking.

## Why I built this

I wanted to understand the DAP market: how enterprises decide to buy adoption tools, what pushes them to act now, and how a DAP business could reach the right people. Building a working tool on real, sourced data made me check every claim instead of assuming it.

This is an independent student project. It is not affiliated with, or endorsed by, any company named in it.

## What's inside

| Section | What it shows |
|---|---|
| **Founder's Brief** | Market snapshot, top 3 sectors, top 5 opportunities with "why now", 5 recommended actions (illustrative) and KPIs (signals per sector, opportunities by stage) |
| **Opportunity Board** | 21 US companies on a map and in a ranked list: signal type, signal strength, timing, sources, stakeholders, where a DAP could help, and a transparent score breakdown |
| **SAP S/4HANA Watch** | Countdown to 31 Dec 2027, the support timeline to 2033, sourced market stats, a migration tracker by stage (stage is my estimate) and a 14-item news feed |
| **Market** | Fortune Business Insights anchor ($1.59B global in 2026, $377M US, $4.37B by 2034, 13.5% CAGR), comparison with five other publishers, industry shares across sources, and a neutral market landscape (WalkMe/SAP, Whatfix, Pendo, Apty, with Everest Group's 2024 assessment of 25 DAP vendors) |
| **Stakeholders & Network** | 23 executives named in public news or press releases, each with a source link; warm-intro paths (company → relevant role → possible route); 6 network contacts shown by role only; a watchlist of 5 companies with no named stakeholder yet |
| **AI reader (beta)** | Paste an article and it tags digital-adoption signals and scores the company. It uses built-in AI when the host provides it, otherwise keyword rules. Results last for the session only |
| **About** | Why I built this, what's real vs simulated, how the score works, how it was built, and the roadmap |

## Data sources

Every signal, number and executive links to its source, with a short trust note: primary source, trade press, vendor case study, and so on. The main groups are:

- **Company signals:** company newsrooms and investor relations, PR Newswire, Business Wire, Banking Dive, American Banker, Insurance Business, CIO.com, CIO Dive, The Register, ERP Today, SAPinsider, Becker's Payer Issues and Microsoft customer stories.
- **Market size:** Fortune Business Insights (anchor), Research and Markets, Market Research Future, Market.us, 6Wresearch and Dataintelo. The estimates differ widely, so the page shows the range, not just one number.
- **S/4HANA context:** SAPinsider (support dates and survey), Gartner via The Register, and CIO.com.
- **Market landscape:** SAP's press release on WalkMe (via Nasdaq/GlobeNewswire), Entrackr, CX Today, Apty's own site and Everest Group.

The data snapshot is dated **15 Nov 2026**. Scores are computed as of that date so they don't drift.

## What's real and what's simulated

| Item | Status |
|---|---|
| Companies, signals, executives, dates | **Real.** Taken from public sources I opened and checked |
| Market size and industry shares | **Real.** Published estimates, linked, shown as a range |
| S/4HANA migration stage | **Estimate.** Stage is my estimate from public announcements |
| Scores and strength labels | **Model.** My own weights, not yet validated against outcomes |
| Recommended actions | **Illustrative.** My reading of the signals |
| Warm-intro routes | **Ideas.** Partner names come from the sources; these are not existing relationships |
| "Refresh signals" button | **Simulated.** No live feeds are connected; nothing is fetched |
| AI reader | **Beta.** Built-in AI only where the host provides it; otherwise keyword rules |

## How the score works

Score (0–100) = **fit** (up to 20: US HQ, high-DAP-spend sector, known size) + **triggers** (up to 50: migration, AI rollout, merger, new leader) + **pain** (up to 30: ERP problems, adoption gaps, go-live within six months, hiring and more).

- Signals older than six months count 0.6×; signals older than a year count 0.3×. Indirect evidence is discounted.
- **Strong** means a score of 65+, or a trigger plus pain at 50+. **Moderate** means 40+. Anything lower is **Early**.

## How it was built

- **AI-assisted research, human verification.** AI helped find candidate articles. I then opened and checked every source before it went in. Anything I couldn't verify went to a watchlist or was dropped.
- **Privacy.** Executives appear only when named in public news or press releases, with the source link. Personal and alumni connections are shown by role only: no names, profile links or photos.
- **One self-contained file.** Plain HTML, CSS and JavaScript, with no external libraries and no API keys in the code.

## Roadmap

| Stage | What happens |
|---|---|
| **Today** | Articles are verified and added by hand. The AI reader analyses pasted articles. Refresh is simulated. |
| **Next** | AI scans news on a schedule and updates signals automatically, with a person approving new sources. |
| **Later** | CRM integration, and validation of scores and recommendations with real companies, if it proves useful. |

## Repository contents

```
index.html    the prototype (single self-contained file)
README.md     this file
.gitignore    keeps the private copy out of the repository
```

---

© 2026 Sriram Sudarsi. Company names and trademarks belong to their owners and are used only to describe public information.
