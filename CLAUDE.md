# Project notes — Ian Bonaparte portfolio

This file holds all the **content** of the portfolio so it can be rebuilt in a different
layout or theme without re-deriving anything. Copy below is final and approved — reuse it
verbatim. Working file: `Ian Bonaparte PS2.dc.html`. Stale export: `index.html`.

---

## Positioning

- Name: Ian Bonaparte
- Title: **Design Engineer**
- Tagline: "Bridging the gap between design and engineering teams"
- Sub-line: "UX/UI Designer with an expertise in front-end engineering. Experienced in leading and building multiple product and website redesigns."
- Audience: recruiters and hiring managers at product companies
- Location: Boston, MA
- Email: IanNBonaparte@gmail.com
- LinkedIn: https://www.linkedin.com/in/ian-napoleon-bonaparte/
- Primary CTA: "Get in touch"
- Aesthetic: PlayStation 2 boot-screen inspired (blue void, floating monoliths, glass panels) — the *look* only, not a literal PS2 UI recreation. Avoid PS2 menu language like "System Configuration".

## Copy voice rules (learned from review)

- No uppercase letter-spaced treatment on nav or buttons. Keep it only for small sub-labels (section labels, stat captions, metric labels).
- No glow: no `text-shadow` halos, no `box-shadow: 0 0 Npx` bloom. Flat fills on buttons, not gradients.
- Avoid the "not X, it was Y" inversion and aphoristic closing sentences. End paragraphs plainly.
- Avoid "best in class" except inside a real quote.
- Vary the shape of list labels; don't start every one with the same verb form.

## Page structure (in order)

1. Sticky header: wordmark + nav
2. Hero: name, title, tagline, sub-line, CTA
3. Stat strip (3 stats)
4. Selected work (4 cards)
5. About
6. Skills (5 columns)
7. Contact
8. Footer

**Nav order must match page order:** Work, About, Skills, Contact.

## Stat strip

| Value | Label |
|---|---|
| 8 yrs | Front-end experience |
| 4 | Product redesigns |
| 200+ | A/B tests launched |

The "4 product redesigns" are: Jordan's Ecom Website (biggest, most challenging), Debticate
New UI (second biggest, better coordinated team), Jordan's IMAX online experience (post-COVID:
new rules, new tech), Enchanted Village online experience. Ian's note: the last two are
arguably a stretch as "product redesigns," but they qualify.

## About (2 paragraphs, verbatim)

> I design interfaces and then build them. For eight years that has mostly meant sitting between design and engineering teams: prototyping in Figma, writing the front end that actually ships, and putting together the design systems other engineers work out of.

> Most recently I led the front end for a fintech platform's component library and UI redesign. Before that I spent years in ecommerce, where almost nothing shipped without a test behind it. I got used to reading analytics and making the case from numbers instead of taste. A lot of that was analytics engineering: standing up Tag Manager properly and writing markup that feeds clean data into dashboards. I have worn a lot of hats along the way, so I bring marketing and analytics knowledge that most front-end engineers do not.

## Skills (5 groups)

- **Languages**: HTML/CSS (Sass), JavaScript, React, C, C#, C++
- **Design systems**: BEM Methodology, Atomic Design, Progressive Enhancement, WCAG 2.1 Compliant
- **Analytics**: Google Tag Manager, Google Analytics, Dashboard-ready markup, A/B testing
- **AI-assisted**: Prompt-driven prototyping, Claude Code, Claude Design, Cursor
- **Domains**: Ecommerce, Fintech, Finance, SaaS

## Contact

Heading is the email itself as a large link. Supporting line:

> Always happy to talk product, design systems, or motion, whether it's a role or a project.

Buttons: LinkedIn, Email.

---

# Case studies

**Featured order is deliberate — strongest project first, not newest-first:**
1. Jordan's Furniture Site Redesign
2. Debticate New UI Overhaul
3. Debticate AI Assistant
4. Jordan's Furniture Enchanted Village

**Detail page structure:** Year → Name → Tagline → metadata strip (Role / Domain / Impact / Year)
→ Screens → Problem → Approach → What I built → Outcome (metrics + paragraph + quote) → Next project.

---

## 01 — Jordan's Furniture Site Redesign

- Blurb: End-to-end Ecommerce reimagination
- Year: 2022-23 · Role: Front End Engineer & Project Manager · Domain: Ecommerce
- Impact: 400% more product page traffic; ecom sales up 40%
- Screens: public (not gated)

**Tagline**
> A three-year rebuild of the ecommerce site at Jordan's Furniture, covering navigation, product pages, checkout and the analytics underneath them.

**Problem**
> The site was running an outdated design with slow pages, a confusing navigation structure and a checkout people gave up on. Nobody could say what shoppers were looking for, because nothing was being collected to answer that. Internally it was not taken seriously either. "Who buys furniture online" was a common phrase around the office.

**Approach**
1. **Executive buy-in came before any of the design work** — The people funding the project had to believe furniture sells online. I walked executive stakeholders through the work early and kept doing it, so by the time we built anything the site had real backing inside the company.
2. **Navigation rebuilt around shoppers, not the org chart** — The old structure mirrored how the business was organized internally. I restructured product discovery and checkout around how people actually shop for furniture, which meant fewer top-level categories and a much shorter path to a product page.
3. **Sitecore, so marketing stopped waiting on engineering** — Campaign updates used to sit in a front-end queue. Building on Sitecore let the marketing team launch their own campaigns without us. Unglamorous work, but it changed how fast the company could move.
4. **We A/B tested our way into the final designs** — Most of the open questions went out as tests instead of opinions: navigation labels, product card layouts, promo placement, checkout steps. Whichever version won became the design. Over 200 tests ran across the project, and having the numbers made design reviews considerably shorter.
5. **A Google Tag Manager structure that outlived the project** — The old site collected almost nothing, so I set up Google Tag Manager properly, with consistent naming feeding a handful of Google Analytics dashboards. Traffic and revenue could be tracked long after launch, and whoever picked the site up next had somewhere to start.

**What I built**: Full front-end development of the redesign · Sitecore implementation for marketing self-service · Restructured navigation and product discovery · Rebuilt checkout experience

**Metrics**: +400% Traffic to product pages · +40% Ecom sales, following year · +8% Credit card applications

**Outcome**
> Traffic to product pages went up 400%. Ecommerce sales the following year were up 40%, and Jordan's credit card applications rose 8%.

**Quote**
> The website was never taken seriously until I helped show the potential.

---

## 02 — Debticate New UI Overhaul

- Blurb: Complete fintech platform redesign
- Year: 2024-25 · Role: Designer + Front End Engineer · Domain: Fintech SaaS
- Impact: Established design system standards where none existed
- Screens: **gated** (NDA). Thumbnail is the Debticate wordmark.

**Tagline**
> Debticate is a fintech SaaS loan syndication platform. Its interface was still built like it was 2005, and there was no design system to fix it with.

**Problem**
> Debticate ran on an outdated 00s UI with no shared visual language. Buttons that did the same job looked completely different from page to page, because every engineer had written their own CSS for them. Whether a page felt consistent came down to who had built it.

**Approach**
1. **I pushed for a design system instead of a reskin** — Repainting the screens would have been faster and everyone knew it. I argued for building the system underneath first, because a reskin drifts apart again within a few releases.
2. **Atomic design, so a component existed once** — Everything composed up from atoms. A button lived in one place, with its variants written down as decisions instead of turning up later in somebody else's stylesheet.
3. **Semantic HTML and BEM naming, so other people could use it** — The system had to make sense to engineers who had not built it. Predictable BEM class names and semantic markup meant they could find the right component and reuse it without coming to ask me.

**What I built**: Component library covering the platform · Atomic design structure with BEM naming · Semantic, accessible markup standards · Redesigned core platform screens

**Metrics**: "Best in class" Experience · 100% Client retention

**Outcome**
> Engineers built faster and more consistently than before, and clients responded well to the new interface. Client retention held at 100%.

**Quote**
> Engineers on the new UI all commented on how easy and surprisingly quick pages were ready for QA, because of a well-structured design system.

---

## 03 — Debticate AI Assistant

- Blurb: AI Chatbot design
- Year: 2026 · Role: Designer + Front End Engineer · Domain: Fintech SaaS
- Impact: Request to production in under 60 days
- Screens: **gated** (NDA). Thumbnail is the Debticate wordmark.
- Timeline is **60 days**, not 30 — this is used for an internal application, so do not stretch it.

**Tagline**
> An AI assistant for Debticate, a fintech SaaS loan syndication platform, designed from scratch and in production in under 60 days.

**Problem**
> Clients had started expecting AI inside their day-to-day workflow. We had no assistant, no pattern for one, and no time for a long discovery phase.

**Approach**
1. **Scoped it down to the minimum first** — I defined the smallest assistant that would be genuinely useful and designed against that. Everything else went on a list for later, which kept the scope conversation short.
2. **Built out of the design system we already had** — The assistant needed patterns that did not exist yet, so I added them to the design system rather than leaving them as one-off screens. It looked native to the product from the first build.
3. **Handed engineers a system rather than a spec** — The components and conventions were already documented, so Claude Code could work straight from them and engineers had the assistant running in weeks. There was very little translation between design and build.

**What I built**: Assistant UI designed from scratch · New patterns folded into the design system · Front-end implementation alongside engineering

**Metrics**: <60 Days, request to production · Weeks Engineering build time

**Outcome**
> From request to production in under 60 days. Clients commented on how quickly it turned up.

**Design reference**: the real prototype lives in a separate project (`AssistantDocked.dc.html`).
The assistant docks *beside* the record view rather than over it, so the answer and the data stay
on screen together. Layout: app bar with assistant trigger → left nav, record workspace, docked
assistant panel (message bubbles, cited-source block, source/actions row, composer).

---

## 04 — Jordan's Furniture Enchanted Village

- Blurb: Online ticketing and in-person experience
- Year: 2023 · Role: Front End Engineer & Project Manager · Domain: Ecommerce
- Impact: First online ticketing; shorter lines, staffing from sales data
- Screens: public (not gated)

**Tagline**
> Jordan's Enchanted Village had never sold a ticket online. I built the flow that did, from landing page through to the printed ticket.

**Problem**
> COVID-era rules meant customers turned up expecting the whole thing to work online first. Jordan's had never sold Enchanted Village tickets online before, so there was nothing to improve on. All of it had to be built.

**Approach**
1. **The printed ticket was part of the design** — The experience does not end at checkout. I designed the physical ticket alongside the digital flow, so what people were holding in line matched what they had just bought online.
2. **Designed backwards from the door** — Store staff had to scan tickets at a busy entrance in December. I started from what worked at the door and shaped the checkout to fit it.
3. **Training the store staff was part of shipping it** — A flow the store did not understand would have fallen apart on opening night, so employee training was in scope from the start instead of being handed over after launch.

**What I built**: Landing page, design and development · Ticketing and checkout flow · Physical ticket design · Employee training on the new process

**Metrics**: First Online ticketing for the attraction · Shorter Lines at the door

**Outcome**
> The handoff from online to the door held up. Lines were shorter, and for the first time the store could staff those nights against how many tickets had actually sold.

---

# Mechanics worth rebuilding

## Screen viewer
Full-page screenshots presented in a browser-chrome frame that scrolls internally
(`height: min(64vh, 620px)`), with:
- page tabs when a project has more than one screen
- a Desktop / Mobile toggle that swaps the image source; the frame clamps to `max-width: 390px` on mobile
- a Full screen overlay: fixed, full-viewport, image fits to width (`width: 100%`), mobile capped at 430px and centred, vertical scroll only
- a `url` per screen shown in the chrome bar

Images must never be rendered with an unresolved template hole in `src` — build the `<img>`
nodes in logic and drop them in by name, or the browser fires failed requests for the literal string.

## NDA gate (Debticate projects only)
Client-side passphrase panel: lock icon, "Screens available on request", explanatory line, password
input, Unlock button, and a "Request access" mailto link. Unlock state is kept in
`sessionStorage` under `ib_screens`, with a "Hide screens" control to re-lock.
Passphrase: **ian-screens-2026** (obfuscated in source, not real security).

Ian's intent: the gate is largely **perception** — there are no screens behind it and he emails
them on request. Keep the mechanism; it reads as a considered process.

## Glow toggle
`glow` prop (boolean, **default false**). Glowing elements carry `data-glow-el`; the root carries
`data-glow="on|off"`, and an override rule kills `text-shadow`, `box-shadow` and `animation` when off.

---

# Assets

| Path | What |
|---|---|
| `assets/screens/jordans-home-desktop.png` | Jordan's home, full page desktop (2231×9503) |
| `assets/screens/jordans-home-mobile.png` | Jordan's home, full page mobile (760×12889) |
| `assets/screens/jordans-outdoor-desktop.png` | Jordan's Outdoor landing, desktop |
| `assets/screens/jordans-outdoor-mobile.png` | Jordan's Outdoor landing, mobile |
| `assets/screens/jordans-home-thumb.jpg` | 880×550 card thumbnail, cropped from the top of the desktop capture |
| `assets/screens/ev-desktop.png` | Enchanted Village desktop. **Doctored:** the sticky "Hours & Location" sidebar was moved up 1020px so its top aligns with the video section, because the full-page capture had placed it mid-page. |
| `assets/screens/ev-mobile.png` | Enchanted Village mobile |
| `assets/screens/enchanted-thumb.jpg` | 880×550 card thumbnail from the Enchanted Village banner |
| `assets/logo-debticate.svg` | Debticate wordmark, white + red mark, for dark backgrounds. Used as the card thumbnail for both Debticate projects. |

Thumbnails are generated, not reused originals — the source screenshots are 3–6 MB each.
Card thumbnails: 880×550 JPEG at q0.82, cover-fit, top-aligned.

---

# NDA / material constraints

- **Jordan's projects**: Ian can provide real screenshots.
- **Debticate projects**: under NDA. Subscription product, no public demo (competitors). No real UI screenshots. If visuals are ever needed, they must be abstracted: wireframe-level diagrams (Ian's preference), greeked or blurred screens, before/after flow charts, component-anatomy illustrations, or redacted crops.

# Open work

- CV: not yet supplied. Needs linking once Ian sends it (header download, Contact line, or both — undecided).
- GitHub: to be connected; repo export pending.
- `index.html` is a stale standalone export and must be regenerated before upload.
- Optional: screenshots for Jordan's checkout flow and the physical ticket design, which are the two strongest unillustrated items in the Enchanted Village case study.
