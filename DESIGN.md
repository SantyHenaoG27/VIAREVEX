---
name: Viarevex
description: Personal travel advisory — designing exceptional journeys down to the last detail.
colors:
  gold: "#B89A62"
  navy: "#101A2B"
  obsidian: "#0B0B0C"
  ivory-canvas: "#FAF9F6"
  linen-surface: "#F4F0E8"
  crimson: "#C8453B"
  ink-dark: "#3a3a3c"
  ink-mid: "#55555a"
  muted: "#B9B4AA"
  muted-deep: "#8a857c"
typography:
  display:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(40px, 6.6vw, 82px)"
    fontWeight: 500
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "clamp(30px, 4.4vw, 52px)"
    fontWeight: 500
    lineHeight: 1.1
  title:
    fontFamily: "Cormorant Garamond, Georgia, serif"
    fontSize: "24px"
    fontWeight: 600
    lineHeight: 1.15
  body:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "16.5px"
    fontWeight: 300
    lineHeight: 1.75
  body-sm:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "14.5px"
    fontWeight: 300
    lineHeight: 1.65
  label:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "12px"
    fontWeight: 400
    letterSpacing: "0.26em"
rounded:
  sharp: "2px"
  card: "3px"
  pill: "12px"
  circle: "50%"
spacing:
  section: "clamp(70px, 10vw, 130px)"
  card-inner: "28px 26px 30px"
  gap-grid: "26px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.obsidian}"
    rounded: "{rounded.sharp}"
    padding: "15px 30px"
  button-primary-hover:
    backgroundColor: "#c4a870"
    textColor: "{colors.obsidian}"
    rounded: "{rounded.sharp}"
    padding: "15px 30px"
  button-navy:
    backgroundColor: "{colors.navy}"
    textColor: "#F4F0E8"
    rounded: "{rounded.sharp}"
    padding: "14px 28px"
  button-ghost-gold:
    backgroundColor: "transparent"
    textColor: "{colors.gold}"
    rounded: "{rounded.sharp}"
    padding: "14px 28px"
  button-ghost-light:
    backgroundColor: "transparent"
    textColor: "{colors.ivory-canvas}"
    rounded: "{rounded.sharp}"
    padding: "15px 30px"
---

# Design System: Viarevex

## 1. Overview

**Creative North Star: "The Velvet Itinerary"**

Viarevex's visual language is a perfectly printed travel brief: precise margins, unambiguous hierarchy, nothing superfluous. Every decision was made before you had to ask. The site does not sell — it accompanies. Its aesthetic is the artifact of someone who has been everywhere twice and knows exactly what matters.

The palette operates in two temperatures: the warm off-white of body surfaces and the cold depth of navy and near-black, held together by a single accent — a muted, travel-worn gold that reads like aged brass, not showroom shine. Sections alternate between light and dark fields, creating a rhythm of contraction and expansion that mirrors how a good journey actually unfolds: bright days, deep nights, no monotony.

Typography carries the voice. Cormorant Garamond handles everything editorial — display headings, serial numbers, pull quotes — and Inter handles everything functional. Their contrast is absolute: one is a letter written by hand, the other is a label on well-made luggage. Neither apologizes for what it is.

This system explicitly rejects the visual grammar of booking platforms (price grids, star ratings, search bars), the excess of traditional luxury (gold wallpaper, baroque flourishes, chandeliers in every section), and the casualness of influencer travel content (vibrant color splashes, rounded everything, zero friction). The Velvet Itinerary is confident without shouting. Elegant without trying.

**Key Characteristics:**
- Two-temperature palette: warm neutral surfaces + cold deep fields, bridged by a single gold accent
- Razor-sharp geometry (2px radius) — no softness as default, no rounding as politeness
- Editorial serif for presence, humanist sans for precision — never mixed within the same type role
- Sections alternate between dark and light fields — rhythm, not repetition
- Motion is sparse and purposeful: scroll reveals once, never loops

## 2. Colors: The Two-Temperature Palette

A three-family system: warm neutral surfaces, cold deep fields, and one muted gold that bridges both. Nothing competes with the accent; it earns its place by being alone.

### Primary
- **Aged Brass** (`#B89A62`): The singular accent. CTAs, active borders, serial numbers, bullet markers, section kickers, and the logo diamond. Its muted warmth distinguishes it from ostentatious gold — closer to a well-traveled watchband than a hotel lobby railing. Never used as a background beyond the primary button.

### Secondary
- **Midnight Atlantic** (`#101A2B`): Deep navy. Section backgrounds (process, header), package card backgrounds, secondary CTAs, and dark headings on light surfaces. Not decorative — structural.
- **Obsidian** (`#0B0B0C`): Near-black. Footer, aviation section, darkest fields, and text color on Gold buttons. Maximum contrast, minimum warmth.

### Tertiary
- **Crimson** (`#C8453B`): Logo diamond + form validation errors only. One deliberate intrusion of urgency. Never decorative.

### Neutral
- **Ivory Canvas** (`#FAF9F6`): Body background. Warm off-white at near-zero chroma — the open road.
- **Linen Surface** (`#F4F0E8`): Section surface tint. Slightly warmer; used for services, FAQ, and corporate sections to create the light-side alternation.
- **Warm Parchment** (`rgba(244,240,232)`): Light text on dark backgrounds, used at 0.72–0.85 opacity for prose on dark fields.
- **Ink Dark** (`#3a3a3c`): Primary body text on light backgrounds. Slightly blue-shifted — not pure black, not mid-gray.
- **Ink Mid** (`#55555a`): Secondary body text, card descriptions. Readable without competing with headings.
- **Dusk Muted** (`#B9B4AA`): Footer links and muted labels on dark surfaces.
- **Deep Muted** (`#8a857c`): Footer descriptions. The quietest voice.

### Named Rules

**The One Voice Rule.** Aged Brass (`#B89A62`) is the only accent color. It appears on less than 15% of any given screen — kickers, bullets, borders, one CTA. Its rarity is the point. A second accent would dilute the trust it signals.

**The Two-Temperature Rule.** Light sections (Ivory Canvas / Linen Surface) always alternate with dark sections (Obsidian / Midnight Atlantic). No two consecutive sections share the same temperature. Monotony is a luxury brand killer.

**The Crimson Exception.** Crimson (`#C8453B`) appears in two contexts only: the logo mark and form validation errors. Adding it anywhere else breaks the accent discipline.

## 3. Typography

**Display Font:** Cormorant Garamond (weights 400, 500, 600 — italic 400 available), Georgia, serif
**Body Font:** Inter (weights 300, 400, 500, 600), system-ui, sans-serif

**Character:** Cormorant Garamond carries the editorial voice — unhurried, classical, built for reading on a long flight. Inter carries the operational layer — precise, unemotional, legible at 12px in a mobile nav. Their pairing is contrast, not complement: neither font tries to be the other.

### Hierarchy
- **Display** (weight 500, `clamp(40px, 6.6vw, 82px)`, line-height 1.02, letter-spacing -0.01em): Hero headline only. One instance per page. Cormorant Garamond.
- **Headline** (weight 500, `clamp(30px, 4.4vw, 52px)`, line-height 1.1): Section headings (h2). Cormorant Garamond. Warm Parchment on dark fields; Midnight Atlantic on light fields.
- **Title** (weight 600, 22–24px, line-height 1.15): Card and component headings (h3). Cormorant Garamond. The 600 weight separates it from Headline without size inflation.
- **Body** (weight 300, 16.5px, line-height 1.75): Primary prose. Inter Light. Max-width ~520px. Low weight and generous leading create a conversational, unhurried register.
- **Body Small** (weight 300, 14.5px, line-height 1.65): Card descriptions and secondary prose. Inter Light.
- **Label** (weight 400–500, 12px, letter-spacing 0.26em, uppercase): Section kickers, navigation, CTA text. Inter. The generous tracking makes 12px feel authoritative, not tiny.

### Named Rules

**The Weight Inversion Rule.** Serif headings at weight 500 feel lighter than sans-serif labels at weight 400. This is intentional — display faces are delicate, functional text is precise. Never bold a Cormorant heading for emphasis; increase font-size instead.

**The Tracking Doctrine.** Uppercase Inter labels carry 0.24–0.26em tracking. Headings use -0.01em or normal. Wide tracking is a label register signal — never apply it to body copy.

## 4. Elevation

Viarevex uses stratified, intentional depth. Surfaces are flat at rest. Shadows appear as narrative anchors — signaling "this element carries weight," not "this element is hovered." The philosophy is editorial: depth communicates importance, not interaction state.

### Shadow Vocabulary
- **Showcase anchor** (`0 30px 70px -40px rgba(16,26,43,.7)`): The destination gallery. Deep, wide — the shadow "sinks" the showcase into the page. The signature elevation moment of the site.
- **Header separation** (`0 10px 34px -22px rgba(0,0,0,.7)`): Sticky header on scroll. Tight radius, moderate depth — enough to lift navigation above content it crosses.
- **Ambient float** (`0 6px 24px rgba(11,11,12,.3)`): Floating action elements (WhatsApp button, back-to-top). Diffuse, lightweight.
- **Modal lift** (`0 8px 30px rgba(11,11,12,.4)`): Toast notifications and overlaid panels. Slightly more opaque to assert the surface above page content.

### Named Rules

**The Structural Anchor Rule.** Shadows mark structural importance, not hover feedback. Cards do not gain shadows on hover. The showcase gallery holds the only "signature" shadow on the page. If you're using shadows for decoration, remove them.

## 5. Components

### Buttons

Razor-sharp geometry. Uppercase Inter labels. Gold is the primary action; Navy is the secondary; Ghost variants adapt to surface temperature.

- **Shape:** Nearly sharp (2px radius)
- **Primary (Gold):** `#B89A62` background, `#0B0B0C` text, padding 15px 30px, 13px Inter 500, letter-spacing 0.06em, uppercase. The only element carrying the brand's full warmth.
- **Secondary (Navy):** `#101A2B` background, `#F4F0E8` text, same geometry. Used on light surfaces where Gold would compete with accent borders.
- **Ghost Gold:** Transparent background, `1px solid #B89A62` border, `#B89A62` text. Used on dark surfaces (aviation, final CTA).
- **Ghost Light:** Transparent background, `1px solid rgba(244,240,232,.45)` border, `#FAF9F6` text. Paired with Gold primary on dark surfaces.
- **Text Link CTA:** `border-bottom: 1px solid #B89A62`, no background. 12px, uppercase, letter-spacing 0.12em. Inside cards for secondary actions.

### Cards / Containers

- **Corner Style:** Nearly sharp (2px radius), 3px for large showcase surfaces
- **Background on light fields:** `#FAF9F6` with `1px solid rgba(184,154,98,.22)` gold-tinted border
- **Background on dark fields:** `#101A2B` with `1px solid rgba(184,154,98,.28)` gold-tinted border
- **Shadow Strategy:** None at rest. Structural anchor shadows only (see Elevation)
- **Internal Padding:** 28px–34px

### Inputs / Fields

Minimal underline style — no stroke box, no fill. The form disappears so content doesn't.

- **Style:** Bottom border only — `1px solid #B9B4AA`, background: none, 15px Inter
- **Focus:** Requires custom treatment (native browser default active; a gold underline focus should be added for WCAG compliance)
- **Error state:** Red Inter text `#C8453B` below submit, `role="alert"` aria-live
- **Textarea:** Full border (1px solid #B9B4AA), 2px radius, resizable vertically

### Navigation

- **Desktop:** Inter 13px, letter-spacing 0.04em, `#F4F0E8` color — horizontal flex on Midnight Atlantic header
- **Language toggle:** Ghost border, 11px, letter-spacing 0.1em
- **CTA in nav:** Gold primary button, always visible in header
- **Mobile:** Full-height side panel sliding in from right — `#101A2B` background, Cormorant Garamond 18px nav links with gold-tinted border-bottom separators, `padding: 13px 0`

### Destination Showcase (Signature Component)

A 16:9 full-width hero with a scrollable thumbnail rail below. The hero image zooms on each slide change (`animation: vxzoom 9s ease-out forwards`). The thumbnail rail uses `#0B0B0C` background; active thumbnail receives `border: 1px solid #B89A62`. Carousel navigation: 46px circle ghost buttons (`rgba(11,11,12,.4)` bg, `backdrop-filter: blur(4px)`) positioned center-left and center-right. This component anchors the destinations section and is the largest single motion moment outside the hero.

## 6. Do's and Don'ts

### Do:
- **Do** keep Aged Brass (`#B89A62`) as the only warm accent on any screen. Its rarity is what makes it credible.
- **Do** alternate section backgrounds between warm neutral and cold deep fields without exception. This temperature rhythm is structural, not decorative.
- **Do** use Cormorant Garamond at weight 500 for section headings, 600 for card titles — never 700 for editorial emphasis. Increase size instead.
- **Do** keep border-radius at 2px for interactive elements, 3px for large showcase panels. Rounding is constrained and deliberate.
- **Do** use uppercase Inter at 0.24–0.26em tracking for all kickers, CTAs, and label-register text — and only there.
- **Do** use full-bleed photography as the primary content vehicle. Alt text should name the specific place and mood, not the generic category.
- **Do** let imagery carry destinations. As PRODUCT.md states: "Show, don't sell." The founder was there; show what they saw.

### Don't:
- **Don't** build price-comparison grids, star-rating rows, or booking-engine filters. Viarevex is "the opposite of a marketplace" (PRODUCT.md). Transaction patterns contaminate the premium reading.
- **Don't** add gold beyond its defined roles. "Ostentatious luxury (excess of gold)" is an explicit anti-reference in PRODUCT.md. Gold as wallpaper is the opposite of sophistication.
- **Don't** introduce a second typographic accent. No Playfair, no Lora, no second display serif alongside Cormorant Garamond. The editorial voice is already spoken.
- **Don't** add hover shadows to cards or list items. Shadows are structural anchors, not state feedback. See the Structural Anchor Rule.
- **Don't** apply wide letter-spacing (> 0.1em) to body copy. Tracking is reserved for the label register — it signals category, not sentence.
- **Don't** replace photography with CSS color blocks or decorative shapes. A solid-color rectangle where a hero photo belongs is broken design. Zero imagery on this brief is a bug.
- **Don't** borrow visual grammar from Booking.com, Expedia, or Despegar — no search bars, no filter toggles, no price badges. These patterns make Viarevex unreadable as the premium, personal service it is.
- **Don't** use influencer-style elements: no rounded pastel callouts, no neon accents, no emoji as decorative icons, no viral-format motion.
