# Landing-page upgrade drafts — from landerlab mimic row (2026-08-18)

Source pattern (mimic.md 2026-08-18): landerlab.io "18 Best Landing Page Examples of 2026 (With AI Prompts to Build Each One)" — pay-per-call anatomy ("one job: get the phone to ring"), objection-killer lead (remove the biggest objection upfront: price/eligibility/"already have a guy"), quiz/assessment that FEELS like help, not a funnel.

**STATUS: DRAFTS ONLY — nothing here is applied. Live edits need [apply]/Gray per guardrails.**
Files affected when applied: `Desktop/water-boys/index.html`, `Desktop/LeadSetter-AI-site/index.html`.

---

## A. Water Boys (`Desktop/water-boys/index.html`)

Current hero (verified on disk 2026-08-18):
- H1: "Driveway looking rough? We'll power-wash it for less than you think."
- CTA: "Call or Text — Free Quote Today — 513-581-1419" (tel: link)
- Sub: "Free quote · Great prices · Satisfaction guarantee"

### A1. Objection-killer headline variants (steal: "removes the biggest objection upfront")
The #1 objection for pressure washing = price fear ("it'll cost a fortune"). Current H1 says "less than you think" — good, but the price range lives 2 sections down. Kill the objection IN the headline:

- V1: "Dirty driveway? We'll power-wash it for **$100–$200** — and you'll know the price before we start."
- V2: "No surprise bills. **Free quote in 60 seconds** — most driveways land around $150."
- V3: "Your driveway, clean in one visit — **$100–$200, no contracts, no surprises.**"

Recommendation: V1 (specific number beats "less than you think" — specificity = trust; matches the honest-copy rule).

### A2. Pay-per-call CTA block (steal: "get the phone to ring" = only logical next step)
Current CTA is a single button. Upgrade to a 3-line "only logical next step" block above the fold:
1. Phone number as the HERO element (largest text on page, tap-to-call on mobile).
2. A one-line urgency/qualifier under it: "Text us a photo of the driveway — we'll quote it without a visit."
3. A tiny "what happens next" strip: "1) Call/text → 2) Photo or quick chat → 3) We show up & clean. ~$150 most driveways."

This makes calling the ONLY next step and pre-answers "what will they ask me / how much".

### A3. Quiz/assessment lead-capture sketch (steal: "feels like help, not a funnel")
Draft (NOT built — needs a JS handler + storage):
- Title: "2-minute driveway check — get your honest price range"
- Q1: What needs cleaning? [Driveway / Patio / Walkway / House siding / Other]
- Q2: Roughly how big? [Small (1 car) / Medium (2 car) / Large (3+ car) / Not sure]
- Q3: When were you hoping to get it done? [This week / This month / Just shopping]
- Result: "Based on that, most homes like yours land in the **$X–$Y** range. Want the exact price? Call/text 513-581-1419 — 60 seconds, free."
- Capture: name + phone + zip at the result gate (opt-in, honest: "we'll text your price and nothing else").
- Why: qualifies before it converts (landerlab pattern #1), and a $150-range quote before contact = objection pre-killed.

### A4. What NOT to change (honest-copy guardrails)
- Keep the real price ranges ($100–$200 driveway, $199/$399 tiers, "most quotes land around $150") — no inflated ranges.
- Keep "No hype, no contracts" voice — that IS the objection-killer; don't replace it with hype.
- Keep tel: links + callbar (already pay-per-call-first).

---

## B. LeadSetter AI (`Desktop/LeadSetter-AI-site/index.html`)

Current structure (verified 2026-08-18): H2s "Right now, you're paying to lose." / "Three steps. Five days. Done." / "You can't lose on this deal."

### B1. Objection-killer for the AI-agency angle (steal: "sells eligibility/outcome, not the service")
LeadSetter's biggest objection = "AI agencies are scams / how is this different?" Kill it upfront:
- H1 draft: "Your missed calls are costing you jobs. **We answer in 5 seconds, 24/7, for less than a part-time hire.**"
- Sub draft: "Real receptionist, real bookings, real lead capture — powered by AI, priced like software. See the exact numbers before you pay a dime."
- Proof strip (from theaiforest honest-numbers pattern): one hard stat beats vibes — e.g. "AI freelance work grew +60% YoY; businesses that answer first win the job" (placeholder until real local stat exists — honest: label as market stat, not our client stat).

### B2. "Can't lose" guarantee block (objection-removal, not risk-transfer)
Current "You can't lose on this deal" — strengthen with a specific, honest guarantee:
- Draft: "Try it on 3 real calls. If it doesn't book you a job, you owe nothing." (only if Gray can actually honor this — flag for Gray decision; do NOT publish without his OK, it's a money-back promise = spend-adjacent).

### B3. Lead-capture assessment sketch (same pattern as A3, agency flavor)
- Title: "Is your phone costing you jobs? 60-second check"
- Q1: How many calls do you miss a week? [0-2 / 3-5 / 6+ / Don't know]
- Q2: What happens when you're on a job? [Goes to voicemail / Family answers / Nobody]
- Q3: What's one job worth to you? [$100-300 / $300-500 / $500+ / Priceless]
- Result: "At 3+ missed calls/week and $300/job, you're losing **~$900+/mo** to voicemail. We can fix that for less than one job." → capture name/phone → "want the exact math? Call/text."
- Why: the loss-framing makes the ROI math the objection-killer.

---

## C. Application plan (when approved)
1. Water Boys: A1-V1 headline + A2 CTA block (pure HTML/CSS patch, ~30 min, auto-push per 08-15 rule once Gray says apply or a task says [apply]).
2. LeadSetter: B1 H1 + B2 flag to Gray (money-back promise = his call) — B2 never publishes without explicit approval.
3. A3/B3 quizzes: need js/quiz.js + storage — flag as a separate [build] task (T27-continue) if Gray wants them; do NOT build silently, they're new surfaces.
4. All drafts verified against honest-copy rules (corrections.md 08-15 export rule + followup-templates voice).

— Drafted 2026-08-18 02:2x by nightshift-runner. NOT applied. Next: Gray picks V1-V3, says apply, runner patches + auto-pushes (Water Boys) and patches LeadSetter after his B2 call.
