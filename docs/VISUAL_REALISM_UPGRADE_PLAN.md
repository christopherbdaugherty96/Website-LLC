# Auralis Digital Visual Realism Upgrade Plan

Date: 2026-04-26

## Why this document exists

The current Auralis homepage has a stronger concept than before, but the execution still reads too much like CSS shape art. The moon looks like a circle, the skyline can feel like spreadsheet blocks, and many lower-page sections/demos still rely on similar dark cards.

This document captures the next visual direction before more code changes are made.

---

## Current honest status

### What is working

- The brand direction is clearer.
- The desert road / distant city metaphor is strong.
- The homepage is more memorable than the earlier generic layout.
- The demo library is visible from the homepage.
- Services, pricing, founder, and contact sections are more polished than before.

### What is not working yet

- The hero does not look realistic enough.
- The moon and skyline still feel geometric.
- The desert does not yet feel like a real place.
- The road does not yet feel like a real road.
- The moving traffic effect is still a light-streak abstraction, not an actual vehicle.
- Below the hero, sections can still feel like repeated card blocks.
- Demo pages need stronger individual character by business type.

---

## Core visual goal

Auralis should feel cinematic, premium, and memorable.

The site should not feel like a generic web agency template.

The intended emotional image:

> A quiet desert at night. A real road cuts through the dark toward a glowing near-future city. Moonlight, neon, haze, and motion create a sense of visibility, direction, and momentum.

This supports the business message:

> A clearer path from first impression to first call.

---

## Main homepage hero direction

### Environment

- Realistic desert at night
- Open space, dust, haze, dunes, road texture
- Cinematic atmosphere
- Dark but readable
- Premium, not cartoonish

### Moon

- Round moon
- Real moonlight glare
- Atmospheric glow
- Soft light spill across the sky and desert
- Not a flat circle

### City

- Distant near-future desert city
- Cyberpunk-inspired lighting
- Blue, cyan, magenta, and warm gold glare
- Not literally Las Vegas
- Should feel aspirational and far away
- Must have depth, haze, and bloom rather than simple block towers

### Road

- Realistic road surface
- Strong perspective toward the city
- Subtle lane reflection or light catch
- Should visually support the headline

### Movement

Preferred motion order:

1. Subtle car/bike/bus headlight motion along the road
2. Moonlight glow breathing slowly
3. City light shimmer
4. Desert haze drifting
5. Tiny star twinkle

Motion should feel cinematic and expensive, not arcade-like.

---

## Recommended implementation approach

### Do not rely on pure CSS for realism

CSS is useful for:

- glow overlays
- haze
- light streaks
- shimmer
- responsive positioning
- subtle animation

CSS is not ideal for:

- realistic desert texture
- realistic moonlight
- real road perspective
- convincing city depth
- natural vehicle motion

### Better approach

Use a layered visual system:

1. **Realistic hero background image**
   - A generated or custom-designed cinematic scene.
   - Desert road at night, moon, distant future city.

2. **Overlay gradient**
   - Keeps text readable.
   - Creates brand consistency.

3. **Motion overlays**
   - Animated headlights / light streaks.
   - Subtle haze.
   - City glow shimmer.
   - Moonlight pulse.

4. **Text and CTAs**
   - Kept clean and readable on the left.

---

## Hero asset prompt

Use this prompt for creating the main realistic hero image:

> A cinematic realistic night desert highway scene, low angle from the road shoulder, asphalt road leading into the distance toward a glowing near-future city skyline on the horizon, not Las Vegas but inspired by neon desert city lights, large realistic full moon with soft moonlight glare, atmospheric haze, subtle dust in the air, cyberpunk blue and magenta glow in the distance, premium dark cinematic mood, realistic photography style, wide website hero composition, empty space on the left for text, ultra detailed, realistic lighting, no logos, no text.

Suggested aspect ratios:

- 16:9 for desktop hero
- 21:9 for wide desktop crop
- 4:5 or 9:16 variation for mobile crop if needed

---

## Homepage section character plan

The rest of the homepage should not feel like repeated cards.

### Services section

Add service-specific visual moments:

- Website Refresh: before/after cleanup feel
- Starter Website: launch path / first light
- Growth Website: expanding city lights / signal lines

### Example Work section

Turn into a showroom:

- Add real or generated thumbnails for each demo.
- Make the cards feel like previews, not text blocks.
- Demo Library should feel like a gallery wall.

### Pricing section

Make pricing feel like premium package cards:

- Stronger package hierarchy
- Larger prices
- Clear “best for” labels
- Included features
- Calm buyer-confidence copy

### Founder section

Make the section more editorial:

- Stronger photo treatment
- Founder note / quote
- “Why I built Auralis” language
- Trust badges

### Contact section

Make it feel like a final destination:

- Glowing panel
- Simpler form rhythm
- Clear “ready to move forward?” message

---

## Demo page character plan

Each demo should feel different.

### Restaurant

- Warm local atmosphere
- Menu-first
- Food imagery
- Hours/location/call flow

### Lawn Care

- Green outdoor neighborhood feel
- Before/after yard imagery
- Quote-first flow

### Barbershop

- Sharp black/cream style
- Appointment focus
- Confident typography

### Painter

- Color swatches
- Clean home interior feel
- Portfolio-style work examples

### Cleaning

- Bright, airy, fresh
- White/blue visual tone
- Trust and recurring-service focus

### Roofing / Contractor

- Strong, rugged, practical
- Warranty/trust focus
- Quote-first layout

### Salon

- Soft, elegant, beauty-focused
- Appointment-first layout

### Mobile Detailing

- Glossy black/chrome/car reflection feel
- Before/after visuals

### Photographer

- Gallery-first
- Portfolio-heavy
- Minimal text

### Maintenance / Handyman

- Reliable, practical, tool/workshop feel
- Checklist/service-area layout

---

## Near-term execution plan

### Phase 1 — Documentation and issue tracking

- Document this realism plan.
- Create a GitHub issue to track visual realism upgrades.

### Phase 2 — Hero asset placeholder implementation

- Add a hero-image layer and fallback CSS.
- Keep current CSS art as fallback, but make room for a real background image.
- Add a clear asset path such as `assets/hero-desert-city.jpg`.

### Phase 3 — Create/select visual assets

- Generate or source realistic hero background.
- Create demo thumbnails.
- Add visual previews to demo cards.

### Phase 4 — Section character pass

- Reduce repeated-card feeling.
- Add varied section layouts.
- Improve visual storytelling down the page.

### Phase 5 — Demo identity pass

- Upgrade each demo one at a time.
- Give every demo a distinct mood, palette, typography, and CTA flow.

---

## Non-goals

- Do not make the homepage chaotic.
- Do not add heavy video before performance is checked.
- Do not overdo cyberpunk effects so the business message gets lost.
- Do not pretend generated visuals are client work.
- Do not make every demo share the same generic dark-card design.

---

## Quality bar

The goal is not just “clean.”

The goal is:

> A small business owner should see the homepage and think: this looks professional, memorable, and more impressive than what I could make myself.

Auralis should feel worth showing off.
