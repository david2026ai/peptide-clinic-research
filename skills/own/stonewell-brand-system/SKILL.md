---
name: stonewell-brand-system
description: Complete brand system for Stonewell Health — logo, colors, typography, video ad application, and paid creative guidelines. Use whenever building ads, landing pages, video end cards, MyDose store assets, or any public-facing material for Stonewell Health.
---

# Stonewell Health — Brand System

## Identity

**Brand:** Stonewell Health
**Domain:** stonewellhealth.com (Cloudflare Registrar, registered Nov 7, 2026)
**MyDose store ID:** dace0c9f-96fe-4711-92c5-5a83bf118ba4
**Position:** Premium longevity telehealth. Plan-first, clinician-guided. For high-performing adults who don't accept average healthcare.
**Channel:** YouTube TrueView + Meta video paid only. No organic.

---

## Logo — Concept A "The Foundation" (selected)

Three ascending horizontal bars. Bottom widest in ink, middle and top in teal. Reads: permanence, measurement, progress.

### Production files
- Full lockup SVG: `branding/stonewell/logo-A-production.svg`
- Favicon SVG: `branding/stonewell/favicon.svg`
- All concepts reference: `branding/stonewell/logo-concepts.html`

### Construction
```
Bar 1 (top):    width=16px, height=10px, rx=5, fill=#0E6B6A, opacity=0.55
Bar 2 (middle): width=36px, height=10px, rx=5, fill=#0E6B6A
Bar 3 (bottom): width=52px, height=10px, rx=5, fill=#15242E
Gap between bars: 7px
```

### Lockup rules
- Always: mark LEFT of wordmark (horizontal) or ABOVE wordmark (stacked)
- Minimum size: 120px wide for horizontal lockup
- Clear space: equal to bar height (10px) on all sides
- Never: stretch, recolor, rotate, or add effects to the mark
- Never: use mark without wordmark in ads (too abstract without context)

### Dark background version
- Bar 3 bottom: `#F3F6F8` (paper) instead of `#15242E`
- Bars 1–2: `#0E6B6A` unchanged
- Wordmark: `#F3F6F8`
- "HEALTH" submark: `#0E6B6A` unchanged

---

## Color System

| Token    | Hex       | Use |
|----------|-----------|-----|
| Ink      | `#15242E` | Primary text, logo bottom bar, dark backgrounds |
| Teal     | `#0E6B6A` | Accent, logo bars 1–2, "HEALTH" submark, CTAs |
| Paper    | `#F3F6F8` | Backgrounds, light-mode surface, dark-bg logo fill |
| Muted    | `#8A9BAA` | Secondary text, captions, metadata |
| White    | `#FFFFFF` | Card surfaces, overlays |

**Rules:**
- Never use hex values not in this list for UI
- All numbers: tabular-nums
- Text contrast: minimum 4.5:1 on all backgrounds

---

## Typography

### Display — Cormorant Garamond
- Weights: 300 (body display), 400 (default), 500 (wordmark, headlines), 600 (emphasis)
- Use: hero headlines, VSL title cards, ad supers, landing page H1–H2
- Italic (`font-style: italic`) in teal for accent phrases

### Body — DM Sans
- Weights: 300 (body copy), 400 (UI), 500 (labels, wordmark subtext)
- Use: body copy, landing pages, email, UI labels, supers in video

### Wordmark specification
```
"STONEWELL" — Cormorant Garamond 500, letter-spacing: 3px, all-caps
"HEALTH"    — DM Sans 500, letter-spacing: 6px, all-caps, color: #0E6B6A
```
Never alter spacing, weight, or case of either wordmark element.

---

## Video Ad Application (paid only)

### YouTube TrueView (16:9)
- **Lower-third:** Mark (28px tall) + wordmark on dark overlay, paper + teal, bottom-left
- **End card:** Arch or Foundation mark centered large, full lockup stacked, `stonewellhealth.com` in DM Sans 300
- **Hook duration:** 5 seconds to skip — brand must be visible in frame 1–3
- **Background:** Dark (#15242E or cinematic footage with 60% dark overlay)

### Meta 9:16 (Reels / Stories)
- **Opening frame:** Logo top-left corner, paper on dark, within first 1 second
- **End card:** Full lockup centered on dark, teal CTA button, URL
- **Lower-third supers:** DM Sans 400, paper white, teal for emphasis words

### End card text (always)
```
STONEWELL  [teal submark] HEALTH
stonewellhealth.com · Start your evaluation
```

---

## Paid Creative Rules (compliance-locked)

### Always say
- "Clinician-guided longevity program"
- "Personalized 12-month plan"
- "Physician-supervised assessment"
- "May support the body's natural [process]"
- "Prescriptions only if clinically appropriate"
- "Individual results vary"

### Never say in any ad or public page
- Compound names: NAD+, BPC-157, TB-500, sermorelin, ipamorelin, semaglutide, tirzepatide
- Outcome words: anti-aging, reverse aging, younger, add years, cure, prevent [disease], guaranteed
- "FDA-approved" for compounded products
- Specific result metrics in testimonials

### Video creative casting
- Target: grounded, research-engaged 40–65 adults (not gym influencers, not bodybuilders)
- Settings: home office, kitchen, outdoors — clinical credibility contexts
- No: visible vials, syringes, injection imagery, shirtless/before-after

### UGC interview questions (safe)
✅ "What were you trying to address when you started?"
✅ "How did you find a provider you trusted?"
✅ "What did the consultation feel like?"
✅ "What surprised you?"
✅ "What would you tell someone researching this?"

❌ "How much faster did you recover?"
❌ "Did you feel younger?"
❌ "How well does it work?"

---

## MyDose Store Configuration (applied Nov 7, 2026)

```
Brand kit: { primary: #15242E, secondary: #F3F6F8, accent: #0E6B6A,
             fontPairing: editorial, corners: rounded, style: soft, surface: tinted }
Store design: { siteName: "Stonewell Health", template: longevity,
                modules: { blog: false, reviews: false, cookieConsent: true } }
Domain: stonewellhealth.com (connect after store goes live)
```

**Next MyDose steps:**
1. Add products from catalog
2. Connect payouts
3. Launch store
4. Connect stonewellhealth.com domain (available post-launch)

---

## Sources
- Brand decisions: `docs/alignment/CURRENT.md`
- Logo concepts: `branding/stonewell/logo-concepts.html`
- Compliance rules: `skills/own/longevity-claims-guard/SKILL.md`
- Ads gate: `skills/clinic-legitscript-ads-gate/SKILL.md`
