**Kat** is a snack food ordering website for Kat.

- **For:** people who use it now and then, often on a phone
- **Screens:** website (screens where people get work done)
- **Runs on:** web
- **Feel:** friendly, bold, energetic (friendly, bold, playful)
- **Brand color:** Your brand color (#8C2224) is on the buttons exactly, with white text that reads clearly on it.
- **Decided:** 9 answers you gave, 1 picked for you; everything else uses sourced defaults
- **Standards:** 288 house standards followed (locked, house standards v3), 1 overridden by you; see the Standards section
- **Next:** zoom into Colors, Typography, Layout, or stop here: each level works
- **Licence risks:** none found

> Generated from `opendesigner/state.json` and `opendesigner/decisions.md`. Made with OpenDesigner 0.1.0. `opendesigner/tokens/` is the source of truth. Change the system with `engine.py set ...` and `engine.py build`, not by editing this file (notes inside `<!-- od:keep -->` blocks survive). Each section opens with one plain sentence; open **More** for the designer and engineer detail.

## Overview

> Zoom: sketch (0 of 3), 5 decisions in this area. To zoom in, answer Q-dir-01, Q-dir-02.
<!-- od:zoom area=overview level=0 -->

**Kat feels friendly, bold and playful. Screens are roomy, in a flat style.**
Designers: visual style: flat, tonal, glass · Code: `preset in state.json`

<details><summary>More</summary>

**Your answers here** (each one either sets tokens or is a rule for this section):
- What are these screens mostly for: selling, getting work done, reading, or enjoying an experience? **website (Operate)** (chosen; tokens; Q-scope-06)
- Where is the project now: an idea, being built, close to launch, or live with real users? **Being built** (assumed; owner input; Q-scope-07)

**Intent.** a snack food ordering website for Kat

- Audience: people who use it now and then, often on a phone
- The memorable thing: not recorded yet (Q-brand-02)
- Surfaces: website (Operate: density spacious; no hero; cards only to group related data)
- Platforms: web; inputs: pointer, touch
- Direction: preset flat2 (the default until Q-dir-01 is answered); feel friendly, bold, playful (your words: friendly, bold, energetic)

**Principles (ranked).**
No principles recorded yet (Q-brand-07). Until they are, the dials act as the tie-breakers below.

**Dial positions.** Three posture dials set the overall stance. Five character dials fine-tune it.

- **Expression 60/100** (productive to expressive: leaning expressive): type ratio 1.25, hero moments: significant-moments, expressive motion: significant-moments, brand color role: accent+signature-surface, containment: mixed.
- **Brand presence 80/100** (native to brand-led: brand-led): typeface suggestion: proprietary-brand-face, brand color placement: large-surfaces+custom-components, native component share about 32%, voice guidance: full.
- **Density 15/100** (spacious to compact: spacious): body 16px on the web, default control 48px, density mode spacious, icons 24px; hit areas never shrink.
- **Energy 55/100** (calm to energetic: balanced): standard easing [0.77, 0, 0.175, 1], duration multiplier 1.02, spring damping 1.0, heading weight 650, navigation: neutral.
- **Roundness 90/100** (sharp to soft: soft): control radius 16, icon corners rounded, caps round.
- **Depth 30/100** (flat to deep: flat): depth model: ring+faint-shadow.
- **Colorfulness 65/100** (monochrome to vivid: leaning vivid): scheme expressive, accent chroma 60.4 (HCT), 3 accent(s), surfaces: tinted-containers.
- **Warmth 80/100** (cool/formal to warm/friendly: warm/friendly): neutral tint chroma 0.015 at hue 58, borders: soft, sentence-case, contractions encouraged.

**Zoom by area** (sketch, broad, defined, detailed). You can stop at any level; each one works.

| Area | Zoom | Next questions |
|---|---|---|
| Colors | sketch | Q-color-02 |
| Typography | sketch | Q-type-01 |
| Layout | sketch | Q-space-01, Q-space-02, Q-space-03 |
| Elevation & Depth | sketch | Q-depth-01 |
| Shapes | sketch | Q-shape-01 |
| Components | sketch | Q-comp-01, Q-comp-02, Q-state-01 |
| Motion | sketch | Q-motion-01 |
| Modes and Themes | defined | Q-theme-02, Q-theme-04 |
| Iconography and Imagery | sketch | Q-icon-01, Q-icon-02, Q-icon-06 |
| Content and Voice | sketch | Q-voice-01, Q-voice-02, Q-voice-03 |
| Accessibility | sketch | Q-aud-03, Q-aud-04 |
| Platforms and Devices | sketch | Q-plat-05, Q-plat-10, Q-plat-08 |

The tokens in `opendesigner/tokens/` (DTCG 2025.10 with `opendesigner.resolver.json`) are the source of truth. This file is a generated view.

Decisions: D-0006 (answers.Q-scope-07), D-0009 (answers.Q-aud-01), D-0014 (macros), D-0016 (answers.Q-scope-06), D-0023 (answers.Q-aud-02).

</details>

**Taste card.** How it looks and feels, in five lines for you, your team and any AI that builds with it. Nothing on it is invented: each line says where it comes from.
Designers: style brief, mood in words · Code: `taste.brief, taste.never`

| Line | What it says | From |
|---|---|---|
| In your words | Not given yet. Describe the look as a picture, not adjectives (for example, "a quiet library at night"). | not asked yet |
| Color | Three accent colors: your brand color `#8C2224` (exactly) marks buttons, links and focus; `#937017`, `#98629c` add highlights. Everything else stays neutral. Keep the accent to small areas, about 15% of a screen at most (a rule of thumb, DC-L15-03). | brand color; colorfulness 65/100 |
| Shape | Buttons and fields have 16px corners; cards have 24px corners. Cards get a faint outline and a very soft shadow. | roundness 90/100, depth 30/100 |
| Motion | Balanced. Most movements take 200ms. They turn into fades when a person asks for less motion. | energy 55/100 |
| Never | Nothing yet. Say what it should never look like, or rate real screens in the taste poll. | not asked yet |

## Colors

> Zoom: sketch (0 of 3), 2 decisions in this area. To zoom in, answer Q-color-02.
<!-- od:zoom area=color level=0 -->

**Three accent colors: your brand color `#8C2224` (exactly) marks buttons, links and focus; `#937017`, `#98629c` add highlights.** Everything else stays neutral.
Designers: primary or brand accent · Code: `color.bg.accent`

<details><summary>More</summary>

**Intent.** Brand color `#8C2224` drives the accent ramp's hue; the Colorfulness dial (65) sets its chroma (scheme expressive, peak HCT chroma 60.39). The brand's role is **accent+signature-surface** and it sits closest to accent step 9. Your brand color #8C2224 is on the buttons exactly (white text on it reads at 8.86:1).

**How ramps are built.** Each hue gets twelve steps in OKLCH, placed by contrast. Step 8 reaches at least 3:1 (edges and focus). Steps 10 and 11 reach the text minimum on backgrounds 1-4. Step 12 reaches at least 7:1. Steps 2-6 are spaced evenly in lightness between step 1 and step 7. Light and dark ramps are solved separately. Dark solids are lighter and carry dark text (dark mode is a separate mapping, never an inversion). Text minimum: 4.5:1 (WCAG 2.2 AA).

| Ramp | Light steps 1-12 | Solid carries |
|---|---|---|
| `accent` | `#fffcfc` `#fdf2f1` `#fee6e4` `#ffdbd7` `#ffcfcb` `#ffc4be` `#ffb8b1` `#c66c67` `#8c2224` `#800f17` `#731116` `#542624` | light |
| `accent2` | `#fefdfa` `#f7f4ee` `#f1ebde` `#ece2ce` `#e7d9bd` `#e2d0ad` `#dcc79c` `#9d834b` `#937017` `#86650e` `#6f5305` `#403214` | light |
| `accent3` | `#fefcff` `#f8f3f8` `#f3e8f3` `#eedeef` `#ead4eb` `#e5c9e6` `#e0bfe2` `#a178a4` `#98629c` `#8a588d` `#734776` `#422d43` | light |
| `danger` | `#fffcfc` `#fff1ef` `#ffe6e3` `#ffdbd6` `#ffcfc9` `#ffc4bc` `#ffb8af` `#d2665c` `#d3403a` `#c13732` `#a22a26` `#5a221e` | light |
| `info` | `#fbfdff` `#eaf6ff` `#d9efff` `#c7e7ff` `#b5e0ff` `#a3d8ff` `#8fd1ff` `#008ed1` `#007cb7` `#0070a6` `#005c8a` `#003755` | light |
| `neutral` | `#fefcfb` `#f7f3f1` `#efebe8` `#e7e2de` `#dfd9d5` `#d8d1cc` `#d0c8c2` `#8d857f` `#7d746d` `#6b635d` `#5e5651` `#272321` | light |
| `success` | `#f9fefa` `#ecf6ee` `#dbf1de` `#c8ebce` `#b6e6be` `#a2e0ae` `#8eda9e` `#28994e` `#00883d` `#007b36` `#00652c` `#003d17` | light |
| `warning` | `#fffcf8` `#f8f4ec` `#f5eada` `#f1e1c6` `#eed8b3` `#eace9f` `#e7c58b` `#aa7f2e` `#efb23b` `#dca333` `#845d00` `#463002` | dark |

**Step-distance guarantee** (neutral, light; WCAG contrast of a foreground step on background steps 1-5):

| Foreground | on 1 | on 2 | on 3 | on 4 | on 5 |
|---|---|---|---|---|---|
| neutral 8 | 3.54 | 3.29 | 3.06 | 2.82 | 2.59 |
| neutral 9 | 4.47 | 4.15 | 3.86 | 3.56 | 3.27 |
| neutral 10 | 5.75 | 5.34 | 4.97 | 4.58 | 4.21 |
| neutral 11 | 7.02 | 6.51 | 6.06 | 5.58 | 5.13 |
| neutral 12 | 15.22 | 14.12 | 13.14 | 12.11 | 11.14 |

**States.** Hover is at least 1.15:1 from its fill and pressed at least 1.3:1, as shade steps (DC-L01-17). Where a color is unknown at design time, use the state opacities in `opacity.state.*`.

| Fill | Base | Hover | Pressed |
|---|---|---|---|
| `color.bg.action.primary` | `#8c2224` | `#6e1b1c` (1.29:1) | `#75000f` (1.34:1) |
| `color.bg.accent.bold` | `#8c2224` | `#6e1b1c` (1.29:1) | `#75000f` (1.34:1) |

**Semantic roles** (use these, never the ramps):

| Token | Light | Dark | Use |
|---|---|---|---|
| `color.bg.accent.bold` | `#8c2224` | `same` | Solid accent fill. |
| `color.bg.accent.bold-hover` | `#6e1b1c` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.accent.bold-pressed` | `#75000f` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.accent.subtle` | `#fee6e4` | `same` | Selected rows, accent badges. |
| `color.bg.accent.subtle-hover` | `#ffdbd7` | `same` | Hover on accent subtle fills. |
| `color.bg.accent.subtle-pressed` | `#ffcfcb` | `same` | Pressed accent subtle fills. |
| `color.bg.accent2.bold` | `#937017` | `same` | accent2 solid fill. |
| `color.bg.accent2.bold-hover` | `#86650e` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.accent2.bold-pressed` | `#7d5c00` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.accent2.subtle` | `#f1ebde` | `same` | accent2 subtle fill. |
| `color.bg.accent3.bold` | `#98629c` | `same` | accent3 solid fill. |
| `color.bg.accent3.bold-hover` | `#8a588d` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.accent3.bold-pressed` | `#814f85` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.accent3.subtle` | `#f3e8f3` | `same` | accent3 subtle fill. |
| `color.bg.action.primary` | `#8c2224` | `same` | Primary action. One per view (DC-L15-03, L15 P08). |
| `color.bg.action.primary-hover` | `#6e1b1c` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.action.primary-pressed` | `#75000f` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.brand` | `#8c2224` | `same` | Brand fill for signature surfaces; carries text.on-brand (brandAnchor rule, DC-L01-09). |
| `color.bg.danger.bold` | `#d3403a` | `same` | Danger solid fill. |
| `color.bg.danger.bold-hover` | `#c13732` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.danger.bold-pressed` | `#b72c29` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.danger.subtle` | `#ffe6e3` | `same` | Danger banner and badge background. |
| `color.bg.disabled` | `#efebe8` | `same` | Disabled control fill. |
| `color.bg.field` | `#ffffff` | `same` | Text field fill: outlined fields sit on the raised surface (Q-form-01). |
| `color.bg.info.bold` | `#007cb7` | `same` | Info solid fill. |
| `color.bg.info.bold-hover` | `#0070a6` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.info.bold-pressed` | `#006799` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.info.subtle` | `#d9efff` | `same` | Info banner and badge background. |
| `color.bg.inverse` | `#272321` | `same` | Tooltips and toasts: the inverted surface. |
| `color.bg.neutral.subtle` | `#efebe8` | `same` | Secondary buttons, chips, hovered rows. |
| `color.bg.neutral.subtle-hover` | `#e5e5e5` | `same` | Hover: +1 step (DC-L01-17). |
| `color.bg.neutral.subtle-pressed` | `#dfd9d5` | `same` | Pressed or selected: +2 steps (DC-L01-17). |
| `color.bg.success.bold` | `#00883d` | `same` | Success solid fill. |
| `color.bg.success.bold-hover` | `#007b36` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.success.bold-pressed` | `#007132` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.success.subtle` | `#dbf1de` | `same` | Success banner and badge background. |
| `color.bg.warning.bold` | `#efb23b` | `same` | Warning solid fill. |
| `color.bg.warning.bold-hover` | `#dca333` | `same` | Hover: one step, at least 1.15:1 from the solid (DC-L01-17). |
| `color.bg.warning.bold-pressed` | `#d19924` | `same` | Pressed: at least 1.3:1 from the solid. |
| `color.bg.warning.subtle` | `#f5eada` | `same` | Warning banner and badge background. |
| `color.border.accent` | `#c66c67` | `same` | Selected card or accent outline. |
| `color.border.danger` | `#d2665c` | `same` | Danger boundary, for example an invalid field (3:1). |
| `color.border.default` | `#e5e5e5` | `same` | Outlines (soft borders). |
| `color.border.focus` | `#8c2224` | `same` | Focus ring (3:1 against every surface, DC-L04-09). |
| `color.border.info` | `#008ed1` | `same` | Info boundary, for example an invalid field (3:1). |
| `color.border.input` | `#8d857f` | `same` | Text field and select borders (3:1, DC-L01-16). |
| `color.border.separator` | `#efebe8` | `same` | Hairlines between table rows and list items, lighter than border.subtle; decorative, so never the only cue (DC-L23-05). |
| `color.border.strong` | `#8d857f` | `same` | Boundaries that are the only cue: inputs, checkboxes, switches (3:1, WCAG 1.4.11). |
| `color.border.subtle` | `#e5e5e5` | `same` | Dividers (soft borders: Warmth 67+, Linear 2026 S-L06-067). |
| `color.border.success` | `#28994e` | `same` | Success boundary, for example an invalid field (3:1). |
| `color.border.warning` | `#aa7f2e` | `same` | Warning boundary, for example an invalid field (3:1). |
| `color.icon.accent` | `#8c2224` | `same` | Selected and interactive icons. |
| `color.icon.default` | `#5e5651` | `same` | Icons beside text; same color as secondary text (DC-L05-08). |
| `color.icon.on-accent` | `#ffffff` | `same` | Icons on solid accent fills. |
| `color.icon.subtle` | `#6b635d` | `same` | Decorative icons. |
| `color.overlay.scrim` | `#272321 @0.45` | `same` | Modal backdrop (DC-L04-18; Q-depth-06). |
| `color.surface.base` | `#ffffff` | `same` | The page background. |
| `color.surface.nav` | `#ffffff` | `same` | Navigation on the page background. |
| `color.surface.overlay` | `#ffffff` | `same` | Menus, popovers, dialogs; always with elevation.floating or elevation.overlay. |
| `color.surface.raised` | `#ffffff` | `same` | Cards and panels on the page. |
| `color.surface.sunken` | `#f5f5f5` | `same` | Wells, code blocks, page gutters. |
| `color.surface.tinted` | `#fdf2f1` | `same` | Tinted container (Colorfulness 50+, L09 X rubric; Q-color-05). |
| `color.text.accent` | `#8c2224` | `same` | Accent text and selected labels. |
| `color.text.accent2` | `#6f5305` | `same` | accent2 text. |
| `color.text.accent3` | `#734776` | `same` | accent3 text. |
| `color.text.danger` | `#a22a26` | `same` | Danger text and icons; pair with an icon or label (DC-L01-15). |
| `color.text.disabled` | `#8d857f` | `same` | Disabled labels; exempt from contrast minimums (WCAG 1.4.3 exception). |
| `color.text.heading` | `#111111` | `same` | Added by a person (engine.py set). |
| `color.text.info` | `#005c8a` | `same` | Info text and icons; pair with an icon or label (DC-L01-15). |
| `color.text.inverse` | `#ffffff` | `same` | Text on color.bg.inverse (tooltips, toasts). |
| `color.text.link` | `#8c2224` | `same` | Links. Underline them in running text so color is not the only cue. |
| `color.text.on-accent` | `#ffffff` | `same` | Text and icons on color.bg.accent.bold* (auto-picked light or dark, S-L06-094). |
| `color.text.on-accent2` | `#ffffff` | `same` | Text on accent2 solid. |
| `color.text.on-accent3` | `#ffffff` | `same` | Text on accent3 solid. |
| `color.text.on-action` | `#ffffff` | `same` | Text on the primary action fill. |
| `color.text.on-brand` | `#e0e0e0` | `same` | Text on color.bg.brand. |
| `color.text.on-danger` | `#ffffff` | `same` | Text on bg.danger.bold. |
| `color.text.on-info` | `#ffffff` | `same` | Text on bg.info.bold. |
| `color.text.on-success` | `#ffffff` | `same` | Text on bg.success.bold. |
| `color.text.on-warning` | `#272321` | `same` | Text on bg.warning.bold. |
| `color.text.primary` | `#252525` | `same` | Body copy, headings, labels (guaranteed >= 7:1 on steps 1-5). |
| `color.text.secondary` | `#666666` | `same` | Supporting text (guaranteed >= the text minimum on surfaces and neutral fills 1-4). |
| `color.text.success` | `#00652c` | `same` | Success text and icons; pair with an icon or label (DC-L01-15). |
| `color.text.tertiary` | `#666666` | `same` | Captions and placeholders (still meets the text minimum on surfaces 1-4). |
| `color.text.warning` | `#845d00` | `same` | Warning text and icons; pair with an icon or label (DC-L01-15). |

**Use / avoid.**
- Use one solid accent fill per view for the primary action; spend chroma on small, meaningful elements.
- Avoid gray text on colored fills; use the matching `text.on-*` role.
- Avoid color as the only signal: pair status colors with an icon or label.
- Charts: no chart palette yet (Q-color-19). Take chart colors from the status and accent hues, and check them separately.

**Tailwind classes:** `bg-action-primary`, `hover:bg-action-primary-hover`, `active:bg-action-primary-pressed`, `text-on-action`, `bg-surface-base`, `bg-surface-raised`, `text-fg-primary`, `text-fg-secondary`, `text-fg-link`, `border-line-subtle`, `border-line-input`, `outline-line-focus`, `bg-danger-bold`.

Decisions: D-0042 (answers.Q-theme-01), D-0049 (raw.brandColor).

</details>

## Typography

> Zoom: sketch (0 of 3), 1 decision in this area. To zoom in, answer Q-type-01.
<!-- od:zoom area=typography level=0 -->

**Body text is 16px, and each larger size is about 1.25 times the one below.**
Designers: type scale: base size and ratio · Code: `font.size.14`

<details><summary>More</summary>

**Your answers here** (each one either sets tokens or is a rule for this section):
- Do you have the brand font files? **No** (chosen; asset status; Q-type-02)

**Intent.** Body text is 16px; sizes follow `round(16 x 1.25^n)` for n from -2 to 4, reaching about 2.5x body (product surfaces only). Sizes: 13, 16, 20, 25, 31, 39px.

- Text face: Be Vietnam Pro, system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif. Licence status (hook H-type): **open-library**. A system font needs no licence; it must not be embedded in apps.
- Licence by platform: text: system (open licence or system font: web, apps and self-hosting).
- On iOS the Swift file uses Dynamic Type text styles (body 17 pt), so text follows the person's text size setting; Compose uses sp, which follows the Android font scale.
- Weights: body 400, label 500, heading 650 (two or three distinct weights per view).
- Emphasized variants: off (they turn on at Expression 67 and up, DC-L02-11).
- Line heights snap to a 4px grid: 1.5 up to 17px, 1.4 to 26px, 1.25 to 44px, 1.12 above.
- Letter spacing: +0.02em at 11-12px, -0.01em from 32px, -0.02em from 48px.
- Text scaling: CSS sizes are rem, line heights unitless, so text scales to 200% (WCAG 1.4.4); containers must grow with it.
- Scripts: Latin only; add scripts in raw.scripts to get per-script line heights (DC-L02-25).

| Style | Size/line (px) | Weight | Tracking | Use |
|---|---|---|---|---|
| `text.body.lg` | 20/28 | 400 | 0em | Long-form reading, onboarding copy. |
| `text.body.md` | 16/24 | 400 | 0em | Default UI text: forms, tables, descriptions. |
| `text.body.sm` | 13/20 | 400 | 0em | Helper text, timestamps, captions. |
| `text.code.md` | 16/24 | 400 | 0em | Code blocks, token names. |
| `text.code.sm` | 13/20 | 400 | 0em | Inline values, dense code rows. |
| `text.headline.md` | 39/48 | 650 | -0.01em | Page and section titles. |
| `text.headline.sm` | 31/40 | 650 | 0em | Page and section titles. |
| `text.label.lg` | 16/24 | 500 | 0em | Button and control labels. |
| `text.label.md` | 13/20 | 500 | 0em | Small control labels, badges, dense tabs. |
| `text.label.sm` | 13/20 | 500 | 0.05em caps | Overlines in capitals with wide tracking (DC-L02-18). |
| `text.numeric.lg` | 25/36 | 650 | 0em | Key numbers: balances, KPIs. |
| `text.numeric.md` | 16/24 | 400 | 0em | Amounts and table figures: tabular digits line up in columns; right-align numeric columns. |
| `text.title.lg` | 25/36 | 650 | 0em | Card, panel and group titles. |
| `text.title.md` | 20/28 | 650 | 0em | Card, panel and group titles. |
| `text.title.sm` | 16/24 | 650 | 0em | Table headers, field-group titles. |

**Use / avoid.**
- Use at most three sizes and two weights in one view; let color and weight carry hierarchy before size.
- Avoid all caps for sentences and in scripts without case; use weight for emphasis there.

**Tailwind classes:** `text-body-md`, `text-label-lg`, `text-title-md`, `text-headline-md`.

Decisions: D-0047 (answers.Q-type-02).

</details>

## Layout

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-space-01, Q-space-02, Q-space-03.
<!-- od:zoom area=layout level=0 -->

**Spacing comes in steps of 4px, and screens use spacious spacing by default.**
Designers: spacing scale, 0 to 96 · Code: `space.0 to space.96`

<details><summary>More</summary>

**Intent.** Everything sits on a 4px unit: ladder 0, 2, 4, 6, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96. Density is a mode on the semantic layer (default **spacious**). Primitives and minimum tap areas never change.

| Density | inset xs/sm/md/lg/xl | section sm/md/lg | control sm/md/lg | row sm/md/lg/two-line | outer:inner |
|---|---|---|---|---|---|
| spacious (default) | 6 / 12 / 16 / 20 / 32 | 64 / 80 / 96 | 40 / 48 / 56 | 52 / 56 / 64 / 80 | 3.5 |
| comfortable | 4 / 8 / 12 / 16 / 24 | 32 / 40 / 64 | 32 / 40 / 48 | 44 / 48 / 56 / 72 | 2.5 |
| compact | 2 / 6 / 8 / 12 / 20 | 16 / 24 / 40 | 24 / 32 / 40 | 36 / 40 / 48 / 64 | 2.0 |

- Target sizes: pointer 24px, touch 44px; `size.target.min` is the floor for the primary input, and `space.target.gap` separates adjacent targets.
- Inner gaps stay below outer gaps (at least half), so grouping reads without borders (L15 P16).
- Breakpoints and grid: not generated yet; use the platform defaults and keep layout spacing independent of density (DC-L03-17).

**Use / avoid.**
- Parents own spacing (padding and gap); children never set outer margins.
- Avoid values off the ladder; if one is needed, add it as a decision.

Decisions: none recorded yet; values are defaults from references/levers.json.

</details>

## Elevation & Depth

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-depth-01.
<!-- od:zoom area=elevation level=0 -->

**Cards get a faint outline and a very soft shadow.**
Designers: flat, shadowed, tonal or glass · Code: `$extensions.opendesigner.model`

<details><summary>More</summary>

**Intent.** Depth 30/100 selects the **ring+faint-shadow** model. Shadow alpha in light mode is 0.107; dark mode doubles it and lifts surfaces by lightness instead (sunken, base, raised, overlay).

| Token | Layers (x y blur spread) | Use |
|---|---|---|
| `elevation.raised` | 0 0 0 1, 0 1 2 0 | Cards that lift on hover, sticky headers, dragged rows. |
| `elevation.floating` | 0 0 0 1, 0 1 2 0, 0 4 12 0 | Menus, popovers, dropdowns. |
| `elevation.overlay` | 0 0 0 1, 0 1 2 0, 0 12 32 0 | Dialogs and sheets (with color.overlay.scrim). |

- Borders: 1px default, 2px selected and focus, 4px emphasis; width changes use an inset shadow so layout does not jump.
- Stacking: page < raised < floating (menus) < overlay (dialogs with `color.overlay.scrim`).
- No materials or glass in this system.

Decisions: none recorded yet; values are defaults from references/levers.json.

</details>

## Shapes

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-shape-01.
<!-- od:zoom area=shape level=0 -->

**Buttons and fields have 16px corners; cards have 24px corners.**
Designers: corner radius, sharp to pill · Code: `radius.control, CSS border-radius`

<details><summary>More</summary>

**Intent.** Roundness 90/100 gives controls a **16** radius; details 8px, containers 24px, overlays 32px, people full. Controls under 32px tall use `radius.control-sm` (12).

- Nested radius: inner = max(outer - padding, smallest step). Here it is 4px inside a container with `space.inset.lg` padding. Equal radii on nested shapes look uneven (DC-L04-05).
- Focus ring: 2px, 2px offset, radius = control radius + offset (18).
- Icons: rounded corners, round caps.
- Corners (Q-shape-04, DC-L04-04): the radii are the same everywhere; iOS draws them continuous (`DS.Radius.shape(...)`, `.continuous`), Android circular (`RoundedCornerShape`), the web and Figma circular.
- Signature shapes: none generated; a brand shape library is a designer asset (hook H-motif).

Decisions: none recorded yet; values are defaults from references/levers.json.

</details>

## Components

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-comp-01, Q-comp-02, Q-state-01.
<!-- od:zoom area=components level=0 -->

**Version 1 plans 25 components, all built from these tokens.**
Designers: core set of about 25 components · Code: `button.* (proposed), APG pattern`

<details><summary>More</summary>

**Intent.** v1 components use the semantic tokens only. Base: not chosen yet (Q-comp-01). Buttons are 48px tall (spacious), 16 radius, `text.label.lg`; one primary action per view.

| Component | Status |
|---|---|
| button | planned (tokens ready) |
| text-field | planned (tokens ready) |
| textarea | planned (tokens ready) |
| select | planned (tokens ready) |
| checkbox | planned (tokens ready) |
| radio | planned (tokens ready) |
| switch | planned (tokens ready) |
| slider | planned (tokens ready) |
| tabs | planned (tokens ready) |
| tooltip | planned (tokens ready) |
| popover | planned (tokens ready) |
| dialog | planned (tokens ready) |
| menu | planned (tokens ready) |
| progress-bar | planned (tokens ready) |
| spinner | planned (tokens ready) |
| banner | planned (tokens ready) |
| badge | planned (tokens ready) |
| avatar | planned (tokens ready) |
| card | planned (tokens ready) |
| list | planned (tokens ready) |
| table | planned (tokens ready) |
| link | planned (tokens ready) |
| breadcrumbs | planned (tokens ready) |
| side-navigation | planned (tokens ready) |
| accordion | planned (tokens ready) |

**Contested policies:** Validation timing and disabled submit: pending; Field style: pending; Toasts: pending; Undo versus confirm: pending; Danger actions: pending; Button emphasis levels: pending.

**Use / avoid.**
- Every interactive component shows hover, pressed, focus-visible and disabled states from the tokens.
- Inputs keep a 3:1 boundary (`color.border.input`); signifier strength: minimal-allowed.
- Component docs belong in `opendesigner/components/<name>.md` (spec 7.8).

Decisions: none recorded yet; values are defaults from references/levers.json.

</details>

## Do's and Don'ts

**These rules keep screens clear and easy to read.** The engine checks the ones it can.
Designers: guardrails and design linting · Code: `engine.py validate, engine.py review`

<details><summary>More</summary>

**Enforced by construction.** The generator cannot break these:
- text contrast 4.5:1, and 3:1 for edges, in every mode
- text on colored fills picked automatically
- tap areas pointer 24px, touch 44px
- a 2px focus ring with a 2px offset
- a reduced-motion mode
- inner spacing smaller than outer spacing, three text colors, and nested radii

**Do**
- Use semantic tokens; never raw hex, px or ms values in components.
- Keep one primary action per view and at most three type sizes per view.
- Pair every status color with an icon or label; underline links in running text.

**Don't**
- Don't shrink hit areas in dense layouts; shrink visuals and extend the hit area.
- Don't use motion as the only signal, or flash more than three times a second.
- Don't copy another brand's identity from a reference (colors, typeface, logo, imagery, copy).

**Current validation findings:** none (errors 0, warnings 0).

**Waivers:** none.

</details>

## Standards

**Follow these rules when you build.** They come from sources marked non-negotiable, their values are locked, and `engine.py review` checks the ones it can.

House standards v3: 288 rules followed in this project; 1 overridden.

**Don't break these:**
- No motion on 100+ times-a-day actions (STD-when-to-animate-05).
- Never use ease-in on UI (STD-easing-duration-03).
- Never enter from scale(0) (STD-enter-exit-origin-01).
- Never use transition: all (STD-performance-properties-06).
- Never disable pinch zoom (STD-accessibility-motion-27).

**Overridden in this project**
- ~~Colors adapt to light and dark~~ Overridden in this project: "Chỉ giữ bảng màu sáng và bỏ chế độ tối cũ theo yêu cầu của chủ dự án." (D-0041). The house rule: Make interface colors adapt to light and dark mode: give each color role a light value and a dark value. (STD-visual-details-24).

<details><summary>Every theme (224 rules)</summary>

- **When to animate** (14 rules, 12 must): Decide whether to animate first; Name a valid purpose for every animation; Scale motion down as frequency rises; No motion on 100+ times-a-day actions; Never animate keyboard-initiated actions; Remove or shrink motion seen tens-of-times daily; Spend delight only on rare moments; Explanatory motion only in marketing, onboarding; and 4 more must rules. Locks `motion.duration.instant` 0ms.
- **Easing and duration** (12 rules, 10 must): Pick easing by the motion's job; Strong custom curves, not built-in keywords; Never use ease-in on UI; UI motion under 300ms unless justified; Duration budget for each element; Nothing over 1s unless illustrative; Duration grows with size and distance; Slow deliberate phase, snappy response; and 2 more must rules. Locks `motion.easing.linear` [0, 0, 1, 1], `motion.easing.hover` [0.25, 0.1, 0.25, 1], `motion.easing.enter` [0.23, 1, 0.32, 1], `motion.easing.exit` [0.23, 1, 0.32, 1], `motion.easing.standard` [0.77, 0, 0.175, 1], `motion.duration.micro` 100ms, `motion.duration.short` 150ms, `motion.duration.medium` 200ms, `motion.duration.long` 250ms.
- **Enter, exit and origin** (29 rules, 16 must): Never enter from scale(0); No opacity-only fade entrances; Scale popovers from their trigger; Keep modals scaling from center; Exit the way it entered; Dropdowns and popovers: scale 0.95, 200ms; Tooltips: scale 0.97, 125ms; Delay only the first tooltip; and 8 more must rules. Locks `motion.scale.enter` 0.95, `motion.duration.medium` 200ms (STD-easing-duration-07 wins), `motion.duration.tooltip` 125ms, `motion.scale.enter-tooltip` 0.97, `motion.duration.instant` 0ms (STD-when-to-animate-05 wins), `motion.duration.modal` 250ms, `motion.scale.enter-modal` 0.96, `motion.duration.stagger` 50ms, `motion.duration.reveal` 600ms, `motion.blur.crossfade` 2px, `motion.easing.drawer` [0.32, 0.72, 0, 1], `motion.duration.drawer` 500ms.
- **Springs and gestures** (32 rules, 21 must): Springs for anything a finger drives; Default springs are critically damped; Bounce only after a momentum gesture; Keep bounce subtle, 0.1 to 0.3; Sheet and drawer spring values; Every animation can be grabbed mid-flight; Never block input during transitions; Start from the on-screen value; and 13 more must rules. Locks `motion.spring.spatial.dampingRatio` 1.0, `motion.spring.spatial.stiffness` 246.7, `motion.spring.momentum` a composite value (see standards.md), `motion.spring.sheet` a composite value (see standards.md), `motion.spring.rotation` a composite value (see standards.md), `motion.gesture.deceleration-rate` 0.998, `motion.gesture.dismiss-velocity` 0.11, `motion.gesture.rubberband-constant` 0.55, `motion.gesture.direction-threshold` 10px.
- **Performance and properties** (14 rules, 9 must): Animate only transform and opacity; Only clip-path, accordion height, childless width; Never use transition: all; Motion: animate the full transform string; Keep per-frame values out of React state; Set drag transforms on the moving element; Pick the cheapest animation tool; Treat dropped frames as a regression; and 1 more must rule.
- **Accessibility in motion** (18 rules, 11 must): Ship reduced motion with the animation; Reduced motion is gentler, never zero; Check reduced motion by toggling it; Reduced transparency makes surfaces solid; Increased contrast gets solid, bordered surfaces; Scale layout with the user's text size; Gate hover motion to fine pointers; Build overlays on accessible primitives; and 3 more must rules. Locks `raw.reducedMotion` "replace", `motion.duration.reduced-fade` 200ms, `reduced:motion.transition.enter` a composite value (see standards.md), `reduced:motion.transition.exit` a composite value (see standards.md), `reduced:motion.transition.expand` a composite value (see standards.md).
- **Toasts, drawers and overlays** (23 rules, 7 must): Fill gaps between toasts for hover; Pause toast timers in a hidden tab; Toast classNames need !important; Copy Sonner styles into shadow DOM; Drawer curve: cubic-bezier(0.32, 0.72, 0, 1); Feedback on press, commit on release; Hold to confirm: slow press, fast release. Locks `motion.duration.toast` 400ms, `motion.easing.toast` [0.25, 0.1, 0.25, 1], `component.toast.gap` 14px, `component.toast.visible` 3, `component.toast.duration` 4000ms, `component.toast.offset.desktop` 32px, `component.toast.offset.mobile` 16px, `motion.easing.drawer` [0.32, 0.72, 0, 1] (STD-enter-exit-origin-41 wins), `motion.gesture.drag-lock-after-scroll` 100ms.
- **Mobile and touch** (20 rules, 16 must): Detect touch by capability, never by device; Remove the tap highlight flash globally; Press feedback scales to 0.97, briefly; Remove the tap delay on tappables; Touch targets 44pt on iOS, 48dp on Android; Size full-height layouts with dvh and svh; Form inputs at 16px or larger; Contain overscroll in app layouts; and 8 more must rules. Locks `motion.scale.press` 0.97, `motion.duration.micro` 100ms (STD-easing-duration-07 wins), `size.target.touch` 44px, `size.target.min` 44px, `font.size.input` 16px.
- **Visual details** (48 rules, 19 must): Cap body text near 65ch; Tabular digits for changing numbers; Use the ellipsis character; Loosen tracking on uppercase labels; Make letter-spacing specific to size; Reserve underlines for links; Metric-matched fallback font stack; Never stack light translucent surfaces; and 11 more must rules.
- **Process, review and taste** (14 rules, 8 must): Motion that merely runs is not done; Self-check motion before finishing; Report review findings as one table; Close every motion review with Block or Approve; Make the motion call yourself; Keep the motion note to a few lines; Say when feel can't be judged from code; Judge feel on real hardware.

</details>

Every rule, with its values, reasons and sources: `opendesigner/standards.md` (it also has the 64 rules this file leaves out). Read the themes you touch before you build.

## Motion

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-motion-01.
<!-- od:zoom area=motion level=0 -->

**Most movements take 200ms.** They turn into fades when a person asks for less motion.
Designers: motion system: duration, easing, springs · Code: `motion.duration.*, motion.easing.*`

<details><summary>More</summary>

**Intent.** Energy 55/100: the duration multiplier x1.02 scales the extra step (standards fix medium, long). Standard easing `cubic-bezier(0.77, 0, 0.175, 1)`, enter `cubic-bezier(0.23, 1, 0.32, 1)`, exit `cubic-bezier(0.23, 1, 0.32, 1)`. Spatial spring: damping 1.0, stiffness 246.7 (Apple duration 0.4s, bounce 0.0; web `linear()` sample over 590ms).

| Token | Value | Note |
|---|---|---|
| `motion.duration.instant` | 0ms | set by house standard STD-when-to-animate-05 |
| `motion.duration.micro` | 100ms | set by house standard STD-easing-duration-07 |
| `motion.duration.short` | 150ms | set by house standard STD-easing-duration-07 |
| `motion.duration.medium` | 200ms | set by house standard STD-easing-duration-07 |
| `motion.duration.long` | 250ms | set by house standard STD-easing-duration-07 |
| `motion.duration.extra` | 710ms | illustrative and marketing motion only, never UI (STD-easing-duration-06) |
| `motion.duration.medium-exit` | 160ms | derived: about 0.8 x medium |
| `motion.duration.long-exit` | 200ms | derived: about 0.8 x long |
| `motion.duration.drawer` | 500ms | set by house standard STD-enter-exit-origin-41 |
| `motion.duration.modal` | 250ms | set by house standard STD-enter-exit-origin-11 |
| `motion.duration.reduced-fade` | 200ms | set by house standard STD-accessibility-motion-02 |
| `motion.duration.reveal` | 600ms | set by house standard STD-enter-exit-origin-26 |
| `motion.duration.stagger` | 50ms | set by house standard STD-enter-exit-origin-13 |
| `motion.duration.toast` | 400ms | set by house standard STD-components-toasts-drawers-07 |
| `motion.duration.tooltip` | 125ms | set by house standard STD-enter-exit-origin-09 |

- Exits are derived, not set on their own: each is about 20% shorter than the entrance in force (medium-exit 160ms from medium 200ms, long-exit 200ms from long 250ms; STD-easing-duration-11). Change an entrance and its exit follows. Linear easing only for spinners and progress.
- Reduced motion (`prefers-reduced-motion` or `data-motion="reduced"`): travel becomes opacity, feedback stays, `motion.transition.move` is 0ms.
- Springs are stored as damping and stiffness in `$extensions.opendesigner.spring` because DTCG 2025.10 has no spring type.
- Haptics: medium intensity where the platform has them; sound: hook H-sound is pending.

Decisions: D-0002 (34 values, standards).

</details>

## Modes and Themes

> Zoom: defined (2 of 3), 1 decision in this area. To zoom in, answer Q-theme-02, Q-theme-04.
<!-- od:zoom area=modes level=2 -->

**The system has one color mode, three spacing densities and a reduced-motion mode.**
Designers: modes: light, dark, density, motion · Code: `resolver modifiers, Figma collection modes`

<details><summary>More</summary>

**Your answers here** (each one either sets tokens or is a rule for this section):
- Should the app have light and dark modes that follow the device, or just one mode? **Light only** (chosen; tokens; Q-theme-01)

**Intent.** Modes live in the DTCG resolver (`opendesigner/tokens/opendesigner.resolver.json`); modifiers are orthogonal, so no two set the same token.

| Modifier | Contexts | Default |
|---|---|---|
| density | spacious, comfortable, compact | spacious |
| motion | standard, reduced | standard |

- Web: `prefers-color-scheme` with a `[data-theme]` override; `[data-density]`; `prefers-reduced-motion` with `[data-motion]` (see `opendesigner/build/css/tokens.css`).
- High-contrast themes are not generated; set `raw.contrastTarget` to AAA for 7:1 text everywhere.
- A second brand or a client re-skin may override the color primitives and `color.bg.brand`; semantic names never change.

Decisions: D-0042 (answers.Q-theme-01).

</details>

## Iconography and Imagery

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-icon-01, Q-icon-02, Q-icon-06.
<!-- od:zoom area=iconography level=0 -->

**Icons are 24px by default.** The logo, photos and custom icons come from a person, not from the engine.
Designers: icon system: style, sizes, color · Code: `size.icon.*, icon.stroke.*, color.icon.*`

<details><summary>More</summary>

**Intent.** Default icon size 24px; sizes 16/20/24 pair with 14/16/20px text. Stroke follows the label weight: 1.5px at 16, 2.0px at 20, 2.5px at 24. Rest style: outline.

| Asset | Hook | Status |
|---|---|---|
| Logo and marks | H-logo | pending |
| Favicon set | H-favicon | pending |
| App icon | H-appicon | pending |
| Custom icons | H-icons | pending |
| Illustration | H-illus | pending |
| Photography | H-photo | pending |
| Motifs and brand shapes | H-motif | pending |

- Placeholders are labelled as placeholders. A generated stand-in is never shown as a finished brand asset.
- Icon-only buttons need an accessible name and a hit area of `size.target.min`.

Decisions: none recorded yet; values are defaults from references/levers.json.

</details>

## Content and Voice

> Zoom: sketch (0 of 3), 0 decisions in this area. To zoom in, answer Q-voice-01, Q-voice-02, Q-voice-03.
<!-- od:zoom area=content level=0 -->

**Words stay plain and short, and every button says what it does.**
Designers: content: voice, tone, microcopy · Code: `DESIGN.md Content and Voice section`

<details><summary>More</summary>

**Intent.** Draft: voice guidance level **full** (Brand presence 80); **sentence-case**; contractions **encouraged** (Warmth 80). Voice guide hook H-voice: pending.

- Buttons say what they do in two to four words; errors say what happened and how to fix it.
- Reading level: plain language; avoid jargon in UI copy.
- Word list: not recorded yet (Q-voice-03).

Decisions: none recorded yet; values are defaults from references/levers.json.

</details>

## Accessibility

> Zoom: sketch (0 of 3), 1 decision in this area. To zoom in, answer Q-aud-03, Q-aud-04.
<!-- od:zoom area=accessibility level=0 -->

**Text passes WCAG 2.2 AA contrast in every mode, and focus is always visible.**
Designers: WCAG 2.2 AA target · Code: `raw.contrastTarget`

<details><summary>More</summary>

**Your answers here** (each one either sets tokens or is a rule for this section):
- Who uses it, and how often: all day for work, often, or now and then on the go? **Now and then, on a phone or in public** (chosen; tokens; Q-aud-01)
- What's at stake for your users, and how do they usually feel when they use it? **Apps for everyday life** (research; owner input; Q-aud-02)

**Intent.** Standard: WCAG 2.2 AA. APCA is reported as advice only.

**The system guarantees:**
- text and edge contrast in every mode
- visible focus (2px ring, 2px offset, 3:1)
- minimum target sizes for each kind of input
- a reduced-motion mode
- rem-based type, so text scales to 200%
- text on colored fills chosen automatically

**Product teams own:** accessible names and labels, alt text, reading and focus order, and never using color alone. Also: clear error messages, dialogs that can be closed, no pre-checked consent boxes, and captions for media.

**Test on each platform:**
- keyboard only
- a screen reader (VoiceOver, NVDA or TalkBack)
- 200% zoom
- forced colors (Windows High Contrast)
- reduced motion
- touch on a phone, for every surface that allows touch

Decisions: D-0023 (answers.Q-aud-02).

</details>

## Platforms and Devices

> Zoom: sketch (0 of 3), 1 decision in this area. To zoom in, answer Q-plat-05, Q-plat-10, Q-plat-08.
<!-- od:zoom area=platforms level=0 -->

**It runs on web, and each platform keeps its own navigation.**
Designers: target platforms · Code: `raw.platforms; size.target.min`

<details><summary>More</summary>

**Your answers here** (each one either sets tokens or is a rule for this section):
- Where will it run first: web, iOS, Android or desktop? **Web** (chosen; tokens; Q-plat-01)

**Intent.** Platforms: web. Inputs: pointer, touch. Brand presence 80: each platform keeps its own shapes and materials: no; each platform keeps its own body text size: no.

- Navigation, back, sheets and pickers stay native on every platform (DC-L10-02).
- Swift and Compose files in `opendesigner/build/` use the same names as the CSS variables (Figma code syntax matches them).
- Fonts by platform: text: system (open licence or system font: web, apps and self-hosting).

Decisions: D-0012 (answers.Q-plat-01).

</details>

## Decisions

**63 decisions so far.** Each one says who set it and why.
Designers: decision history with reasons · Code: `opendesigner/decisions.md`

<details><summary>More</summary>

Your own decisions first (the newest value per path), then your changes to standards, then one row per standards batch. Full log: `opendesigner/decisions.md`.

| Id | Path | Value | Set by | Reason |
|---|---|---|---|---|
| D-0006 | `answers.Q-scope-07` | "building" | assumed | the handoff describes an in-progress team project |
| D-0008 | `context.market.analogous` | "Popeyes" | reference | named in the handoff as ordering-flow inspiration; identity must not be copied |
| D-0009 | `answers.Q-aud-01` | "large" | chosen | sketch: Level 0 answer |
| D-0010 | `context.audience` | "people who use it now and then, often on a phone" | assumed | sketch: plain words for Q-aud-01 |
| D-0012 | `answers.Q-plat-01` | ["web"] | chosen | sketch: Level 0 answer |
| D-0013 | `raw.stack` | ["html", "css", "vanilla-js"] | chosen | sketch: the code stack the person named |
| D-0014 | `macros` | ["friendly", "bold", "playful"] | chosen | sketch: Level 0 answer (their words: friendly, bold, energetic) |
| D-0015 | `taste.feelWords` | ["friendly", "bold", "energetic"] | chosen | sketch: the person's own feel words |
| D-0016 | `answers.Q-scope-06` | ["website:operate"] | chosen | sketch: Level 0 answer |
| D-0023 | `answers.Q-aud-02` | "consumer" | research | user research (F1, F2, F4): an everyday consumer product |
| D-0024 | `profile.library` | "declined" | chosen | the owner chose to build the food UI from scratch |
| D-0025 | `size.content.max` | {"value": 1312, "unit": "px"} | chosen | maximum width for Maika storefront and admin pages |
| D-0026 | `size.dialog.product.max` | {"value": 832, "unit": "px"} | chosen | maximum width for the product detail dialog |
| D-0027 | `size.dialog.form.max` | {"value": 480, "unit": "px"} | chosen | maximum width for compact confirmation and form dialogs |
| D-0028 | `size.dialog.max-block` | {"value": 896, "unit": "px"} | chosen | maximum dialog height before internal scrolling |
| D-0029 | `size.auth.max` | {"value": 544, "unit": "px"} | chosen | comfortable reading width for the account form |
| D-0030 | `size.review.list.max` | {"value": 320, "unit": "px"} | chosen | limit the review list height inside the product dialog |
| D-0031 | `size.toast.max` | {"value": 384, "unit": "px"} | chosen | keep confirmation messages readable |
| D-0032 | `size.cart.column.min` | {"value": 320, "unit": "px"} | chosen | minimum checkout column width before stacking |
| D-0033 | `size.detail.image.max` | {"value": 288, "unit": "px"} | chosen | bound the product image in a narrow dialog |
| D-0034 | `size.quantity.field` | {"value": 80, "unit": "px"} | chosen | comfortable width for a quantity input |
| D-0035 | `size.table.product.min` | {"value": 208, "unit": "px"} | chosen | keep product table names legible |
| D-0036 | `size.status.max` | {"value": 192, "unit": "px"} | chosen | allow order status labels to fit |
| D-0037 | `size.preview.max` | {"value": 352, "unit": "px"} | chosen | bound the uploaded image preview |
| D-0038 | `size.admin.sidebar.min` | {"value": 192, "unit": "px"} | chosen | minimum width for management navigation |
| D-0039 | `size.admin.sidebar.max` | {"value": 240, "unit": "px"} | chosen | maximum width for management navigation |
| D-0040 | `size.product.mobile.image.min` | {"value": 112, "unit": "px"} | chosen | keep menu photography visible beside mobile product details |
| D-0042 | `answers.Q-theme-01` | "light-only" | chosen | The owner requested a light-only Maika interface and asked to remove the previous dark palette. |
| D-0043 | `name` | "Kat" | chosen | The owner renamed the snack shop to Kat. |
| D-0044 | `context.product` | "a snack food ordering website for Kat" | chosen | The owner confirmed the product direction is a snack shop and renamed it Kat. |
| D-0045 | `context.purpose` | "help people browse Kat's snack menu and place delivery or pickup orders" | chosen | The owner confirmed the snack shop direction and the Kat name. |
| D-0046 | `font.family.text` | ["Be Vietnam Pro", "system-ui", "-apple-system", "Segoe UI", "Roboto", "Helvetica Neue", "Arial", "sans-serif"] | chosen | Use a Vietnamese-ready open sans for clarity and warmth while keeping Popeyes' restricted Chicken Sans out of Kat. |
| D-0047 | `answers.Q-type-02` | "no" | chosen | Use the open Be Vietnam Pro font for Kat rather than a private brand font or owner-supplied asset. |
| D-0048 | `context.goals` | ["let customers browse and build a cart as guests, then sign in before checkout with account details prefilled", "let customers manage their cart, vouchers and reviews", "let admins manage products, orders, vouchers and reviews"] | chosen | The evaluation record requires sign-in before checkout; keep guest browsing and cart access. |
| D-0049 | `raw.brandColor` | "#8C2224" | chosen | Use the original Maika burgundy palette as requested: #8C2224 for Kat primary brand and actions. |
| D-0050 | `color.accent.light.10` | {"colorSpace": "srgb", "components": [0.4314, 0.1059, 0.1098], "hex": "#6e1b1c"} | chosen | Use the original Maika palette requested by the owner. |
| D-0051 | `color.accent.light.11` | {"colorSpace": "srgb", "components": [0.549, 0.1333, 0.1412], "hex": "#8c2224"} | chosen | Use the original Maika palette requested by the owner. |
| D-0052 | `color.neutral.light.4` | {"colorSpace": "srgb", "components": [0.898, 0.898, 0.898], "hex": "#e5e5e5"} | chosen | Use the original Maika palette requested by the owner. |
| D-0053 | `light:color.surface.base` | {"colorSpace": "srgb", "components": [1.0, 1.0, 1.0], "hex": "#ffffff"} | chosen | Use the original Maika palette requested by the owner. |
| D-0054 | `light:color.surface.nav` | {"colorSpace": "srgb", "components": [1.0, 1.0, 1.0], "hex": "#ffffff"} | chosen | Use the original Maika palette requested by the owner. |

12 more in the full log.

</details>

## Open Items

**These parts are still defaults, guesses, or waiting for a person.**

- Still defaults (zoom 0, sketch): Colors, Typography, Layout, Elevation & Depth, Shapes, Components, Motion, Iconography and Imagery, Content and Voice, Accessibility, Platforms and Devices
- Assets not final: Logo, wordmark, symbol, lockups (H-logo): pending; App icon (H-appicon): pending; Favicon set (H-favicon): pending; Custom icons, pictograms, spot icons (H-icons): pending; Illustration, characters, empty-state art (H-illus): pending; Photography and art direction (H-photo): pending; Fixed brand colors (H-color): pending; Motion signature and rich media (H-motion): pending; Graphic devices, patterns, textures, brand gradients, signature shape (H-motif): pending; UI sounds and sonic logo (H-sound): pending; Custom haptic patterns (H-haptic): pending; Voice and tone guide (H-voice): pending; Brand guidelines PDF (H-brandbook): pending
- Answers taken on assumption or delegated: answers.Q-scope-07 (assumed), context.audience (assumed)
- Waivers: none.
- Licence risks: none found.
- Validation: 0 errors, 0 warnings.

## For Agents

**AI agents: read this file and the tokens before you change any screen.**

1. Before any visual work, read this file, PRODUCT.md and `opendesigner/tokens/` (start at `opendesigner/tokens/opendesigner.resolver.json`).
2. Use tokens, never raw values: CSS `var(--ds-...)`, Tailwind classes from `opendesigner/build/tailwind/theme.css`, `DS.*` in Swift. In Compose: colors from `LocalDsColors.current` (provide `DsLightColors` or `DsDarkColors`), then `DsSpace`, `DsType` and `DsMotion`.
3. Do not change a locked decision without asking the owner. Keep new screens inside the taste card at the top of the Overview, and never add anything on its Never list without asking.
4. To change the system: `engine.py set <path> <value> --why "..."`, then `engine.py generate`, `engine.py validate`, `engine.py design-md`.
5. To extend: add a decision (never hand-edit tokens or this file). Keep semantic names the same across modes. Deprecate instead of deleting.
6. After any implementation, run `engine.py review` and re-read this file.
7. Follow the Standards section. Change a standard only when the person explicitly asks: `engine.py standard override <id> --why "<their words>"`.

**Tailwind v4 classes** (one import: `@import "tailwindcss"; @import "<path>/opendesigner/build/tailwind/theme.css";`; Tailwind's default colors, text sizes, radii and shadows are switched off, so only these exist):

| Area | Classes |
|---|---|
| Color | `bg-action-primary`, `hover:bg-action-primary-hover`, `active:bg-action-primary-pressed`, `text-on-action`, `bg-surface-base`, `bg-surface-raised`, `text-fg-primary`, `text-fg-secondary`, `text-fg-link`, `border-line-subtle`, `border-line-input`, `outline-line-focus`, `bg-danger-bold` |
| Layout | `p-inset-md`, `gap-stack-md`, `gap-inline-sm`, `h-control-md`, `size-icon-md`, `min-h-target-min` |
| Shape | `rounded-control`, `rounded-container`, `rounded-overlay`, `rounded-full` |
| Elevation | `shadow-raised`, `shadow-floating`, `shadow-overlay` |
| Type | `text-body-md`, `text-label-lg`, `text-title-md`, `text-headline-md` |
| Motion | `transition-feedback`, `ease-enter`, `ease-exit`, `ease-hover` |
