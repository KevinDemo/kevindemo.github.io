---
name: Kevin Chen
description: Freelance homepage of a Sydney .NET and SQL Server engineer. Measured work, fixed prices, hairline precision.
colors:
  accent-light: "#0A6B4A"
  accent-dark: "#3FCF8E"
  ground-light: "#F6F6F4"
  surface-light: "#FFFFFF"
  surface-raised-light: "#FBFBF9"
  line-light: "#E2E2DE"
  line-strong-light: "#C9C9C4"
  ink-light: "#101113"
  ink-secondary-light: "#4F5257"
  ink-tertiary-light: "#66696E"
  meter-light: "#85888D"
  segment-light: "#E2E2DE"
  close-ground-light: "#101113"
  close-ink-light: "#F4F4F2"
  close-ink-secondary-light: "#AEB1B6"
  close-line-light: "#2A2C30"
  ground-dark: "#0A0B0C"
  surface-dark: "#111315"
  surface-raised-dark: "#16181B"
  line-dark: "#232529"
  line-strong-dark: "#383B40"
  ink-dark: "#EDEEF0"
  ink-secondary-dark: "#A6A9AF"
  ink-tertiary-dark: "#8E9299"
  meter-dark: "#6E7177"
  segment-dark: "#2A2D31"
  close-ground-dark: "#15171A"
  close-ink-dark: "#EDEEF0"
  close-ink-secondary-dark: "#A6A9AF"
  close-line-dark: "#2B2E33"
typography:
  display:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "5.96rem"
    fontWeight: 560
    lineHeight: 1
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "3.815rem"
    fontWeight: 560
    lineHeight: 1.05
    letterSpacing: "-0.035em"
  figure:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "3.052rem"
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: "-0.035em"
  heading:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "2.441rem"
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "1.563rem"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "-0.02em"
  lead:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Geist, ui-sans-serif, system-ui, Segoe UI, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Geist Mono, ui-monospace, Consolas, Menlo, monospace"
    fontSize: "0.8rem"
    fontWeight: 400
    lineHeight: 1.4
  micro:
    fontFamily: "Geist Mono, ui-monospace, Consolas, Menlo, monospace"
    fontSize: "0.64rem"
    fontWeight: 500
    lineHeight: 1
rounded:
  sm: "2px"
  md: "4px"
spacing:
  s-1: "4px"
  s-2: "8px"
  s-3: "12px"
  s-4: "16px"
  s-5: "20px"
  s-6: "24px"
  s-8: "32px"
  s-10: "40px"
  s-12: "48px"
  s-16: "64px"
  s-20: "80px"
  s-24: "96px"
  s-32: "128px"
  s-40: "160px"
components:
  button-primary-light:
    backgroundColor: "{colors.ink-light}"
    textColor: "{colors.surface-light}"
    rounded: "{rounded.md}"
    padding: "0 24px"
    height: "48px"
  button-primary-dark:
    backgroundColor: "{colors.ink-dark}"
    textColor: "{colors.ground-dark}"
    rounded: "{rounded.md}"
    padding: "0 24px"
    height: "48px"
  panel-light:
    backgroundColor: "{colors.surface-light}"
    rounded: "{rounded.md}"
  panel-dark:
    backgroundColor: "{colors.surface-dark}"
    rounded: "{rounded.md}"
---

# Design System: Kevin Chen

## Overview

**Creative North Star: "The Measured Sheet"**

The page behaves like a well-kept engineering record: a ruled sheet where every line sits on the grid and every claim has a number beside it. The buyer is a small or mid-size business owner who has been burned by vague software work, and what persuades them is precision they can check, so the design spends its ambition on exactness rather than on decoration. It is calm and confident, it has a lot of air, and the only moving part of any consequence is a measurement.

Two product sites anchor the look, and principles were taken from them, never assets, logos or layouts.

**Anchor 1, Vercel (vercel.com).** Taken: a precise sans with tight tracking on large headlines, a mono voice for small labels and numbers, a near-monochrome palette, hairline 1px borders and visible grid lines, crisp near-square panels, a calm hero, and light and dark versions that are each designed.

**Anchor 2, Linear (linear.app).** Taken: dark surfaces that gain elevation from slightly lighter panels rather than shadows, muted secondary text, one very restrained accent, generous spacing, polished section rhythm, and product-style feature blocks in place of generic cards.

**Key Characteristics:**
- Vertical rails and full-width hairlines make the grid itself the visible structure.
- Geist at tight tracking for statements, Geist Mono for data and quiet labels.
- One green accent, reserved for one meaning: delivered and measured.
- Light and dark are two tuned palettes, and the closing section behaves differently in each.

## Hard Rules

These are binding on all code in this repo.

- **No purple, violet or blue-to-purple gradients anywhere. No decorative gradients at all unless one is clearly justified.** This page currently has zero gradients.
- **No overly rounded cards: corner radius at most 4px on cards, panels and buttons (pills only for tiny status tags, if at all).** This page has no pills.
- **More whitespace: section padding and spacing are larger than the previous site, with at least one generous breathing space between every major section, and body measure around 60 to 72 characters.**
- One accent colour at most, used sparingly; neutral palette otherwise. Text contrast is WCAG AA or better in light and dark mode.
- A clear type scale with named steps and a stated ratio, and at most two typefaces plus an optional mono for labels. This page uses Geist plus Geist Mono, both OFL.
- A spacing scale on a 4px base, used consistently.
- The usual AI tells are banned: Inter-only, purple gradients, glassmorphism, three identical cards in a row, emoji icons, generic stock phrases.
- Theme has exactly three options: System (default), Light, Dark. All colours come from CSS custom properties. Without JavaScript the page still follows the system setting.

## Colors

Near-monochrome neutrals with very slight warmth in light mode and very slight coolness in dark mode, plus a single green.

### Primary
- **Verified Green** (`accent-light`, `accent-dark`): the Delivered dot and the After bar in a measurement. It always means "this was delivered and measured". It darkens in light mode and brightens in dark mode, tuned separately rather than inverted.

### Neutral
- **Stone Ground / Carbon Ground** (`ground-*`): the page itself.
- **Sheet / Raised Carbon** (`surface-*`): panels and case cells. In light mode a panel is white on stone, in dark mode a slightly lighter carbon on near-black, so depth reads as tone in both.
- **Hairline** (`line-*`): every rule and grid line. **Strong Hairline** (`line-strong-*`): underlines and ghost button edges.
- **Ink** (`ink-*`), **Secondary Ink** (`ink-secondary-*`), **Tertiary Ink** (`ink-tertiary-*`): statements, supporting prose, and small labels.
- **Meter Grey** (`meter-*`): the Before bar. It clears 3:1 against its surface.
- **Close** (`close-*`): the contact section's own set.

### Named Rules
**The One Meaning Rule.** Green means delivered and measured. It never colours a button, a link at rest, a heading or a background field.

**The Two Sheets Rule.** Dark is not light inverted. Dark uses a lighter display weight and lifts panels by tone. Light closes the page on a solid ink block, dark closes on a raised carbon band.

## Typography

**Display and Body Font:** Geist (with ui-sans-serif, system-ui, Segoe UI fallback)
**Label/Mono Font:** Geist Mono (with ui-monospace, Consolas, Menlo fallback)

**Character:** Geist is exact without being cold, and tight tracking lets large statements read as one shape. Geist Mono only speaks for data and quiet labels, in sentence case, so the page never shouts in tracked capitals.

### Hierarchy
The scale has a ratio of 1.25 (major third) from a 16px base, and skips steps on purpose so that each role is clearly distinct.
- **Display** (95.4px at the top end, fluid): the hero statement and the closing statement.
- **Headline** (61px at the top end, fluid): section titles and the contact email.
- **Figure** (48.8px at the top end, fluid): measured results such as test counts.
- **Heading** (39px at the top end, fluid): scale numbers under the hero.
- **Title** (25px): prices.
- **Lead** (20px): hero and contact intro, and item titles.
- **Body** (16px, line height 1.6): all prose, held to 34rem, which is about 72 characters of Geist. Use rem rather than `ch` for this measure, because `0` is wider than the average letter in Geist and 68ch came out at 88 characters.
- **Label** (12.8px): mono for data labels and the status tag, sans for controls such as navigation, the switcher and contact links.
- **Micro** (10.2px, one step below Label): the two letters in the logo mark, and nothing else.

Dark mode sets Display and Headline at weight 500 and light mode at 560, because light text on dark blooms optically.

### Named Rules
**The No Kicker Rule.** No small label sits above a heading. The role line lives at the head of the summary panel, where it titles the panel rather than announcing the statement, and the status tag sits beside a case title rather than above it.

**The Tracking Floor Rule.** Tracking never goes tighter than -0.04em.

## Layout

The page is a sheet 1280px wide. Above 81rem, two 1px rails mark its edges from header to footer, and full-width hairlines separate sections, so the grid is visible. Page gutters run from 20px to 40px. Grids of cells bleed to the rails, so their dividers join the page structure.

Section padding is 96px to 160px, up from 48px to 88px on the previous site, and it applies above and below a section's content. Section bodies alternate pacing: a sticky title on the left with rows on the right (Rate card, Experience), then a title on top with a full-width grid (Work, How I work).

The hero's summary panel fills the last five of the sheet's twelve columns and joins the right rail and the scale row beneath it, so the numbers arrive inside the first viewport on a 1440 by 900 screen.

Work uses cells of unequal width on 12 columns, 12 then 7 and 5 then 5 and 7 then 12, so no row is a set of identical cards. Neighbouring cells share rows and columns through subgrid, so figures and text line up across the sheet. How I work is a 2 by 2 grid, which keeps its text near the target measure. Below 64rem the case and hero grids become a single column. The page holds from 360px upward, and the header stops being sticky below 48rem to protect reading height.

## Elevation & Depth

No shadows anywhere. Depth comes from tone: ground, then surface, then raised surface, separated by hairlines. Hover raises a case cell one tonal step.

**The No Shadow Rule.** If something needs to look lifted, it gets a lighter or whiter surface and a hairline, never a `box-shadow`.

## Shapes

Crisp and near-square. Panels, buttons and the switcher are 4px, inner segments and the logo mark are 2px to 4px, and grid cells are square because they sit in the ruled sheet. The only circle is the 6px status dot.

## Components

### Buttons
- **Shape:** near-square (4px), 48px tall.
- **Primary:** solid ink with ground-coloured text, never the accent.
- **Hover / Focus:** hover drops to secondary ink. Focus is a 2px ink ring offset by 2px.
- **Ghost:** transparent with a strong hairline. Hover raises the surface.

### Theme Switcher
Three native radio inputs in a fieldset, labelled System, Light and Dark, in Label type. Arrow keys move between them natively. The selected segment takes a filled neutral and full ink, and focus is a visible ring. It is hidden when JavaScript is off, because the page then follows the system by itself.

### Status Tag
A 6px accent dot and the word Delivered in mono. It has no border and no pill.

### Case Cell
A square cell on the ruled grid, with a surface fill and 48px of padding at the top end. The whole cell is the link, through the title's stretched hit area. A secondary link, such as Live demo, sits above it.

### Measurement
A caption, then Before and After rows with a key, an 8px square-ended bar and a tabular mono value. When the block is first seen, the After bar shrinks once from the Before length to its measured length, on a timer rather than tied to scroll position.

**The True At Rest Rule.** A bar must never rest at a false length. Scroll-scrubbed animation was tried and removed because a reader who stopped scrolling saw "6" beside a long bar. The markup carries the true width, so no JavaScript, reduced motion or printing all show the real value.

### Summary Panel
Titled by the role line, holding a definition list of mono labels and body values on ruled rows. On wide screens it is a square cell joined to the rail, and below 64rem it is a 4px panel with a hairline.

### Navigation
Sans Label type in secondary ink. Hover goes to full ink. Targets are 44px tall. The header is solid ground with a bottom hairline, with no blur.

## Do's and Don'ts

### Do:
- **Do** take every spacing value from the 4px scale in the frontmatter.
- **Do** put a number next to a claim, and set that number in tabular figures.
- **Do** tune each colour separately for light and dark, then recompute contrast.
- **Do** keep motion to two moments: the hero statement settling on load, and the After bar shrinking once when first seen.
- **Do** theme the browser surfaces as well: selection, scrollbars, underline offset, focus rings.

### Don't:
- **Don't** use purple, violet or blue-to-purple gradients, or any decorative gradient.
- **Don't** round a card, panel or button past 4px, and don't use a pill except on a tiny status tag.
- **Don't** use Inter alone, glassmorphism, three identical cards in a row, emoji icons or generic stock phrases.
- **Don't** add a kicker above a heading, section numbers or tracked uppercase labels.
- **Don't** bring back the Waybill language: yellow, stamps, rotated labels, barcodes, offset shadows.
- **Don't** add a `box-shadow` for depth.
- **Don't** use an em dash or en dash in copy.
