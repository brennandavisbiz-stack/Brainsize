# BrainSize — Static Pages

Flat HTML mockups for the BrainSize site. Each file is fully self-contained (inline CSS + JS, Google Fonts via CDN). No build step required.

## Pages & routes

| File | Route | Purpose |
|------|-------|---------|
| `index.html` | `/` | Homepage |
| `instructions.html` | `/instructions` | Pre-test rules / start screen (the "Start Test" CTA target) |
| `profiles.html` | `/profiles` | IQ Profiles — the eight cognitive profiles |
| `pricing.html` | `/pricing` | Pricing (free / $3.99 report / BrainSize+) |
| `plus.html` | `/plus` | BrainSize+ subscription |
| `compare.html` | `/compare` | BrainSize vs. clinical vs. typical online |
| `methodology.html` | `/methodology` | How the test works (CAT + IRT + 5 domains) |
| `about.html` | `/about` | About / mission |
| `faq.html` | `/faq` | Full FAQ |
| `privacy.html` | `/privacy` | Privacy policy (template) |
| `terms.html` | `/terms` | Terms of service (template) |
| `refunds.html` | `/refunds` | Refund policy (template) |

## Routing
`vercel.json` sets `cleanUrls: true`, so links like `/pricing` resolve to `pricing.html` automatically. Internal links already use clean paths (no `.html`).

## Deploy
1. Push this folder to a GitHub repo.
2. Import the repo in Vercel (Framework Preset: **Other** — it's static, no build command).
3. Done. Vercel serves the files directly.

## Before launch — replace placeholders
- **Stats / logos / testimonials / leaderboard** on the homepage are placeholder data (flagged with `DEV NOTE` comments). Swap for real, verifiable figures.
- **BrainSize+ price** ($7.99/mo, $59.99/yr) is a placeholder; the $3.99 report price is confirmed.
- **Legal pages** are templates — have a lawyer review and fill `[DATE]` / `[JURISDICTION]`. Update `support@` / `privacy@brainsize.com` to real addresses.
- **The test itself** (`/test`) and the **results/paywall** screen are not in this set yet.

## Design tokens (for the dev)
- Primary: `#5B3DF5` (indigo-violet) · hover `#4A2FD9`
- Tints: `#ECE8FE`, `#F5F3FF` · Ink: `#111114` / `#5A5A66` / `#9A9AA6`
- Surface alt: `#F7F7F9` · Border: `#ECECF1`
- Font: Plus Jakarta Sans (500/600/700/800)
- Card radius 24px, pill buttons, soft shadows
