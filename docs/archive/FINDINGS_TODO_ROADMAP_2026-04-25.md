# Auralis Digital — Findings, Corrections, TODOs, and Roadmap

Date: 2026-04-25
Status: Active planning document
Scope: Repo review findings, website corrections, business-readiness TODOs, visual design roadmap, and implementation order

---

## Purpose

This document consolidates the grounded review findings for the current Auralis Digital repo and turns them into a practical action roadmap.

It is meant to prevent drift, avoid random redesigns, and keep future work tied to the real business goal:

- make the website credible
- make the offer clear
- capture leads reliably
- support outreach and sales
- build a memorable brand without hurting conversion

---

## Current Repo / Website Summary

Auralis Digital is no longer a starter template.

The current site has a complete marketing homepage with:

- premium dark styling
- Auralis Digital logo in the hero
- local-business positioning
- services section
- example work / portfolio preview
- pricing section
- process section
- founder section with real founder photo
- why-it-matters / trust section
- proof-point messaging
- Michigan service area section
- FAQ section
- contact section
- mobile sticky CTA
- desktop sticky contact buttons
- footer
- SEO metadata
- structured data
- social preview SVG asset
- service-area pages
- sitemap and robots file

The repo also includes supporting business documents:

- current state checkpoint
- regression checklist
- next-steps implementation plan
- lead capture strategy
- massive visual design direction
- brand guide
- ad campaign document
- outreach scripts
- lead reply scripts
- active outreach tracker
- lead tracker template

---

## What Is Strong

### 1. Homepage foundation is strong

The homepage has enough structure to sell from now. It clearly explains what Auralis Digital does, who it helps, what it costs to start, and how a prospect can take action.

### 2. Brand positioning is mostly aligned

The brand direction is grounded: professional websites for local businesses, built around trust, clarity, calls, quote requests, and customer action.

### 3. Pricing is clear enough for early sales

The current pricing tiers are simple and understandable:

- Website Refresh — $250
- Basic Website — $500+
- Standard Website — $1,000+
- Premium / Custom — quote based

This is strong for outreach because prospects can quickly understand whether the service is in range.

### 4. Local SEO structure exists

The site already has service-area pages for:

- Belleville
- Ypsilanti
- Ann Arbor
- Detroit Metro

The sitemap and robots file are present and point to the live domain.

### 5. Sales support docs exist

The repo is not only a website. It already includes outreach scripts, lead tracking, response scripts, and campaign guidance. This gives the business a lightweight sales operating system.

### 6. Visual direction is now documented

The future high-impact design direction is captured in:

`docs/MASSIVE_VISUAL_DESIGN_DIRECTION_2026-04-25.md`

This protects the idea of a cinematic sci-fi city "wow" moment while keeping the rest of the site practical and conversion-focused.

---

## What Is Weak / Needs Correction

### 1. Lead capture is still the biggest weakness

The current contact form opens a prepared email using `mailto:`. This is usable as a fallback, but it is not true lead capture.

Problems:

- the visitor may not have an email app configured
- the visitor can abandon the email before sending
- no submission is stored automatically
- no success state exists
- no analytics event exists
- no CRM or lead log is created

Correction:

- install Formspree now
- keep phone and email fallback visible
- add success/error feedback
- later upgrade to a custom backend

### 2. Analytics are missing

The site cannot currently measure:

- quote button clicks
- phone clicks
- form submissions
- portfolio clicks
- pricing interest
- service-area page performance

Correction:

- add privacy-friendly analytics
- track important CTA events
- use analytics before making major conversion decisions

### 3. Proof-point section can look like testimonials

The current proof-point cards use quote-like styling and language. The content is conceptual and honest, but visually it may look like testimonials.

Correction:

- rename or reframe the section so it is clearly not fake testimonials
- suggested section title: `Built around real customer behavior`
- keep real testimonials for later, after client permission exists

### 4. Portfolio demo has at least one placeholder contact path

The Bryan's Neighborhood Coney demo contains an owner-preview mailto path using `hello@example.com`.

Correction:

- replace placeholder email with `auralisdigitaleco@gmail.com`
- check all demo CTAs before using them in outreach

### 5. Founder photo path is messy

The founder photo currently loads from a folder path with spaces:

`website%20building%20LLC/25e7f6af-bc55-47ba-811d-2c0a5ea43978.jpeg`

Correction:

- copy image to `assets/founder-photo.jpeg`
- update `index.html` only after the copied asset is verified
- do not delete the old asset until the new path is confirmed live

### 6. Social preview is SVG only

The social preview asset exists as SVG. Some platforms handle SVG preview images inconsistently.

Correction:

- add `assets/social-preview.png`
- update Open Graph image to PNG only after the PNG exists and is verified

### 7. Service-area pages are thin

The service-area pages exist and are useful, but they are simpler than the homepage and do not yet carry the full trust/conversion structure.

Correction:

- improve service-area pages after lead capture is working
- add stronger local CTAs
- add founder trust snippet
- add services/pricing preview
- keep each page locally useful and not spammy

### 8. Documentation has minor drift

Known drift:

- checkpoint document contains a typo: `n- Ypsilanti`
- regression checklist references an older safe restoration commit; useful, but should clarify it is a restoration baseline, not necessarily current head
- README says `lead intake form`, but should remain clear that the current form is mailto until Formspree is installed

Correction:

- clean up documentation after the next implementation pass
- keep docs aligned with actual site behavior

---

## Immediate Corrections TODO

These are the highest-priority fixes before major design expansion.

### Lead Capture

- [ ] Create Formspree project / endpoint.
- [ ] Update the existing homepage contact form to submit to Formspree.
- [ ] Preserve all current form fields.
- [ ] Keep direct email and phone fallback visible.
- [ ] Add form success message.
- [ ] Add form error message.
- [ ] Test live submission end-to-end.
- [ ] Do not remove mailto fallback until Formspree is verified.

### Analytics

- [ ] Choose analytics provider.
- [ ] Recommended options: Plausible, GoatCounter, Cloudflare Web Analytics, or Google Analytics.
- [ ] Track hero CTA clicks.
- [ ] Track phone clicks.
- [ ] Track form submissions.
- [ ] Track portfolio/demo clicks.
- [ ] Track pricing page or pricing-section engagement.
- [ ] Track service-area page visits.

### Portfolio Demo Cleanup

- [ ] Replace `hello@example.com` in the Bryan's demo.
- [ ] Check demo phone links.
- [ ] Check demo email links.
- [ ] Check image paths.
- [ ] Check mobile layout.
- [ ] Confirm demo pages are safe to share with prospects.

### Proof / Trust Cleanup

- [ ] Reword proof-point section so it does not look like fake testimonials.
- [ ] Keep conceptual proof separate from real client testimonials.
- [ ] Add real testimonials only after client permission exists.

### Asset Cleanup

- [ ] Copy founder photo to `assets/founder-photo.jpeg`.
- [ ] Verify the new image path exists.
- [ ] Update homepage image path surgically.
- [ ] Keep old image file temporarily.
- [ ] Add `assets/social-preview.png`.
- [ ] Update Open Graph image only after PNG is verified.

### Documentation Cleanup

- [ ] Fix `n- Ypsilanti` typo in current state checkpoint.
- [ ] Clarify regression checklist baseline language.
- [ ] Update README after Formspree is installed.
- [ ] Update checkpoint after each major implementation pass.
- [ ] Keep roadmap, checkpoint, and live site behavior aligned.

---

## Roadmap

## Phase 1 — Conversion Foundation

Goal: make the current site reliably capture and measure leads.

Tasks:

- [ ] Install Formspree.
- [ ] Add success/error form states.
- [ ] Preserve fallback contact options.
- [ ] Add analytics.
- [ ] Track CTA behavior.
- [ ] Fix the Bryan's demo placeholder email.
- [ ] Clean proof-point wording.
- [ ] Update docs after changes.

Why this comes first:

The current site already looks good enough to start selling. Reliable lead capture is more valuable than another visual pass.

---

## Phase 2 — Site Structure Split

Goal: break the long homepage into focused pages.

Create or improve:

- [ ] `services.html`
- [ ] `portfolio.html`
- [ ] `pricing.html`
- [ ] `about.html`
- [ ] `contact.html`

Homepage should become shorter and more focused:

- [ ] cinematic hero / brand intro
- [ ] quick service preview
- [ ] quick portfolio preview
- [ ] trust/founder preview
- [ ] strong CTA to contact page

Navigation should become:

- Home
- Services
- Portfolio
- Pricing
- About
- Contact

Why this matters:

Separating pages improves readability, SEO targeting, animation performance, and conversion clarity.

---

## Phase 3 — Cinematic Visual Upgrade

Goal: add the desired massive visual identity without hurting the business flow.

Recommended first implementation:

- [ ] lightweight cinematic homepage hero
- [ ] nighttime near-future city mood
- [ ] fog / haze layers
- [ ] subtle particles
- [ ] soft blue-white neon glow
- [ ] light shimmer
- [ ] optional parallax
- [ ] reduced-motion support
- [ ] mobile fallback

Do not start with full 3D.

Preferred first stack:

- HTML
- CSS
- vanilla JavaScript
- SVG / compressed image assets
- optional Canvas later

Why this matters:

The site gets a memorable "wow" moment while staying fast and practical.

---

## Phase 4 — Portfolio / Showcase Upgrade

Goal: use the portfolio page to show stronger design ability.

Tasks:

- [ ] create stronger portfolio page layout
- [ ] show restaurant demo
- [ ] show lawn care demo
- [ ] add future barber/salon demo
- [ ] add future contractor/service demo
- [ ] add explanation of what each site is designed to improve
- [ ] add animated project cards
- [ ] add hover depth and glow effects
- [ ] keep demos clearly labeled as examples

Why this matters:

The portfolio page is where stronger visuals support sales instead of distracting from the homepage CTA.

---

## Phase 5 — Local SEO Expansion

Goal: make service-area pages more useful and more locally relevant.

Tasks:

- [ ] improve Belleville page
- [ ] improve Ypsilanti page
- [ ] improve Ann Arbor page
- [ ] improve Detroit Metro page
- [ ] consider adding Downriver page
- [ ] consider adding Canton page
- [ ] consider adding Livonia page
- [ ] consider adding Romulus page
- [ ] consider adding Taylor page
- [ ] update sitemap after adding pages

Each local page should include:

- local headline
- city/service-area relevance
- business types served
- service overview
- pricing preview
- direct CTA
- internal links
- contact path

Avoid thin, repetitive SEO spam.

---

## Phase 6 — Testimonials / Case Studies

Goal: replace conceptual proof with real trust assets.

Tasks:

- [ ] collect client permission before publishing testimonials
- [ ] add real testimonial section
- [ ] add simple case study format
- [ ] add before/after examples where appropriate
- [ ] document what was improved: clarity, mobile layout, contact flow, service explanation

Suggested case study structure:

1. Business type
2. Problem
3. Website solution
4. Customer action improved
5. Screenshot / preview
6. Testimonial if available

---

## Phase 7 — Advanced Motion / Experimental Design

Goal: explore more advanced motion only after the business foundation is stable.

Possible tools:

- GSAP
- Canvas
- Three.js
- Spline
- Blender
- Figma

Possible features:

- animated skyline layers
- flickering city lights
- moving fog
- light beams
- mouse-reactive depth
- portfolio page cinematic transitions
- optional 3D showcase scene

Rules:

- do not make every page heavy
- do not sacrifice readability
- keep mobile fallbacks
- support reduced motion
- test load performance

---

## Implementation Order Recommendation

Best next order:

1. Formspree lead capture
2. analytics
3. demo placeholder cleanup
4. proof-point wording cleanup
5. founder image asset cleanup
6. social preview PNG
7. split pages
8. cinematic homepage hero
9. portfolio page upgrade
10. service-area expansion
11. testimonials / case studies
12. advanced motion experiments

---

## Technical Safety Rules

When editing `index.html`:

- fetch the full current file first
- make surgical changes only
- never replace it with a placeholder
- preserve existing sections unless intentionally moving them into subpages
- preserve SEO metadata
- preserve structured data unless updating it accurately
- preserve mobile CTA behavior
- preserve direct phone/email fallback
- test form behavior after changes

When adding assets:

- verify asset exists before referencing it
- keep file names simple
- prefer `/assets/` for shared site assets
- compress images
- avoid massive unoptimized video backgrounds

When adding animation:

- include reduced-motion fallback
- do not block content rendering
- keep text readable
- keep CTA visible
- ensure mobile performance

---

## Business Safety Rules

Do not claim:

- guaranteed leads
- guaranteed revenue
- fake testimonials
- fake client results
- inflated agency scale
- unsupported AI capabilities

Do claim:

- clear website structure
- mobile-ready design
- better first impression
- easier customer action
- practical local-business websites
- founder-led process
- transparent starting pricing

---

## Current Best Next Move

The next implementation pass should be:

**Formspree + analytics + demo cleanup + proof wording cleanup.**

This is the best ROI because it improves the real sales funnel without risking the working homepage.

After that, split the site into separate pages and then add the cinematic hero visual system.
