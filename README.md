# Fancy Millwork — Design System

The visual and verbal system for **Fancy Millwork**, the architectural millwork division of **Fancy Floors Incorporated**. Custom cabinetry and woodworking studio for high-end residential interiors. We collaborate with architects, interior designers, and custom builders to deliver precise, furniture-grade work — kitchens, libraries, paneled rooms, bars, vanities, and full-house millwork packages.

> Sister brand to Fancy Floors (the hardwood flooring division). The two divisions share materials, craftsmanship standards, and aesthetic DNA; this system describes the millwork extension.

---

## Sources & inputs

This system was built from the following materials supplied by the client:

- **Logo** — `uploads/logo.png` (original Fancy Floors corporate mark, red/grey with serif wordmark). Preserved at `assets/fancyfloors-original-logo.png`. A new editorial wordmark for the Millwork division (`assets/wordmark-millwork.svg`) extends the brand for this division while leaving the parent mark intact.
- **Photography** — 13 reference photographs of finished projects: classic-paneled kitchens, walnut-floored interiors, a bookcase wall inspired by De Stijl, a walnut-and-onyx primary bath, two coffered-ceiling clubrooms with bar and cigar lounges. All copied into `assets/` with semantic filenames.
- **Brand brief** — written direction: *ultra luxury architectural studio aesthetic; modern, minimal, cinematic; editorial-style layout inspired by high-end interior design studios; warm off-white, walnut wood tones, soft black accents.*
- **Capability statement** — long-form copy describing services, standards, target market, differentiators. The verbal voice in this system is derived directly from that document.

No codebase, no Figma file, no existing live website were provided. The Millwork division is treated here as a **new editorial brand** that inherits material culture from Fancy Floors but establishes its own visual language for the architect / designer / luxury homeowner audience.

---

## Index

| File / folder | What's in it |
|---|---|
| `README.md` | This document — brand context, content & visual fundamentals, iconography. |
| `SKILL.md` | Agent-skill entry point. Use this when invoking the system as a skill. |
| `colors_and_type.css` | All design tokens — colors, type, spacing, radii, shadow, motion. |
| `assets/` | Logos, monogram, photography library. |
| `preview/` | Small HTML specimen cards that populate the Design System tab. |
| `ui_kits/website/` | The marketing website UI kit — components and an interactive index. |

---

## Content fundamentals

The Fancy Millwork voice is **understated, specific, and architectural**. It reads like the studio bio in an interior design magazine — confident enough to leave silence, precise enough to never overstate. Every sentence should sound like it could be read aloud by the owner of the firm to a serious architect at a site walk.

### Tone

- **Restrained, never breathless.** "A studio for custom architectural millwork." Not "Welcome to the world of luxury woodworking!"
- **Material-first.** We talk about walnut, rift-sawn oak, polished brass, and Carrara marble — not "premium materials" or "high-quality finishes." Be specific.
- **Process as proof.** We earn trust by describing *how* we work: shop drawings, AWI compliance, scheduling. Never with adjectives like "amazing" or "best-in-class."
- **Quiet confidence.** Avoid superlatives. "Furniture-grade" is a fact; "world-class" is a brag.

### Voice patterns

- **Person.** Mostly third-person studio voice ("Fancy Millwork collaborates with…"). First-person plural ("We…") is used selectively, in the About / Studio sections, for warmth. Never second-person marketing voice ("You'll love…").
- **Casing.** Sentence case in body. **UPPERCASE WITH WIDE TRACKING** for eyebrows, labels, and section indices. Display headlines use Title Case sparingly — most large headlines are sentence-case for editorial feel.
- **Punctuation.** Em dashes are encouraged — they create the cadence. Oxford comma. Periods at the ends of all sentences, including pull quotes.
- **Numbers.** Spell out one through nine; numerals for 10+. Years and dimensions always in numerals. Project counts and indices use monospaced numerals (e.g. `Index 014 / 042`).
- **No emoji. Ever.**
- **No exclamation marks.**
- **No jargon-as-marketing.** "Value engineering" appears once, in services. It does not appear on the homepage.

### Example copy

These are the actual lengths and rhythms we should hit:

> **Hero (homepage).**
> *Custom architectural millwork for residences that hold up to a closer look.*

> **Section opener — Capabilities.**
> *Kitchens, libraries, paneled rooms, vanities, full-house packages. Designed in coordination with the architect, fabricated to AWI standards, installed under our own supervision.*

> **Project caption.**
> *Lakeside Residence, Connecticut. Rift-sawn white oak, hand-rubbed oil finish. 2024.*

> **About paragraph.**
> *Fancy Millwork is the architectural millwork studio of Fancy Floors. We work with a small number of architect-led projects each year, from a single library wall to a complete interior package. Our work is documented like architecture and installed like furniture.*

> **CTA.**
> *Begin a project →*  (not "Get started," not "Contact us today")

### Words we use

walnut, rift-sawn, quarter-sawn, oil-rubbed, hand-rubbed, furniture-grade, paneled, coffered, dovetailed, mitred, casework, carcass, dimension, tolerance, joinery, scope, drawing set, site survey, finish schedule, lead time, install.

### Words we avoid

solutions, premium, world-class, cutting-edge, bespoke (overused), elevated, luxury (when it could be a description of materials instead), elevate, transform, journey, experience, "your dream kitchen."

---

## Visual foundations

The Fancy Millwork interface is **a quiet stage for photography of finished rooms**. UI chrome is almost absent. Where it appears, it is hairline-thin, sharp-cornered, and warm-neutral.

### Mood in one paragraph

Imagine the studio's own portfolio book, printed on warm cream paper with a deep walnut endpaper. Photographs are large — sometimes full-bleed, often three-quarter-bleed with a thin caption sitting in the margin in 11px tracked-out caps. Typography is editorial: a Cormorant-family serif at display sizes, Inter Tight in sans for everything else, JetBrains Mono for indices and dimensions. The page breathes — vertical rhythm is generous, sometimes 192px between sections. The only color besides paper-and-ink is the walnut accent itself, used like a thread you can pull but rarely as a fill.

### Color

- **Paper neutrals** (`--fm-paper-50` through `--fm-paper-400`). Warm off-white scale — pages are `--fm-paper-50`, cards/inset surfaces are `--fm-paper-100`/`200`. **Never pure white.**
- **Ink** (`--fm-ink-900` through `--fm-ink-100`). Soft architectural black scale — `--fm-ink-900` (#1a1714) is the darkest you go. **Never pure black.**
- **Walnut** (`--fm-walnut-100` through `--fm-walnut-900`). The brand's signature warm. `--fm-walnut-500` is the accent color used for links, the underline-on-hover, key emphasis, and small filled controls.
- **Brass** (`--fm-brass-500`, `--fm-brass-700`). A single metallic note — hardware-inspired. Used only for hover-state underlines on key links and the most-emphasized CTA on the page.
- **State colors** (`--fm-success`, `--fm-warning`, `--fm-danger`). Muted, earth-toned — lichen green, burnt amber, terracotta. **No saturated reds, no bright greens.**
- **Imagery color.** Warm. Slightly golden. Long shadows. All photography sits in a 3200–3800K color temperature; cool/blue interiors are reframed warm in post if needed. A subtle film grain is acceptable; heavy filters are not.

### Type

- **Display serif:** Cormorant Garamond, 300–500 weight, with negative tracking at display sizes. Used for hero headlines, page openers, the wordmark, and the italic *lede* paragraph that introduces a section.
- **Sans:** Inter Tight, 400/500/600. Body, UI, captions, navigation, button labels.
- **Mono:** JetBrains Mono, 400/500. Indices, dimensions, project numbers, captions when adjacent to drawings.
- **Hierarchy:** Display 1 (128px) → Display 2 (88px) → H1 (64px) → H2 (40px) → Lede (24px italic serif) → Body (16px) → Caption (12px) → Eyebrow (11px tracked +0.32em).
- **Eyebrow labels are critical.** Tracked-out (0.32em) uppercase 11px in `--fm-ink-500`, often paired with a hairline above the headline they sit on. This is the single strongest signal that the brand is editorial.

### Spacing & layout

- 4px grid, scaling to 192px section breaks.
- 12-column grid, 24px gutter, 48px outer page gutter on desktop.
- Generous whitespace. A homepage section often runs 96–192px tall vertically between elements. **More air than feels comfortable.**
- Pages are wide (`--fm-container: 1440px`, `--fm-container-wide: 1680px`). Never feel cramped.

### Backgrounds & imagery

- **Photography is the primary visual.** Full-bleed at the top of pages and as section dividers. Three-quarter-bleed with margin captions in editorial body sections.
- **No gradients** (the warm light in the photography is the gradient). The only acceptable gradient is the soft top-down protection scrim on top of a full-bleed image, `linear-gradient(to bottom, rgba(26,23,20,0.4), transparent 30%)`, used only when text sits over the image.
- **No patterns, no textures, no hand-drawn illustrations.** Marble veining and wood grain are the only "textures" — and they come from the photography, never CSS.
- **No stock illustration.** Where an icon is needed, see Iconography below.

### Hover & press states

- **Links.** Walnut accent color. On hover: a hairline brass underline grows from 0 to 100% width in 320ms `--fm-ease-out`. No color change.
- **Buttons (primary).** Ink-900 fill, paper-100 text. Hover: walnut-700 fill. Press: walnut-900 fill, no shrink.
- **Buttons (secondary / outline).** Hairline ink-900 border, ink-900 text. Hover: fill becomes ink-900, text becomes paper-100. Press: same with `--fm-shadow-inset`.
- **Cards / image tiles.** Hover: image scales `1.03` in 640ms `--fm-ease-out`; the caption underline animates in; the card itself does not move.
- **No transforms on press of static UI** (no shrink, no jump). Sub-1px nudges only.

### Borders

- Hairlines everywhere: `1px solid var(--fm-border)` is the workhorse.
- Strong borders (`--fm-stroke: 1.5px`) only on hero outlines and key data tables.
- Border color always neutral (`--fm-paper-300` or `--fm-ink-100`). Walnut/brass are used as text and underlines, not as borders.

### Shadows

- Used sparingly. Most surfaces sit at elevation 0 — the page is flat by default.
- When elevation is needed (a floating menu, a hover state for a project tile), shadows are **soft, large, warm-tinted, and far-offset** (`--fm-shadow-md` and up).
- No hard 1–2px drop shadows on cards. If a card needs separation, use a 1px hairline border instead.
- Inset shadows mark sunk panels (search field, inset spec block).

### Corner radii

- **Default is sharp (0).** Architectural means crisp edges.
- 2–4px allowed on small controls (input fields, buttons, pills) for tactile softness.
- 8px is the maximum and is used only on the largest image cards.
- No pill buttons, no 9999px radii anywhere except small icon dots / status indicators.

### Cards

- Background: `--fm-paper-100` (or `--fm-paper-200` for inset variants).
- Border: 1px solid `--fm-paper-300`, or no border + `--fm-shadow-md` — never both.
- Radius: `--fm-radius-md` (4px) by default; image tiles use `--fm-radius-sm` (2px).
- Padding: `--fm-space-6` (32px) on desktop, `--fm-space-5` (24px) on tablet/mobile.
- The card title sits on a line of its own, often with an eyebrow above and a thin walnut line below the headline.

### Motion

- **Cinematic, not bouncy.** No spring physics. No overshoot. Custom-bezier ease-out for entrances, ease-in-out for navigation transitions.
- Page-to-page navigation should feel like a curtain wipe or a slow scrub. Use `--fm-dur-curtain` (1200ms) for full-screen image reveals.
- Body content reveals on scroll with a 24–48px translate and 0→1 opacity over `--fm-dur-slow` (640ms).
- Reduced-motion: respect `prefers-reduced-motion`. Skip translations; keep fades.

### Transparency & blur

- Used **only** on overlay scrims for hero text legibility, and on the sticky top navigation when it overlays imagery (rgba `--fm-paper-50` at 80% with 12px backdrop-blur).
- No frosted-glass cards. No translucent modals over translucent modals.

### Fixed elements

- The top navigation is the only fixed-position element by default. It is hairline-thin (56–64px tall), warm-neutral, and disappears its border when sitting over the full-bleed hero (then re-applies the hairline once the page scrolls).
- No floating chat bubbles, no sticky CTAs at the bottom of the page, no cookie banners disguised as design elements.

---

## Iconography

Icons in this system are **a last resort**, not a primary visual element. Photography and typography do the work. When an icon is necessary (a directional arrow on a "Next project" link, a phone glyph in the footer, a checkmark in a feature list), follow these rules:

### System

- **Library:** [Lucide](https://lucide.dev) (`lucide.dev`), linked from CDN.
- **Stroke weight:** 1.5px (Lucide default). Never increased; for very small contexts (12–14px) consider increasing to 1.75px only.
- **Cap & join:** round. (This softens the otherwise sharp interface.)
- **Color:** inherits `currentColor` from surrounding text. Never colored independently.
- **Size:** 16px (inline with body), 20px (button), 24px (standalone in a nav rail). 32px+ is too loud.
- **Substitution note.** No proprietary icon set was supplied. Lucide is chosen because its 1.5px hairline stroke, round caps, and architectural geometry match the brand's hairline-everywhere visual language better than Heroicons (heavier strokes) or Font Awesome (filled). Replace with a bespoke set when budget allows.

### Logo & wordmark

- **Original Fancy Floors corporate mark:** `assets/fancyfloors-original-logo.png` — preserved for legal/contractual use, footer co-branding, invoices. Not used as the primary identity for the Millwork division.
- **Fancy Millwork wordmark (primary):** `assets/wordmark-millwork.svg`. Editorial serif "FancyMillwork" with hairline rule and "a Fancy Floors studio" tracked-out beneath. Use this in the top navigation and on light backgrounds.
- **Fancy Millwork wordmark (light):** `assets/wordmark-millwork-light.svg` — same mark, paper-100 fill, for use over dark imagery and on the ink-900 backgrounds.
- **FM monogram:** `assets/monogram-fm.svg` — square mark with thin keyline, used at small sizes (favicon, social avatars, project card overlays).

### Emoji & unicode

- **Emoji: never.** Not in marketing, not in product, not in error states.
- **Unicode glyphs:** used sparingly and intentionally. `→` for forward action, `↗` for external link, `·` (middle dot) as a separator in meta lines, `—` (em dash) for editorial rhythm. Bullets in lists are `—` not `•`.
- **No icon fonts** beyond standard typographic glyphs.

### Asset inventory

| File | What it is |
|---|---|
| `assets/wordmark-millwork.svg` | Primary wordmark, ink on paper |
| `assets/wordmark-millwork-light.svg` | Wordmark, paper on ink |
| `assets/monogram-fm.svg` | FM square monogram, small-size use |
| `assets/fancyfloors-original-logo.png` | Parent brand corporate mark (preserved) |
| `assets/img-kitchen-walnut-floor.jpeg` | Hero-grade kitchen with walnut floor |
| `assets/img-kitchen-viking-range.jpeg` | Symmetrical kitchen, range centerpiece |
| `assets/img-kitchen-window-sink.jpeg` | Carrara-marble kitchen, classic |
| `assets/img-kitchen-classic-white.jpeg` | Classic painted kitchen |
| `assets/img-kitchen-detail.jpeg` | Kitchen detail shot |
| `assets/img-kitchen-blue-island.jpeg` | Painted blue island, marble herringbone |
| `assets/img-builtin-mondrian-wall.jpeg` | De Stijl–inspired built-in (signature) |
| `assets/img-bath-walnut-vanity.jpeg` | Walnut + onyx primary bath |
| `assets/img-lounge-bar.jpeg` | Walnut bar / wine room |
| `assets/img-lounge-bar-alt.jpeg` | Bar alt angle |
| `assets/img-lounge-coffered.jpeg` | Coffered-ceiling clubroom |
| `assets/img-detail-2.jpeg`, `assets/img-detail-3.jpeg` | Misc. interior details |

---

## Open questions / known substitutions

1. **Display & body fonts are substitutions.** Cormorant Garamond + Inter Tight are Google Fonts standing in for an editorial serif (GT Sectra, Canela, or similar) and a precise neutral sans (GT America, Söhne). If the studio has licensed fonts, swap them in by replacing the `@import` and `--fm-font-display` / `--fm-font-sans` values.
2. **Iconography** is Lucide via CDN as a stylistic match. A bespoke icon set is recommended for production.
3. **The "Millwork" wordmark is new** and proposed as an extension of the Fancy Floors identity. Sign-off needed before broad use.
4. **No real project metadata** was supplied — project names, locations, years, and client quotes used in the UI kit are plausible placeholders.

