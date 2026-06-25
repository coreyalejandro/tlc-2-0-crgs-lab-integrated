# TLC 2.0 × CRGS Lab — Integrated Site Build Plan

**Version:** 1.0
**Created:** 2026-06-22
**Status:** PHASE 1 COMPLETE — Phase 2 remaining
**Repo:** /Users/coreyalejandro/Projects/tlc-2-0-crgs-lab-integrated
**Agent handoff:** Read this file + AGENT_HANDOFF.md to continue

---

## Canonical Intent Statement (LOCKED)

> The project's objective is to develop a **constitutional AI-governed, blockchain-runtime-verified** research and development tool that will empower users across various resource categories — Fortune 500 enterprise corporations, academic research institutions, standard enterprise corporations, Tier-1 academic research institutions, small businesses and startups, and hobbyist developers — to produce Tier-1 research, resulting in Tier-1 research papers and, ultimately, a **Tier-1 research-based consumer-facing product**.
>
> The project is designed to be accessible regardless of financial resources, allowing development with any amount from **$100 to $1 billion**.

**Ratified:** 2026-06-22 · Source: CANONICAL_INTENT.md

---

## Non-Negotiable Identity (LOCKED)

**Corey Alejandro** is an expert **Hybrid AI Constitutional Runtime Governance Systems Research Scientist AND Research Engineer** who engages in a one-of-a-kind, state-of-the-art R&D development practice using **The Living Constitution 2.0** — a groundbreaking **constitutional AI-governed, blockchain-runtime-verified** research and development tool developed by Corey Alejandro.

---

## Source Repositories

| Source | Local Path | GitHub |
|---|---|---|
| Portfolio (PRESERVED — do not modify) | /Users/coreyalejandro/Projects/the-living-constitution-2.0-portfolio | https://github.com/coreyalejandro/the-living-constitution-2.0-portfolio |
| CRGS Lab Kit | /Users/coreyalejandro/Projects/crgs-lab-website-kit | Local only |
| TLC 2.0 Runtime | /Users/coreyalejandro/Projects/the-living-constitution-2.0 | https://github.com/coreyalejandro/the-living-constitution-2.0 |
| This integrated repo | /Users/coreyalejandro/Projects/tlc-2-0-crgs-lab-integrated | TBD — push to GitHub |
| CALS Template v6.1 | ~/Library/CloudStorage/GoogleDrive-.../Downloads/Constitutional_Adaptive_Learning_Systems_Research_Template__v6.1_...md | Google Drive |

---

## Phase 1 — Core Pages (8 pages + assets)

| Page | File | Status |
|---|---|---|
| Homepage | index.html | ✅ BUILT |
| Tool | tool.html | ✅ BUILT |
| Six Tiers | tiers.html | ✅ BUILT |
| Pipeline | pipeline.html | ✅ BUILT |
| Template | template.html | ✅ BUILT |
| Registry | registry.html | ✅ BUILT |
| Identity | identity.html | ✅ BUILT |
| CRGS Lab | programs/crgs.html | ✅ BUILT |
| Assets (CSS + JS + logos + PORTFOLIO_DATA.json) | assets/ | ✅ BUILT |

## Phase 2 — Remaining Work

| Task | Status | Notes |
|---|---|---|
| Fix asset paths in index.html (golden-folio references) | ⬜ TODO | index.html has golden-folio.css and golden-folio.js refs — need to verify paths work |
| Fix relative paths in programs/crgs.html | ⬜ TODO | Uses ../assets/ — verify correct |
| Add .gitignore | ⬜ TODO | Exclude .wrangler/, node_modules/, .DS_Store |
| Create GitHub repo | ⬜ TODO | gh repo create coreyalejandro/tlc-2-0-crgs-lab-integrated --public |
| Push to GitHub | ⬜ TODO | git remote add origin + git push |
| Configure Cloudflare Pages | ⬜ TODO | npx wrangler pages deploy . --project-name tlc-2-0-crgs-lab-integrated |
| Restore portfolio to clean state | ⬜ TODO | Revert index.html + site.css in portfolio to pre-stash state; keep CANONICAL_INTENT.md |
| Verify all 8 pages load at localhost:8000 | ⬜ TODO | python3 -m http.server 8000 |
| Update STATUS.md in portfolio repo | ⬜ TODO | Record integrated repo creation |

## Phase 3 — Enhancements (future)

| Task | Notes |
|---|---|
| Port remaining 39 pages from portfolio | about, paper, detector, folio/001, research/*, security/*, governance/*, programs/*, runtime/* |
| CRGS animated logo in topbar | Replace text brand with crgs-logo-animated.svg |
| Live Registry auto-refresh | Webhook or cron to pull latest PORTFOLIO_DATA.json from TLC 2.0 runtime repo |
| Kernel commands for new pages | Add tool, tiers, pipeline, template, registry to kernel.js COMMANDS |
| HUD page weights for new pages | Add tool.html, tiers.html, pipeline.html, template.html to PAGE_WEIGHTS in hud.js |
| Blockchain governance diagram | SVG diagram showing governance ledger scaling from Git → file-hash → permissioned → public |
| CALS v6.1 section nav | Sticky sidebar navigation for template.html sections |

---

## Technology Stack

- Pure HTML + CSS + JS — no framework, no bundler, no npm
- EB Garamond + Inter + JetBrains Mono (Google Fonts)
- Cloudflare Pages (free) or GitHub Pages (free)
- No build step — `python3 -m http.server 8000` for local preview

---

## Key Architecture Decisions (locked)

1. Blockchain governance at Tier 6 — planned, EU AI Act / NIST / ISO justified
2. Quantum compute at Tier 6 — planned
3. Physical sensor networks at Tier 5–6 — planned
4. "Autonomous AI Scientist" — destination framing for what the tool produces, NOT Corey's identity
5. "Verifiable confidence" — first-class concept; stronger than "100% accuracy"
6. Portfolio is PRESERVED at its own GitHub repo — this is a new site
7. FOLIO 001 preserved below the fold on index.html
8. truth_status governs what is shown at each tier (working / partial / planned)

---

## Agent Pickup Instructions

1. Read this file completely
2. Read CANONICAL_INTENT.md
3. Read AGENT_HANDOFF.md
4. Run `python3 -m http.server 8000` in this directory to verify pages load
5. Check Phase 2 checklist — start at first unchecked item
6. DO NOT modify the-living-constitution-2.0-portfolio except STATUS.md
7. Commit after every completed task: `git add . && git commit -m "task: description"`
8. Deploy when Phase 2 complete: `npx wrangler pages deploy .`
