# nascentidea.com Changelog

Last archived: 2026-05-20

## TODO: Add analytics to nascentidea.com — Cloudflare Web Analytics (free) for page views (#1) + GA4 (free) for CTA-click tracking (#2)

Funnel Mike wants to measure: page views → CTA button clicks → booked meetings (#3 already visible in Cal.com). Currently ZERO analytics on the site (`index.html` has no tracking code — only script is a mobile-nav toggle). No retroactive data recoverable since May 20th launch.

- **#1 page views** — Cloudflare Web Analytics (free). Natural to fold into the Cloudflare migration (pivotstory.org Cloudflare setup already queued). DNS currently at Namecheap; either move DNS to Cloudflare (also gets server-side traffic + CDN/SSL) or use JS-beacon mode without moving DNS.
- **#2 CTA clicks** — GA4 (free). CTA = `https://cal.com/nascent/founder?ref=nascentidea.com` (external link), so GA4 Enhanced Measurement auto-tracks it as an outbound click. Add a cookie/consent notice with GA4.
- Cal.com does NOT give #2 — its Insights track bookings only, not booking-page visits by referrer. Confirmed Jul 17th.
- Mike chose Cloudflare + GA4 (both free) over Plausible ($9/mo). Deferred to a future session — "don't wanna deal w this now."

## No other WIP.

---

## [~2:30 PM] PT Thu Jul 16th 2026

### Namecheap domain portfolio scoped — decision: null project

**Context:** Mike owns ~22 Namecheap domains (bmccontrarian.com, chiefpivotofficer.com, contrarianfounder.com, dollarsofpain.com, ernyvalue.com, quantifypain.com, etc.), bought ~a year ago (~$170), auto-renewed a couple weeks ago. Auto-renew now OFF — they lapse over the next year. Source: `~/Downloads/Domain List_july 16th 2026.pdf`.

**Decision: do nothing.** Scoped and closed as a null project:

- Redirecting all 21 unused domains to nascentidea.com rejected — near-zero traffic × domains dying within a year = zero ROI, not worth even 20 min.
- One-page GitHub Pages microsites / Google Doc rejected — zero-authority exact-match domains don't rank (Google devalued EMDs ~2012; thin microsite networks = doorway-page spam risk). Invisible to AEO too (LLMs retrieve from linked, crawled content).
- If SEO/AEO on coined terms (ERNY, QPG, disideation) is ever wanted, the play is content on nascentidea.com or Substack (where authority exists), not domains. Out of scope here.
- Domains lapse naturally on their expiration dates; $170 written off.
- Mike confirmed nascentstartups.com email + auto-renew settings are under control (not CC's concern).

---


## [~12:00 PM] PT Wed May 20th 2026

### Remove Paul Tepper testimonial + add ERNY pronunciation note

**What was done:**

- Removed Paul Tepper testimonial blockquote from index.html (was between Doug Ambort and Ellen Classen). Per Mike: rest of website stays as-is.
- Kept `images/PaulTepper-linkedin-1516284815226.jpeg` on disk in case the testimonial returns later.
- Added inline pronunciation note `(ERNY, pronounced "Ernie")` in 2 spots: pricing deliverables paragraph and FAQ 2.3 ERNY definition. (Edit had been sitting uncommitted since Feb 13th 2026.)
- Started tracking `changelog.md` in git (previously untracked since Feb).

**Commits:**

- `643095d` — Add ERNY pronunciation note ("Ernie")
- `137e1f5` — Remove Paul Tepper testimonial

---
