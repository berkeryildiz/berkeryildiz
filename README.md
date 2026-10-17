# Hi, I'm Berker

I work in product and growth, and I build the products myself: live sports data dashboards, browser games, and the content tools that keep a brand's channels running. I like taking an idea from a blank page to something people use every day, and I care about the parts that don't show on a screenshot: data quality, fair rules, and numbers I can defend.

I build mostly in TypeScript and Node.js, with React and Next.js on the front end. I pair with Claude Code daily: I set the direction and the design, and I check every result before it ships.

Open to product, growth and product-minded engineering roles in gaming, sports and tech.

<a href="https://www.linkedin.com/in/berkeryildiz"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge" alt="LinkedIn"></a>
<a href="mailto:berkeryildiz99@gmail.com"><img src="https://img.shields.io/badge/Email-30363d?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
<img src="https://img.shields.io/badge/%C4%B0stanbul%2C_T%C3%BCrkiye-30363d?style=for-the-badge" alt="İstanbul, Türkiye">

---

## Macko: live football dashboard with match analysis

![Macko](assets/macko.png)

A dashboard I use every day to follow 100+ matches a day across European leagues, the Champions League, the NBA and more, with live scores, a nine-day calendar and goal notifications.

Each match has an analysis panel that pulls together who is scoring, the last five results, missing players and the weather at kick-off, each figure with its source noted, and "no data" shown instead of a guess. On top of that sits a probability model (Poisson goals, result first, then the most likely score in that result) with small, capped adjustments for form, injuries and weather. I measured it on 290 finished matches: correct results went from 50.7% to 55.2%, and calls marked high-confidence were right 72% of the time.

It stays usable when the data feed misbehaves: a shared request budget, a circuit breaker and a disk cache keep it running instead of going blank.

`Next.js 14` `TypeScript` `Tailwind` `Zod` `Recharts` `Open-Meteo` `Wikidata`

## Kutubil: daily film trivia grid ([play it](https://oyna.kutubil.workers.dev))

![Kutubil](assets/kutubil.png)

**Built and shipped in under 24 hours:** first commit on a Saturday evening, live on Cloudflare the next afternoon with the data pipeline and online rooms working; automated backups and a guarded deploy followed the same evening.

A daily 3×3 grid for film fans: name an actor who fits both the row and the column. Film data comes from Wikidata and TMDB, gets cleaned into six catalogues (global, Turkish film and TV, Korean, Gen-Z and a mix), and a generator builds a new grid every night. You can also challenge a friend in a live room.

`React 19` `Vite` `TypeScript` `Cloudflare Workers` `D1` `Durable Objects`

## Firing XI: fantasy transfer league (in progress)

![Firing XI](assets/firing-xi.png)

Managers build squads and play each other in a weekly league. I wrote the simulator before the game, because the hard part isn't the screens, it's making sure the rules give every manager a fair season. Every rule change runs through hundreds of simulated seasons and 500+ tests before it reaches the game. Mobile-first, with a pitch view, kit-style player cards and drag-and-drop line-ups. The repo is private for now; happy to walk anyone through it.

`Node.js` `JavaScript` `CSS` `Headless browser testing`

---

## Content systems and brand design

Most social content breaks down the same way: every post is designed from scratch, so the look drifts and the text gets mangled by image models. I build systems that fix both.

- **Brand systems in Claude Design.** For Firing XI I designed the whole identity on a Claude Design canvas: logo, colour and type tokens, and ready-made templates for posts, stories and thumbnails. All of them read from one tokens file, so a new post comes out on-brand without being redesigned, and the game's interface uses the same file.
- **Social content agent** for a football game's accounts. It learns the brand's voice from past posts, plans a week of varied ideas across content pillars, and writes a ready-to-use image prompt for each, with automated checks against the brand rules.
- **Football news content engine.** Headline in, fact-checked Instagram carousel plus captions for Instagram and X out. Slides are rendered from HTML templates, so Turkish characters always come out right.
- **Post studio.** A single-file, offline tool: pick a size and a template, write the text, download the PNG and copy matching image and motion prompts.
- **Daily AI news digest.** Collects Claude and Anthropic news every morning, summarizes it in Turkish and adds a new page to a Google Slides "magazine" with a linked table of contents.

## Also built

- **Match highlight simulation:** turns raw player-tracking data into an animated 2D highlight reel, plus a clip list analysts can filter in Excel.
- **Tek Taht:** a strategy game prototype with design documents, 47 SVG sprites and a playable single-file build.
- **Studio work** on a football management game: parts of the playable prototype (React, Vite, Playwright) and the landing page (Next.js).
- A car-rental website for a client, and a small generative-visuals tool for Reels.
