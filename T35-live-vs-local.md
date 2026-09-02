# T35 — Water Boys v2 live-vs-local verification (2026-08-18)

**Finding (verified 2026-08-18 03:05):** local repo `Desktop/water-boys` is **ahead of origin/main by 1 commit** (b80ca4a) — the T22 conversion-audit patches are committed locally but **NOT live**.

## Evidence
- Local `index.html` T22-feature markers: **12** (og:meta, LocalBusiness JSON-LD, #how, #faq, callbar, nav links — all present)
- Live `beefalo1234.github.io/water-boys/` (HTTP 200, 7769 bytes): T22-feature markers: **0**
- `git status`: `## main...origin/main [ahead 1]` → b80ca4a unpushed

## What's missing on live (the whole T22 batch)
1. OG/social meta tags
2. LocalBusiness JSON-LD schema
3. How-it-works section (#how)
4. FAQ section (#faq, 4 honest Qs)
5. Sticky mobile call bar (.callbar)
6. Nav links to the new sections

## Why it's not pushed (guardrail compliance)
- T22 ran as [build] with an explicit "NO push — live-site edit needs [apply]/Gray ok (1 command away)" note (mission.md T22 row, 2026-08-17).
- The 08-15 auto-push rule covers **Gray-requested** site builds ("if I tell you to make or adjust a site... just auto push"). T22 was a runner-initiated audit, not a Gray request → push stays blocked on [apply].
- The runner does NOT push unprompted per nightshift guardrails (live-site edits need [apply]).

## Patch/push list (when Gray says apply — 1 command + verify)
```
cd C:/Users/Gray/Desktop/water-boys
git push origin main
curl -sL https://beefalo1234.github.io/water-boys/ | grep -c 'LocalBusiness\|callbar\|id="faq"'   # expect >= 3
```
Expected after push: live markers 0 → ≥3, byte size grows past 7769. Also re-verify pay.html (200) per the 08-17 verify-live rule.

**Status: BLOCKED-needs-Gray ([apply]) — everything is staged and one push away.**
