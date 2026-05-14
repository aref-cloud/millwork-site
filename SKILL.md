---
name: fancy-millwork-design
description: Use this skill to generate well-branded interfaces and assets for Fancy Millwork — the architectural millwork studio of Fancy Floors — either for production or throwaway prototypes, mocks, decks, and marketing pages. Contains essential design guidelines, colors, type, fonts, project photography, and UI kit components for prototyping.
user-invocable: true
---

Read the `README.md` file within this skill, and explore the other available files.

The brand is a custom architectural millwork studio — kitchens, libraries, paneled rooms, vanities, full-house millwork packages — under the Fancy Floors umbrella. The aesthetic is editorial, architectural, cinematic: warm off-white paper, walnut wood tones, soft architectural blacks. Think the studio bio in an interior design magazine. Photography is the primary visual; UI chrome is hairline-thin and quiet.

Key files:

- `README.md` — full content & visual fundamentals, iconography, voice/tone, asset inventory. **Read this first.**
- `colors_and_type.css` — all design tokens (color, type, spacing, radii, shadow, motion).
- `assets/` — logos (wordmark, inverse wordmark, monogram, parent corporate mark) and the project photography library (13 images: kitchens, baths, lounges, built-ins).
- `ui_kits/website/` — component-by-component recreation of the marketing site. Use this as a reference for layout, type pairing, image treatment, and the eyebrow+headline+lede pattern that defines the brand.
- `preview/` — small specimen cards for each design token group.

If creating visual artifacts (slides, mocks, throwaway prototypes, marketing pages, decks): copy assets out of `assets/`, import `colors_and_type.css` for the token layer, and follow the static HTML patterns in `ui_kits/website/`. Reach for full-bleed photography, generous vertical rhythm (96–192px section breaks), the display serif at scale, and the tracked-out monospace eyebrow labels. Do not invent new colors; the palette is small on purpose.

If working on production code: copy `colors_and_type.css` into the project and use the CSS variables. The component patterns in `ui_kits/website/` are reference-quality but not production-hardened — replicate the structure, not the file layout.

If the user invokes this skill without any other guidance, ask them what they want to build — a marketing page section, a project portfolio piece, a deck, a one-pager, an email — ask 2–4 focused clarifying questions, and act as an expert designer for the Fancy Millwork brand.

### House rules (the things you must never do for this brand)

- Never use pure white (#fff) or pure black (#000). Use `--fm-paper-50` and `--fm-ink-900`.
- Never use emoji. Never use exclamation marks in marketing copy.
- No rounded-pill buttons. Default radius is sharp; 8px max on the largest cards.
- No saturated reds, blues, or greens. State colors are muted earth tones.
- No CSS gradients, patterns, or hand-drawn illustrations. The photography is the texture.
- No second-person marketing voice ("You'll love..."). The voice is third-person studio.
- No filler content. If a section feels empty, it's a layout problem, not a content problem.

### House rules (the things you should always do)

- Use the eyebrow + hairline rule + index pattern (`01 / 04`) on every section opener.
- Use the display serif (Cormorant Garamond) for headlines, the sans (Inter Tight) for body, and the mono (JetBrains Mono) for indices, dimensions, and project numbers.
- Caption every photograph. Captions live in monospace, tracked-out, in the margin.
- Earn trust by being specific. Say "rift-sawn white oak" not "premium hardwood."
