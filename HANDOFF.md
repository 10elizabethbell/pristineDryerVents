# Pristine Dryer Vents LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/pristineDryerVents/ · **Repo:** https://github.com/10elizabethbell/pristineDryerVents · **Built:** 2026-10-20 from Muse brief (run 2026-10-20, NJ Small Business Network group post) · **Call Sheet:** site URL set

## What's built
- One page, phone first, calm band style: paper header (wordmark left, tap-to-call 732-799-1379 top right) → navy hero (H1, "We're Daniel & Brandi, the owners. $139 per dryer, $129 your first time.", two buttons) → "Safer homes. Lower drying times. Peace of mind." with the flyer's own five benefits → navy price card ($139 per dryer, $129 first time) → "Hey neighbors, we're Daniel & Brandi" + where we work → deep-navy How it works (3 steps) → booking form → navy close ("Clean dryer, no fire." + big phone) → deep footer (name, owners, area; no number there because the close's number is on the same phone screen).
- Palette from the flyer logo: navy #0d3768, deep #06182f, the logo's vent blue #15a0f5 as the one accent fill (navy text on it), #0a5fa8 when blue has to be text on light.
- Hero: plain textured navy band (no photo, see below). H1 "Clean dryer, no fire. Ocean County, NJ." bounces in letter by letter. On desktop (≥1024px) the logo sits in the hero's right column; on phones it sits under the owners' intro.
- If the messages app doesn't open, the form shows the number plus a "Copy message" button (clipboard may be blocked in Facebook's browser, so the number is always there too).
- Contact: "Book a cleaning" → form; "Text us" → `sms:` with a pre-filled message; floating text circle after the hero (hidden over the form). The form (name, town, number of dryers, first time?, when, notes) composes one text. The price card's button pre-ticks "first time".
- `CONFIG.MOTION = false` turns off the bounce-in and fade-up in one switch (see the audience question below).
- Favicon/home-screen icon: a "P" lettermark drawn in the site's colours (the logo is too detailed for 16px). og.png is a 1200x630 card with the headline.

## Assumptions I made
- **Accent is blue, not warm.** The calm style asks for a warm accent, but the brand is all blue/silver/white; the brand wins on colour. A warm amber would read as "fire" on a fire-safety site.
- **"We" voice, both owners.** The caption is "We're Daniel & Brandi, the owners". I wrote that you deal with the owners when you book (the number is Daniel's) — confirm they do the jobs themselves.
- "Locally owned & insured" and "Friendly, reliable service" are quoted as their own words; insurance itself isn't verified.
- I cut "No surprises" from the price band: nothing says there are no extra charges (question 3).
- "$139 per dryer" read as one dryer's vent. The flyer said "First time customer $10 off"; the caption said "First-time customers save $10 — only $129!". Both used.
- Service area: caption towns first, then the flyer's towns; "Tom's River" corrected to Toms River; "everywhere in New Jersey except North Jersey" from the flyer.
- The benefit list is exactly the flyer image's five (Prevents fire hazards, Improves drying time, Increases energy efficiency, Extends dryer lifespan, Cleaner, safer home). Muse's OCR also had "Lowers energy bills", "Healthier indoor air" and "Prevents house fires"; they aren't on the image, so I left them out. The section's lede is the flyer's own sentence.

## Placeholders and gaps
- **No real job photos.** The only image is their promo flyer, which is an illustration; its before/after is a drawing, not a photographed job, so I didn't present it as proof or put it in the hero. Hero = plain textured navy band. **Photos wanted:** real before/after of a vent, lint pulled out, the owners at work.
- **No Facebook link** anywhere: they have no business page (the ad was posted from Daniel's personal profile). The flyer says "Follow Us" with a Facebook icon, so a page may exist that Muse couldn't find. Once there is one, add "Click to see more of our work." under the proof and in the footer.
- **No email** (none found), so the footer has none.
- **No reviews.** The flyer's "5 star reviews on Google" claim is not used: no Google listing exists.
- No hours, no years in business.
- Logo is cropped from the flyer (820x400); ask for the original file.

## Questions for the owner
1. Do you have a Facebook business page, and photos of real jobs (before/after)?
2. Hours and how quickly you can usually come out?
3. Any extra charges beyond $139 per dryer (roof vents, long runs, repairs, bird guards)?
4. Is the first-time $10 off ongoing?
5. Do you do anything besides vent cleaning (repairs, new vent lines, inspections)?
6. Are you insured, and is there anything to show for it? Is there a Google listing on the way?
7. Do both of you come out to jobs?

## Ideas not built (yours to pick)
- **Older audience?** Manchester and Whiting (their first-named towns) are home to big 55+ communities. If you think the customers skew older, set `CONFIG.MOTION = false` (no bounce-in, no fade-up), raise the body to 18px, and consider Atkinson Hyperlegible (`references/older-audience.md`). I left the default calm motion on because the brief doesn't flag the audience.
- Opt-in signature motion worlds, best first: **lint that clears** (a vent cross-section in the hero, packed with grey lint you wipe out with a finger to reveal clean silver duct, regrowing slowly), airflow (soft lines streaming out of a vent, faster once cleaned), the flyer's silver spiral duct as a drawn backdrop, a lint-trap screen you peel, warm/cool dryer drum.
- A real before/after slider once actual photos exist.
- "Book your yearly cleaning" reminder text (offer to text customers a year later) — a natural first paid feature.
- Desktop: the booking section's left column is empty beside the tall form (only a sticky heading). Option from the finish review: move the How-it-works steps under the booking lede at ≥1024px.
- "Prevents fire hazards" as a bigger lead row above the other four (sweep's "bolder" idea).
- Impeccable flags kept by design (your calm-style choices): eyebrow pills, diagonal band texture (detector: "repeating-gradient stripes"), Cal Sans, the H1 bounce-in, the floating circle. Detector ignores saved in `.impeccable/config.json` (texture: house style; flat type hierarchy: false positive, headings are clamp() 30–84px).

## Not verified
- Real-device touch, and the SMS handoff on real iOS/Android and inside Facebook's in-app browser (tested headlessly: composed message decodes correctly).
- Frame rate of the bounce-in on old phones.
