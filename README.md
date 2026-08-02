# Chris James

Self-taught full-stack engineer. I build and ship production software solo, with Claude Code as my primary development mode — not an assistant to my workflow, but the workflow.

Mobile (Flutter), web (TypeScript / SvelteKit / Cloudflare Workers), Python, SQL. I own the whole line: backend, frontend, deploy, monitoring, and the iteration after.

**[chrisjk.com](https://chrisjk.com)** — every app and link in one place · **[cannappy.org](https://cannappy.org)** — the studio these ship under

---

## What I shipped in the last 90 days

Roughly 60 projects touched. The parts that matter:

**Two apps live on the App Store, shipping continuously**
- [Strain Guide](https://apps.apple.com/us/app/id1596314933) — 7 store versions in 90 days (4.9.0 → 4.12.0)
- [Grow Guide](https://apps.apple.com/us/app/id6637720578) — 6 store versions (2.2.0 → 2.4.0)
- **31 over-the-air patches** pushed straight to users on top of those releases, via Shorebird. Fixes reach users the same day they're written.
- Both apps run PostHog observability, remote-config kill switches, and an in-app feedback pipeline that closes the loop back to the user who reported the bug.

**Built a house ad network in four days**
Both apps and both websites were monetized through a third-party ad vendor. I replaced it with my own: a Cloudflare Workers ad server, a Flutter client package, and an ops dashboard.

- First commit 2026-07-10. Live across all four properties by 2026-07-14.
- Per-property and per-build delivery controls, so I can dark a bad creative on one app version without a release.
- An A/B bench that switches the whole ad stack in place to compare against the vendor it replaced.
- Contextual serving: ads on a strain page now match the strain being read.
- Revenue digest that reports what to act on, not just CTR.

**[signalbot](https://github.com/chris-jk/signalbot) — live, open source** → https://signalbot.cannappy.org
SEC Form 4 and Congressional trading disclosures, ingested, normalized, and backtested. Includes an **MCP connector** that exposes the whole dataset as Claude-callable tools. Empty repo to shipped in seven days.

**[freeply](https://github.com/chris-jk/freeply) — live, open source**
Agentic customer messaging: a keyword in an Instagram comment triggers an automated DM with the link. Self-hostable on Cloudflare's free tier, with the Meta Graph API edge cases already solved.

**~40 Cloudflare Workers in production**, including an API gateway, an email operations pipeline, SMS/voice outreach services, and a secrets gateway designed so no API key ever enters an LLM context.

**Six MCP servers, built from scratch**
`cloudflare-deploy` (ship any project to a live URL from a prompt) · `app-store` (App Store Connect + RevenueCat: bundle IDs, IAP, subscriptions) · `admob` · `play-store` · `reel-transcriber` (hosted) · signalbot's disclosure connector.

**Eight custom Claude Code skills**, because the workflow is the product
`outliers` (finds the videos overperforming a channel's own baseline) · `reel-teardown` (fact-checks a short-form video claim by claim) · `blog-post` (keyword discovery → written → published → sitemap → IndexNow) · `apk-audit` (unpack, decompile, map the backend) · `screenshot-studio` (App Store screenshots designed and exported at every Apple size) · plus mail, DNS, and outreach skills.

Five scheduled automations run unattended on top of that — a cloud-cost watchdog, an ads health check, and an analytics pull among them.

**Client work, same velocity** — a powersports dealer: live catalog, Shopify drop-ship pipeline with order scopes, and a full SEO foundation, in ten sessions.

---

## Try things

| | |
|---|---|
| [chrisjk.com](https://chrisjk.com) | Everything I've shipped, in one place |
| [signalbot.cannappy.org](https://signalbot.cannappy.org) | Insider + Congress trading signals, with an MCP connector |
| [Strain Guide](https://apps.apple.com/us/app/id1596314933) · [Grow Guide](https://apps.apple.com/us/app/id6637720578) | iOS + Android, live, actively shipping |
| [freeply](https://github.com/chris-jk/freeply) | Instagram comment → DM automation, self-hostable |
| [Its My Birthday](https://apps.apple.com/us/app/id6475056772) | Rebuilt 1.x → 2.0 in eight days |

## Selected open source

- **[signalbot](https://github.com/chris-jk/signalbot)** — disclosure data pipeline + MCP connector
- **[freeply](https://github.com/chris-jk/freeply)** — agentic Instagram comment-to-DM on Cloudflare
- **[claude-bs-detector](https://github.com/chris-jk/claude-bs-detector)** — fact-checks short-form video claim by claim
- **[claude-outliers](https://github.com/chris-jk/claude-outliers)** — finds videos overperforming a channel's own baseline
- **[focus-app-mac](https://github.com/chris-jk/focus-app-mac)** — menu bar Pomodoro + day planner
- **[desktop-switch](https://github.com/chris-jk/desktop-switch)** — macOS menu bar desktop-icon toggle
- **[SpeakHUD](https://github.com/chris-jk/SpeakHUD)** — text-to-speech HUD with word highlighting

Much of the work above lives in private repos — the App Store and live URLs are the public proof. Happy to walk through any of it.
