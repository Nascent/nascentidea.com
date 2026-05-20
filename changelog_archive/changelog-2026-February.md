# Podcast Changelog Archive -- February 2026

Archived from changelog.md on May 20, 2026.

---

## [~10:30 PM] PT Wed Feb 12th 2026

### FAQ 2.2 — Lean Startup blockquote + failure stats + copy tightening

**Challenge:** Flesh out FAQ 2.2 with Eric Ries quote as a styled blockquote, cite startup failure statistics (Failory, CB Insights), and argue that "startup success can be learned" is insidious.

**What was done:**

- Added `<blockquote class="faq-blockquote">` with Ries quote from theleanstartup.com/principles (2011)
- Added `.faq-blockquote` CSS — thick gray left border, italic text, no background (matches classic blockquote style)
- Added failure stats paragraph: 90% fail (Failory), most common reason is never discovering customers (CB Insights, 111 post-mortems, 2021)
- Mike rewrote "In short:" paragraph — tightened, ends with "conventional strategies sometimes even harm founders:" to set up blockquote
- Mike added "startup success CANNOT be engineered" counterpoint
- Mike added "This reinforces the feeling that a startup failure is a personal failure" sentence
- Mike rewrote "The details:" paragraph — "developing a product that nobody wanted"
- Mike rewrote Nomenclature bullet — simplified, added "look for the earliest possible signal of a customer"
- Mike rewrote Actionable deliverables bullet — added Steve Blank 2025 link, specific Nascent deliverables (QPG + ERNY)
- Fixed typos: "takess" → "takes", "project" → "projects", double space

**CB Insights data note:** The 2021 report (111 post-mortems) shows "no market need" at 35% (#2), not the older 42% (#1) figure that circulates widely. #1 is "ran out of cash" at 38%. Site copy uses "most common reason" framing which is defensible via Failory (56% marketing/PMF problems).

**Commits:**

- `a41362b` — Add Lean Startup blockquote + failure stats to FAQ 2.2
- `b3608c4` — Restyle FAQ blockquote to match thick-border reference
- `c183d53` — Tighten FAQ 2.2 copy + fix typos

**Key files:** `index.html` (lines 302-319), `style.css` (lines 565-585)

---


## [~evening] PT Wed Feb 12th 2026

### Intro bold emphasis shift

**What was done:**

- Removed bold from "repeatable methodology" inside the FAQ anchor link
- Reworded closing clause: "recognize when it's bad" → "**recognize and avoid bad ideas**"
- Net effect: bold emphasis moved from methodology descriptor to the action/value prop

**Commit:** `f46c50e` — Shift bold emphasis from methodology to value prop in intro

---


## [~2-4pm] PT Wed Feb 12th 2026

### Deutsch/Popper copy additions + ERNY vs TAM FAQ

**Challenge:** Add intellectual foundations (Deutsch, Popper, Kahneman, Tversky, Krippendorff) to nascentidea.com per spec from Claude web app collab session.

**What was done:**

- Hero intro: added falsification sentence, Mike rewrote to "You can't prove a startup idea is good — but you can quickly recognize when it's bad"
- Body: added error-elimination paragraph (replaced "Instead of promising PMF, Nascent promises clarity"). Mike condensed from h3+2 paragraphs to single paragraph, relocated People in Pain/ERNY content to FAQ 2.3
- FAQ 2.1: expanded intellectual foundations (Deutsch, Popper, Kahneman, Tversky, Krippendorff). Mike rewrote summary and restructured first answer
- FAQ 2.2: revised Data analysis bullet with error-elimination framing
- FAQ 2.3: Mike added new intro paragraph tying deliverables to People in Pain and ERNY
- New FAQ 2.4: ERNY vs TAM/SAM/SOM (Mike expanded acronyms, improved traceability sentence)
- Renumbered FAQs 2.4→2.5 through 2.11→2.12
- Added `id="faq-2-3"` anchor to deliverables FAQ
- TM cleanup: removed 3 extra ™ symbols per definition-point-only policy (`clients/memo-tm-symbols.md`)
- Fixed self-referencing #faq-2-3 anchor in FAQ 2.3 intro
- Fixed missing articles ("the most common reason", "a lack of")
- Cleaned trailing whitespace
- Split People in Pain intro paragraph, added bridge about founders focusing on ideas where PMF is possible
- Downshifted singular "person in pain" (no TM — singular/plural are same mark)
- Updated `clients/memo-tm-symbols.md` with singular/plural TM guidance

**Commits:**

- `fc8de7f` — Add intellectual foundations + new ERNY vs TAM FAQ
- `1bfae01` — Split People in Pain intro into two paragraphs

**Wayback Machine snapshot:** https://web.archive.org/web/20260212204735/https://nascentidea.com/
**Spec file:** `~/Downloads/nascent-popper-additions-v3.1.md`
**TM policy:** `clients/memo-tm-symbols.md` + `ip-and-url-strategy.md`

---
