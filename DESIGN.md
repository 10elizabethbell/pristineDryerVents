---
name: Pristine Dryer Vents LLC
description: Owner-run dryer vent cleaning in Ocean County, NJ. Clean dryer, no fire.
colors:
  vent-blue: "#15a0f5"
  vent-blue-light: "#4db8f8"
  blue-ink: "#0a5fa8"
  pristine-navy: "#0d3768"
  deep-navy: "#06182f"
  ink: "#06182f"
  body: "#24364b"
  soft: "#4a5a6c"
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c6d5ea"
  line: "rgba(6,24,47,.12)"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(44px, 12.6vw, 84px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  numeral:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(64px, 19vw, 88px)"
    fontWeight: 400
    lineHeight: 0.9
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(20px, 5.4vw, 24px)"
    fontWeight: 400
    lineHeight: 1.15
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  body-large:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 4.8vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  caption:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.7
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-mobile: "20px"
  gutter-desktop: "40px"
  band-mobile: "64px"
  band-desktop: "96px"
  stack-sm: "12px"
  stack-md: "20px"
  stack-lg: "28px"
  column-gap: "64px"
components:
  button-primary:
    backgroundColor: "{colors.vent-blue}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.vent-blue-light}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-ghost-ink:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "48px"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.body}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  step-marker:
    backgroundColor: "{colors.vent-blue}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.vent-blue}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "60px"
---

# Design System: Pristine Dryer Vents LLC

## Overview

**Creative North Star: "The Calm Band"**

A one-page, phone-first site built from full-width horizontal bands that alternate between off-white paper, Pristine navy, and a deep navy carrying faint diagonal lines. Every band holds one idea in big, friendly Cal Sans and short system-font copy, so the page reads like a neighbor explaining things plainly, one screen at a time. The single loud colour is the logo's vent blue, and it is spent on things you tap (buttons, the step markers, the floating text circle) and on the last phrase of a few headings. It is not used for decoration.

Density is low and type is large: body copy sits at 16/1.7, ledes at 18 to 19px, and every touch target is at least 44px tall, because many visitors are older homeowners arriving from Facebook on a phone. The world has no photography (the business has no job photos), so the hero is a plain textured navy band. The logo artwork sits on its own matte card, in the hero's right column on desktop and under the owners' intro on phones.

Motion is restrained and switchable: the hero H1 bounces in letter by letter once, content below the fold rises 12px as it enters, and a floating text circle slides up once the hero has gone. All three respect `prefers-reduced-motion`, and `CONFIG.MOTION = false` turns the first two off for an older-audience build.

**Key Characteristics:**
- Three band grounds (paper, navy, deep navy with lines); no gradients, no photos.
- One accent, the vent blue, used as a fill. Text on it is always ink.
- Cal Sans at weight 400 for every display role, including buttons, labels, prices and the phone number.
- Fully round pill buttons and chips, 24px cards, 10px fields.
- Flat surfaces. The only shadows are on things that float.
- Booking is a text message: every primary action ends in `sms:` or `tel:`.

## Colors

A cool, near-monochrome navy-and-paper palette with one saturated sky blue taken from the logo.

### Primary
- **Vent Blue** (`vent-blue`): the logo's blue and the only accent fill. It is used for primary pill buttons, numbered step markers, the floating text circle, and `::selection`. On navy and deep-navy bands it is also the accent colour for heading phrases and icons, the focus outline, and link hover.
- **Vent Blue Light** (`vent-blue-light`): the hover state of primary buttons. Only used there.
- **Blue Ink** (`blue-ink`): vent blue darkened enough to be read as text on light grounds. It is used for accent heading phrases on paper, the line icons in the claims list, the header phone icon and its hover, and the "You save $10" emphasis.

### Neutral
- **Paper** (`paper`): the page ground, the header, and light bands. Also `theme-color`.
- **Card White** (`card`): the form card and the inner price panel; selected-chip text.
- **Field Mist** (`field`): input and unselected-chip fill on the white form card.
- **Ink** (`ink`): headings on light grounds, all text on vent blue, the selected-chip fill.
- **Body Slate** (`body`): running text on light grounds.
- **Soft Slate** (`soft`): ledes, placeholders, helper text, the wordmark subline.
- **Pristine Navy** (`pristine-navy`): the hero, price, and closing bands; also the focus and hover outline on light grounds, and the text caret.
- **Deep Navy** (`deep-navy`): the "How it works" band and the footer, always paired with the line texture.
- **On-Dark** (`on-dark`) and **On-Dark Soft** (`on-dark-soft`): headings and body text on the navy bands.
- **Hairline** (`line`): 1px dividers between claims and inside the price card.
- **Error Red** (`error`): field error text and the error border. Never used decoratively.

### Contrast pairings (WCAG 2.x, measured)
| Foreground on ground | Ratio | Use |
|---|---|---|
| ink on paper | 16.5:1 | headings |
| body on paper | 11.4:1 | running text |
| soft on paper / card / field | 6.5 / 7.1 / 6.0:1 | ledes, helper, placeholder |
| blue-ink on paper / card | 6.0 / 6.5:1 | accent text on light |
| ink on vent-blue / vent-blue-light | 6.3 / 8.1:1 | button, marker, float labels |
| on-dark on navy | 11.1:1 | headings on navy |
| on-dark-soft on navy / deep | 8.0 / 12.0:1 | body on dark bands |
| vent-blue on deep | 6.3:1 | accent text, link hover |
| vent-blue on navy | 4.2:1 | large display accents (24px and up), icons and focus rings only |
| ink on field / card on ink | 15.0 / 17.8:1 | inputs, selected chip |
| error on card | 6.5:1 | error text |
| vent-blue on paper | 2.6:1 | **not allowed** for text or focus |
| white on vent-blue | 2.9:1 | **not allowed** |

### Named Rules
**The Fill-Only Blue Rule.** Vent blue is a fill. Text and icons on it are always ink. When blue has to be text on a light ground it becomes blue ink. On navy it may be text only at display sizes (24px and up), because it reaches 4.2:1 there and needs large text to pass.

**The Three Bands Rule.** A section sits on paper, navy, or deep navy. The diagonal line texture (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`) goes only on the hero and the deep-navy bands. Plain navy bands (price, close) stay untextured.

**The Navy Focus Rule.** On light grounds, focus and hover outlines are Pristine navy, so they never look like the blue fill. On navy and deep grounds the outline switches to vent blue. On the blue float circle it is white.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** the system UI stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans is a rounded, geometric display face set at one weight. It makes headings and buttons feel friendly and confident. The native system body keeps running text familiar and fast on in-app phone browsers.

### Hierarchy
- **Display** (400, clamp 44 to 84px, 1.02, max 11ch): the hero H1 only. It contains the place name in vent blue.
- **Numeral** (400, clamp 64 to 88px, 0.9, -0.02em): the price figure. The closing phone number is a sibling at clamp 30 to 52px, 1.
- **Headline** (400, clamp 30 to 48px, 1.08, balanced wrap): section H2s.
- **Title** (400, 20 to 24px, 1.15 to 1.2): claim rows, step titles (21px, 22px on desktop), the price card heading (20px), and the "Where we work" heading (24 to 30px).
- **Label** (400, 18px, 1 to 1.2): button text, form labels and legends, the header phone number (20px on desktop), and the "Locally owned" words line (18 to 21px).
- **Body Large** (system 400, 18 to 19px, 1.7, 40 to 52ch): ledes, the owners' intro, the town lists. The hero promise is a variant at 17 to 20px, 1.5, 32 to 40ch.
- **Body** (system 400, 16px, 1.7): default text, inputs, chips, the footer.
- **Caption** (system 400, 14px): helper text under the form and "(optional)" markers.
- **Wordmark subline** (system 600, 11px, 0.08em, uppercase): "Dryer Vents LLC" under the wordmark only.

### Named Rules
**The One Weight Rule.** Cal Sans is only ever set at 400. Hierarchy comes from size alone. Don't fake-bold it, and don't use it for running text.

**The Accent Phrase Rule.** Some headings end with a phrase in the accent colour: vent blue on dark bands, blue ink on paper. Examples are "Ocean County, NJ.", "per dryer.", "Daniel & Brandi.", "works." and "no fire." Use it on a minority of headings, never all of them. (The house style says dark bands only. The build also uses it once on paper, in blue ink, and this file records the build.)

**The Hero-Only Bounce Rule.** Only the hero H1 animates letter by letter. No other heading moves except through the shared fade-up.

## Layout

The layout is a single column of full-bleed bands. Content sits in a centred container (max 1160px) with a 20px gutter that becomes 40px at 760px. Bands have 64px vertical padding, or 96px at 760px and up. The hero uses 56/68px top/bottom padding, or 96/112px on desktop.

- **Phones (default):** everything stacks. Hero buttons are full-width in a 12px grid. Headings blocks use a 16px gap and a 640px max width.
- **760px:** hero buttons sit side by side with a 230px minimum width, and the promise widens to 40ch.
- **1024px:** two-column splits with a 64px column gap. These are claims beside the "why" text, the price card at 460px beside its heading, the owners' intro beside the area, and the form at 1.2fr beside a sticky heading (top 40px). The steps become three columns with a 40px gap, the hero gains its logo column (440px), and the closing phone number aligns to the bottom right of the heading.
- **380px and below:** chips tighten to 14px side padding.

Rhythm comes from vertical stacks of 12, 16, 20 and 28px inside bands, and 64px between columns. Safe-area insets are respected at the header top, the footer bottom, and the float circle's corner. The footer reserves 96px of bottom padding so the float circle never covers its text.

## Elevation & Depth

The surfaces are flat. Depth comes from the band colours (paper, then navy, then deep navy), from white cards set on paper, and from the price card's translucent white frame (`rgba(255,255,255,.08)`, 10px) around a solid white panel. Shadows are reserved for objects that sit above the page.

### Shadow Vocabulary
- **Float** (`box-shadow: 0 10px 28px rgba(3,14,30,.35)`): the floating text circle.
- **Hero logo lift** (`box-shadow: 0 24px 60px rgba(2,10,22,.45)`): the logo card in the desktop hero column only.

### Named Rules
**The Flat Bands Rule.** Cards, buttons, chips and inputs have no shadow, at rest or on hover. A shadow means the object floats over the page, and only the text circle and the hero logo do that.

## Shapes

The form language is soft and round. Buttons and chips are fully round (`pill`). Content containers have a 24px radius (`card`): the form, the price card, and the logo matte. The price card's inner white panel uses 18px so the nested curve stays concentric inside the 10px frame. Inputs use a gentler 10px (`field`). Step markers and the float circle are true circles. Borders are 2px and transparent at rest, so hover and focus can colour them without shifting layout. Dividers are 1px hairlines. Icons are inline SVG line drawings (2.2 to 2.4 stroke, round caps and joins) in `currentColor`.

## Components

### Buttons
Big, round, and obvious. They are built for thumbs.
- **Shape:** full pill (`pill`), at least 56px tall, Cal Sans 18px, a 10px gap to an optional 20px icon, and a 2px border.
- **Primary:** vent blue fill and border with ink text. It is used for "Book a cleaning" and "Text this to us". Hover (on pointer devices only) moves to vent blue light. Inside the form and for the ghost-ink button, hover adds a 2px navy outline offset by 2px.
- **Ghost (dark bands):** transparent, with on-dark text and a 70% on-dark border. Hover makes the border white and adds a 10% white fill. It is used for "Text us" in the hero.
- **Ghost Ink (light):** 48px tall, 16px text, ink border and text. It is the secondary action on the white card ("Copy message").
- **Press:** scales to 0.98 over 120ms. Colour changes transition over 200ms.
- **Focus:** 3px outline offset by 3px, navy on light and vent blue on dark.

### Chips (single-choice radio)
- **Style:** pill, 48px tall, field mist fill, ink 16px system text, and a transparent 2px border. The real radio input is visually hidden but still focusable.
- **State:** hover gives a navy border. Selected gives an ink fill with white text, and hovering a selected chip shows a navy outline. Keyboard focus gives a 3px navy outline.

### Cards / Containers
- **Form card:** white, 24px radius, padding clamp 20 to 32px, a 20px internal grid gap, max 600px. No border and no shadow.
- **Price card:** a translucent white frame (10px padding, 24px radius) on navy. It holds a white panel (18px radius, 24/22px padding) with the title, the numeral, and a hairline-divided first-time line. A full-width primary button sits underneath.
- **Logo matte:** 24px radius, near-black matte matching the artwork, 12/16px padding, max 520px.

### Inputs / Fields
- **Style:** field mist fill, a transparent 2px border, 10px radius, at least 52px tall, 13/14px padding, ink 16px text, a navy caret. Placeholders are soft slate. The textarea is at least 110px tall and resizes vertically.
- **Label:** Cal Sans 18px in ink, above the field with an 8px gap. Optional fields carry a 14px soft "(optional)".
- **Hover / Focus:** the border turns navy (no glow) over 150ms.
- **Error:** the border turns error red, a 16px error message appears below, and `aria-invalid` is set. The error clears as soon as the field has a value.

### Navigation
There is no menu. The header is a paper bar, 64px tall (76px on desktop). The wordmark sits on the left ("Pristine" in Cal Sans 22 to 25px over an 11px uppercase subline) and the tap-to-call number on the right (Cal Sans 18 to 20px with a blue-ink phone icon, hovering to blue ink). Every target is at least 44px.

### Numbered Steps
An ordered list with a CSS counter. Each step has a 48px vent-blue circle holding an ink Cal Sans 20px numeral, then a Cal Sans title on-dark and a soft one-line explanation. It stacks on phones with a 24px gap and becomes three columns at 1024px.

### Claims List
A divided list. Each row has a 40px blue-ink line icon followed by a Cal Sans 20 to 24px statement, with 15px vertical padding and hairlines between rows.

### Floating Text Circle (signature)
A 60px vent-blue circle fixed bottom-right (16px plus the safe-area inset) with a 26px ink chat icon. It opens `sms:` with a pre-filled message. It waits 120px below the viewport and slides in over 350ms (`cubic-bezier(.2,.8,.2,1)`) once the hero has scrolled away, then hides again while the booking form is on screen. Its tab index and `aria-hidden` follow its visibility. There is one circle, never a bottom bar.

### Motion
- **Hero H1 bounce-in:** JS splits the heading into letters once Cal Sans loads (with a 600ms fallback). Each letter goes from `opacity:0; translateX(50px)` to rest over 1s on `cubic-bezier(.34,1.56,.64,1)`, staggered 20ms per letter. Words stay unbroken, and the no-break space keeps "no fire" together. The H1 carries an `aria-label` during the animation, and the plain HTML is restored after the last letter lands. Without JS, or with calm motion, the heading is static.
- **Fade-up:** elements marked to rise are visible at rest. Only those that start below the first screen get hidden (12px down, transparent) and then rise over 400ms ease-out on entering (rootMargin -8% at the bottom). Claim rows stagger by 40ms.
- **Reduced motion:** `prefers-reduced-motion` disables the bounce, the fade-up, smooth scroll, and button and float transitions.

### CONFIG switches
These are set in the script `CONFIG` object at the top of the page.
- **`FLOAT`** (default `true`): `false` removes the floating text circle from the DOM. It is also removed if IntersectionObserver is unavailable.
- **`MOTION`** (default `true`): `false` disables the H1 bounce-in and the fade-up, and is meant for an older-audience (40+) build. It is equivalent to reduced motion for those two effects.
- **`PHONE`** (`+17327991379`): the number the booking form composes its `sms:` to. The static `tel:` and `sms:` links in the markup hold the same number and must be changed alongside it.

## Do's and Don'ts

### Do:
- **Do** use vent blue only as a fill for actions and markers, with ink text on it (6.3:1).
- **Do** switch blue to blue ink whenever it is text or an icon on paper or white.
- **Do** keep Cal Sans at 400 and let size carry the hierarchy (84, 48, 24, 18px steps).
- **Do** keep every touch target at least 44px, buttons at 56px, chips at 48px, and inputs at 52px.
- **Do** put hover styles inside `@media (hover:hover)` so taps don't leave them stuck on.
- **Do** keep content visible at rest. Motion only reveals what starts below the first screen.
- **Do** route every booking action to `sms:` or `tel:` on the one published number.

### Don't:
- **Don't** set vent blue as text on paper (2.6:1) or white text on vent blue (2.9:1).
- **Don't** use vent blue as body-size text on navy. At 4.2:1 it is for display-size accents only.
- **Don't** add shadows to cards, buttons, chips or inputs. Shadows are for the float circle and the hero logo.
- **Don't** put the line texture on paper or on the plain navy price and closing bands.
- **Don't** animate any heading but the hero H1, or add motion beyond the 12px fade-up.
- **Don't** replace the float circle with a sticky bottom bar, or add a second floating action.
- **Don't** add a Call button to the hero. The number lives in the header's top right and in the closing band.

### Flagged exception (not a system rule)
The build has three small "eyebrow" pill labels above headings (hero, price, and booking). Ellie asked for them in her house calm style on 2026-10-19, and HANDOFF.md records them as a known Impeccable conflict. They stay in this build as her decision, but they are not a component for new surfaces to copy. Don't add eyebrows to further headings or new pages unless Ellie re-confirms.
