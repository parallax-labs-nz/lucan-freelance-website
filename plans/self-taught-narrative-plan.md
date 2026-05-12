# Plan: Weaving the Self-Taught Narrative into Lucan Fulcher's Website

## Objective
Subtly communicate that Lucan's development and AI skills were born from real operational experience — not formal education — without explicitly stating "self-taught." Avoid em dashes in the actual site content and keep language natural, not AI-sounding.

## Changes Summary

### Change 1: Web & App Development service description
**File:** [`index.html`](index.html:357) — service row for Web & App Development

**Current (line 358):**
> Clean, functional digital products for small and medium-sized businesses. Whether you need a new website, a web application, or a mobile app, I build things that are straightforward to use and built to last. No bloat, no unnecessary complexity.

**Proposed:**
> I build digital products shaped by years inside the operations that need them. Whether it's a website, a web application, or a mobile app, the goal is the same: straightforward, functional, built to solve real problems. No bloat, no unnecessary complexity.

---

### Change 2: About section — add a bridge paragraph
**File:** [`index.html`](index.html:460) — about-text div

**Current structure:**
1. "I've spent the better part of a decade working across customer experience..." (CX/ops background)
2. "That work has taken me into some complex environments..." (gov't/compliance + formal quals)
3. "These days I also run Parallax Labs..."
4. "If something isn't working the way it should..."

**Proposed:** Add a new paragraph between #2 and #3:

> Over that time I kept coming back to the same thought. So much of the friction in business came down to tools and systems that just weren't built for how people actually work. So I started building my own. What began as a way to solve specific problems became a genuine passion for development, and eventually Parallax Labs.

Then reword the existing Parallax Labs paragraph (#3) slightly:

> These days I run Parallax Labs, an AI software studio based in Auckland. For me the consulting and the development are the same thing. I like working directly with businesses on the stuff that's frustrating them, not just building software about it.

---

### Change 3: Add a skill entry under Web & Development
**File:** [`index.html`](index.html:444) — skill-list under "Web & Development"

Add after "SEO structure and metadata":

> Built from scratch, templates optional

---

## Execution Order
1. Update the service description (Change 1)
2. Update the About section (Change 2)
3. Add the skill entry (Change 3)
4. Preview and verify the text flows naturally
