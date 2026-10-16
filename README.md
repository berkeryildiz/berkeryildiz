# Berker Yıldız

**Product developer · games, automation and data tools**

I take ideas from a blank page to a working product: game rules and balance, data pipelines, interfaces, AI-driven automation and deployment even social media. I work mainly in TypeScript, JavaScript and Node.js.

(https://www.linkedin.com/in/berkeryildiz/) · berkeryildiz99@gmail.com · İstanbul, Turkey

---

## Featured

### Kutubil · daily film trivia grid · [Play live](https://oyna.kutubil.workers.dev)

A 3×3 grid for film fans: find the actor who fits both the row and the column category. New grid every day, six catalogues (global, Turkish film and TV, Korean and more).

![Kutubil](assets/kutubil.png)

- **Stack:** TypeScript, React 19, Vite, Cloudflare Workers, D1, Durable Objects
- **Data:** Wikidata and TMDB pipeline → normalized catalogue → generated daily grids with answer-rarity scoring
- **Features:** online head-to-head rooms, streamer mode, guided first game, editor tools for answer disputes
- **Ops:** guarded one-command deploy, unit and API tests

### Firing XI · fantasy transfer league *(in development · private, code on request)*

Managers build squads and play each other in a league; the rules decide whether a season is fair.

![Firing XI](assets/firing-xi.png)

- **Rules first:** every rule change is tested in a deterministic simulation (seeded worlds, frozen result snapshots) before it reaches the game
- **Quality:** 500+ automated tests; headless-browser audits for layout overflow and console errors at phone and desktop sizes
- **Interface:** mobile-first 9:16 layout, dark and light themes, drag-and-drop line-ups
- **Stack:** Node.js, plain JavaScript and CSS, no runtime dependencies

---

## More work

### Automation and AI agents

| Project | What it does | Built with |
|---|---|---|
| **Social media content agent** *(football game brand)* | Learns a brand's voice from sample posts and produces a fresh, varied set of image prompts on every run, planned across content pillars and a weekly calendar. Automated checks enforce the brand rules; a dashboard tracks what was produced. | Node.js, Claude Code (headless) |
| **Football news content engine** | Turns a headline into a researched, source-checked Instagram carousel, captions for Instagram and X, and a video prompt. All text is rendered as real typography (HTML → PNG), so Turkish characters never break. Live RSS suggestions; learns from posts the editor liked. | TypeScript, Fastify, Playwright, Anthropic API |
| **Daily AI news digest** | Collects updates once a day, summarizes them in Turkish and adds a magazine-style slide to a Google Slides deck with a linked table of contents. | Node.js, Google Slides API, Claude Code |
| **Content concept studio** | Several social content concepts on one system: shared legal guardrails, prompt assembly and a click-to-run dashboard. | Node.js |

### Data and tracking tools

| Project | What it does | Built with |
|---|---|---|
| **Match highlight simulation** | Converts professional player-tracking data into an animated 2D highlight replay and a structured clip list for analysts. | JavaScript, Pixi.js, ExcelJS |
| **Live match tracker** | Real-time scores from a public sports feed, personal watch lists stored locally, charts, and a circuit breaker that keeps the app usable when the feed fails. | Next.js, TypeScript, Tailwind, Zod, Recharts |

### Games and web

| Project | What it does | Built with |
|---|---|---|
| **Football management game** *(studio work)* | Contributed to the playable prototype and the marketing landing page. | React, Vite, Playwright · Next.js, Vercel |
| **Tek Taht** *(strategy game prototype)* | Village-building strategy game with three empires: design documents (economy, combat, UX), 47 SVG sprites and a single-file playable prototype. | HTML, JavaScript, SVG |
| **Car-rental website** *(freelance, in progress)* | Fast static site with no third-party dependencies, automated brand guard and rebrand drill, tests. | Node.js |
| **Generative visual studio** | Single-file canvas tool for psychedelic POV reels; records clips straight from the browser. | HTML Canvas |

---

## How I work

- **Decisions first.** Each project keeps a short decision record (decided, proposed, open) before code is written.
- **Measure, don't guess.** Simulations, automated tests and headless-browser audits back every claim.
- **Review gates.** Nothing is published or merged without an explicit approval step.
- **AI pair programming.** I build with Claude Code. I own the product decisions and the design, and I verify the results.
