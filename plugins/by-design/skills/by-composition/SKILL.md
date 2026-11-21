---
name: by-composition
description: "Composition foundation for posts, Stories, carousels, Reels covers and ads for any brand in Claude Design: grid, reading order, typography, photo, product, data visualisation, layouts, multi-level checks and learning on the project. Use for any social media visual."
---

# by.composition — the foundation

This skill governs HOW elements are placed. The brand's style (fonts, colours, photo character, tone) lives in the brand's Design System in Claude Design. The visual character (preset) is chosen with the by-presets skill.

## Three layers and which one wins

- **Layer A "Always".** Nothing overrides it: neither brand style nor preset.
- **Layer B "Default".** Applies until the brand's Design System says otherwise.
- **Layer C "Style preset".** The visual character from by-presets: a base preset (Neutral, Editorial, Corporate, Fintech, Health, Bold, Minimal, Playful, Street, Lifestyle) and layers on top (Food, Promo, Beauty, Auto, Real Estate, Holidays, Cultural code). The preset is chosen by the by-presets rules and changes layer B only where its card says so.

The brand's Design System and the project's "Style from practice" (section "Learning on the project") outrank layers B and C. Full order: layer A → brand tokens and README → "Style from practice" → preset (layer C) → layer B. "The brand said otherwise" means both the README text and the values in tokens.json: e.g. a heading weight of 600+ means bold headings are allowed even if the README doesn't say so.

If the brand README contradicts layer A — follow layer A and flag the conflict in the summary for the user.

## Workflow

0. **Settings and project memory.** If the user's design settings (from the design-setup skill: memory line "by design settings", project instructions or `settings/design` in the Trend Library) exist, apply them (market, languages, publishing method); if none exist and the user is present, offer design-setup in one line and continue with defaults. Read the brand's "Style from practice" in full (section "Learning on the project") and apply it in all following steps. It may record a base preset and layers. No brand Design System — first the "Starting a new brand" section.
0a. **Preset and layers.** Determine the base preset and needed layers with by-presets (load it if not loaded). A record in "Style from practice" outranks a guess; a request for one layout ("make it Bold") applies to that layout and doesn't change the record.
0b. **Format — a question before building.** If the post format isn't set in the request, README or "Style from practice", read the text, propose a format and ask how it will be published in one short question (section "Which format to choose") — only then build.
1. **Meaning and volume.** Read the text. Determine the one main thing: headline or number — and the reading order (A2). Check the volume against A1 limits. Doesn't fit — propose splitting into slides or a shortened version. Don't rewrite the client's text yourself: show the shortening in the summary as a proposal, with what was changed.
2. **Layout.** First look at layouts from the base preset and layer cards that fit the content; the "Content → layout" table is for L1–L15 and as a fallback. Consider what the brand allows; only what's after "Don't use" in a card is forbidden. For a carousel — structure per A10.
3. **Photo.** Find a source per A9. No suitable photo — a layout without a photo.
4. **Grid and frame.** The agreed format (step 0b), margins, safe zones, CSS frame.
5. **Text.** Typesetting per layers A and B, non-breaking spaces, hyphenation, even lines.
6. **Building in Claude Design.** Each layout is a separate fixed-size artboard.
7. **Check.** Mandatory, per the "Check" section. Every layout is checked. If the environment can't render an image or run subagents — do what's possible and state honestly in the summary which levels didn't run.
8. **Delivery.** Files, names and alt text — per "Delivery".

## Formats and grid

| Format | Size | Safe zones |
|---|---|---|
| Post / carousel 4:5 | 1080×1350 | in the profile grid the central 1013×1350 is visible: ~34 px cropped on each side |
| Post / carousel 3:4 | 1080×1440 | fully visible in the profile grid; for ads (boosting) — check in Ads Manager, ads default to 4:5 |
| Square 1:1 | 1080×1080 | in the profile grid the central ~810×1080 is visible: ~135 px cropped on each side |
| Landscape 1.91:1 | 1080×566 | the widest allowed post; the profile grid shows only the central ~425×566 (~330 px cropped on each side) |
| Landscape 16:9 | 1080×608 | like 1.91:1, slightly taller; central zone in the grid ~456×608 |
| Landscape 3:2 | 1080×720 | magazine spread (two text columns); central zone in the grid ~540×720 |
| Stories | 1080×1920 | nothing important in the top 250 px and bottom 340 px |
| Reels cover | 1080×1920 | the profile grid shows the central 1080×1440 (240 px cropped top and bottom); the cover headline sits inside it |
| Ads | 4:5, 1:1, 9:16 (and 1.91:1 on request) | as for the corresponding formats |

In a carousel all slides take the first slide's ratio.

### Which format to choose
The post format is part of the design, not a constant. The feed accepts any ratio from 1.91:1 (wide) to 3:4 (tall); taller than 3:4 gets cropped — 9:16 is only for Stories and Reels. Choose by content and intended composition:

| Format | When |
|---|---|
| **3:4** (default) | most posts and carousels: maximum feed space, matches the profile grid; portraits, text + photo, vertical products |
| **4:5** | auto-posting (Metricool and other services via the Meta API accept at most 4:5 — 3:4 gets cropped there), paid ads, series already made in 4:5 |
| **1:1** | catalogue and product round-ups, symmetrical compositions (mark in the centre, circle, 3×3 grid), quotes and short text cards, top-down flat lays, record-sleeve covers and "printed" posters |
| **3:2** (spread) | lots of text in two columns: bilingual carousels (A13), reports, stories, magazine-style long reads |
| **1.91:1 or 16:9** (landscape) | wide scenes: interior, architecture, landscape, a car in profile, a table with dishes; a film frame and video still; a horizontal scale and timeline; two things compared side by side; a row of 3–5 products; one long line of large text |
| **Panorama in a carousel** | one image or word runs across 2–10 slides without a seam (e.g. L49): build one long N×1080-wide artboard and cut it into equal slides; the cut doesn't go through a face or a letter, the first slide reads on its own (A10) |

- **Ask first (step 0b).** In one question propose the format, explain why and ask how the post will be published: manually in the app, via auto-posting or as an ad. Example: "I suggest 16:9 landscape — the interior is wide and reads as one scene. If the post goes via auto-posting I'll make 4:5, if as an ad — 4:5 or 1:1. How are we publishing?" For carousels and series — one question for the whole series.
- **Don't ask again:** offer to record the publishing method and usual format in "Style from practice" ("publishing: auto-posting → no taller than 4:5"). After that ask only if the recorded format is clearly worse for the content. The request, brand and "Style from practice" outrank the proposal.
- **No one to ask** (a task without a person) — take the proposed format, and if the publishing method is unknown — 4:5 as safe everywhere; say so in the summary.
- **Different formats in a feed are fine,** but within one pillar or series — one format.
- **The profile grid crops everything to 3:4 at the centre.** In square and landscape the main thing (headline or cover hero) goes in the central zone from the table above, or consciously accept the tile crop and say so. Show the grid tile next to the layout.
- **Landscape is smaller in the feed:** less text (headline up to 5 words, body up to 15), type sizes no smaller than in 3:4 (same 1080 width), margins 56–72 px. Detailed text — in the next slides or the caption.
- In the summary name the chosen format and in one phrase — why; if torn between two, show the cover in both.

- **Margins:** 72 px unless the brand sets its own. One value for the whole project and all slides.
- All elements, including small text, sit exactly on the margins. Spacing between blocks — from one scale (e.g. 16 / 24 / 40 / 64), not "by eye".
- Lots of air: empty space is part of the composition.
- **Adapting to another format** is not proportional scaling. Type sizes and margins stay, blocks rearrange, the main element stays in the visible zone. Each version is checked anew.

### Artboard CSS frame

Start each artboard with this frame and change only the values:

```css
.artboard {
  --margin: 72px;          /* margins */
  --safe-top: 0px;         /* Stories: 250px */
  --safe-bottom: 0px;      /* Stories: 340px */
  width: 1080px; height: 1440px; box-sizing: border-box;   /* height by format: 1440 / 1350 / 1080 / 720 / 608 / 566 */
  padding: calc(var(--margin) + var(--safe-top)) var(--margin) calc(var(--margin) + var(--safe-bottom));
  display: flex; flex-direction: column; overflow: hidden;
}
.artboard * { hyphens: none; -webkit-hyphens: none; }
.headline { text-wrap: balance; }   /* manual <br> take priority, see A3 */
.body     { text-wrap: pretty; }
```

## Grid plan
When making a content plan, 6+ posts in a row, or the user asks to see the feed:
- Build a profile grid preview: 3 columns, 3:4 tiles, newest posts on top. If the brand's latest published posts are available (Metricool, the account, screenshots) — put them below so the join is visible.
- Show posts of other formats the way the grid crops them (central zone from the formats table); Reels covers — by the 1080×1440 zone.
- **Rhythm:** no two tiles with the same layout or the same dominant colour next to each other horizontally or vertically; photo, text and graphic tiles alternate; one pillar is recognisable by one template.
- Show the grid plan before building all layouts — by covers; fix the publishing order, not the design, if the problem is only adjacency.

## Layer A — always

### A1. Readability — the main rule
Everything is subordinate to readability. A device that hinders reading isn't used.
- Headline — up to 8 words (about 60 characters; for Japanese and Chinese about 15–20 characters, for Korean about 20–25 characters); a question in an interactive Story (A10c) — up to 10.
- Body text — up to 35 words per artboard, in Stories — up to 25 (CJK limits in characters — see A4).
- Total per artboard — up to 50 words, excluding legal text.
- Doesn't fit — split into slides or propose a shortening (step 1).
- A preset may raise the limits (like Corporate), but only with a clear structure: headline separate, body separate, lists as numbered lines. Ceiling — 80 words per artboard.
- Lots of text is no reason to add a picture "just because": keep a text slide, visualise the meaning or split into slides.

### A2. Reading order matches the logic of the text
- The eye moves in the order the meaning is built: usually top to bottom, left to right — headline, explanation, details.
- What carries the message becomes the main element. Meaning in the headline — the headline is first and highest. Meaning in a number ("2x", "53%") — the number is higher or so much larger it's seen first; the headline reads as its explanation.
- One main element per layout. Headline and number don't compete with equal weight.
- Small elements don't sit where the eye should meet the main thing.
- Check: read the elements in order of prominence — it should form a coherent phrase.

### A3. Lines form an even block
- Headlines and texts up to 4 lines: **the shortest line is at least 80% of the longest** (by characters). A long first line and short second and third — a violation.
- For headlines the main method is manual `<br>`: split the phrase by meaning into lines of similar length. `text-wrap: balance` — a fallback and for body text.
- A long paragraph (5+ lines): the last line isn't a single word.
- If it won't even out, in order: first respect A4 → change block width → change type size → propose rewording in the summary.
- Exception: text wraps around a photo or object — line lengths follow the shape.

### A4. Non-breaking spaces and hyphenation
- **Russian:** short words bind to the next one with a non-breaking space: в, с, к, о, у, и, а, я, на, по, под, над, за, из, от, до, не, ни, но, для, без, при, про, через, об, со, во, что, как, это — any first-letter case and after punctuation. The particles же, ли, бы bind to the previous word. A dash doesn't start a line: ` —`.
- Numbers don't separate from units and signs, and follow the post language's conventions: **English (US/UK):** 50%, $10,000, 2,000, 3 days, No. 5, dates "Dec 3" in US English and "3 Dec" in UK English (US numeric 12/03, UK 03/12 — avoid numeric dates in visuals, write the month); **Russian / Kazakh:** 50 %, 10 000 ₸, 2 000, 3 дня, № 5, 3 декабря. Units by market: US — miles, °F, lb, oz; most others — km, °C, kg.
- Hyphenated words don't break: «из‑за», «по‑новому», "well‑known" — non-breaking hyphen U+2011 (`&#8209;`). Initials: "J. R. R. Tolkien".
- Words aren't split by hyphenation (`hyphens: none` in the frame).
- Everywhere in A4 a "non-breaking space" is the U+00A0 character. In HTML write it as the nbsp entity (ampersand, nbsp, semicolon) or as the U+00A0 character itself, never a regular space. At level 1 you search for a regular space (U+0020) after a short word.
- **English:** the same for a, an, the, of, to, in, on, at, by, for, and, or.
- **Kazakh:** the Russian list doesn't apply; bind short function words and postpositions (мен, бен, пен, үшін, деп, да/де, та/те) to the neighbouring word by meaning.
- **Japanese, Korean, Chinese (CJK):** words aren't separated by spaces (Korean uses spaces between word groups), so the Russian/English rules and the regex don't apply. Use `line-break: strict` (Japanese/Chinese — no small kana, closing brackets or punctuation at the start of a line), `word-break: keep-all` for Korean so words aren't split mid-word, and break headlines manually with `<br>` at phrase boundaries (bunsetsu in Japanese; tools like BudouX help). Keep numbers with their counters and units together (3日, 50%, ₩10,000, ¥1,000). Japanese may be set vertically (`writing-mode: vertical-rl`) as a decorative headline device — body text stays horizontal on social media. Leading slightly larger: headline 1.2–1.3, body 1.6–1.8. Full-width punctuation: Japanese 、。「」, Traditional Chinese ，。「」, Simplified Chinese ，。“”. Text limits for CJK are counted in characters: body up to ~90 characters per artboard (Stories ~60), total up to ~130 (Japanese/Chinese; Korean about 1.3× more); body line length 15–25 characters.
- **Other languages:** apply the same principle to that language's short prepositions, articles and conjunctions; add them to the regex.
- Code search for level 1 (a space, not U+00A0, after a short word):
  `(?<![\p{L}])(в|с|к|о|у|и|а|я|на|по|под|над|за|из|от|до|не|ни|но|для|без|при|про|через|об|со|во|что|как|это|a|an|the|of|to|in|on|at|by|for|and|or) ` — flags `iu`. Fix every match.

### A5. Long words
The longest word of the headline fits the text block width in full. If not — reduce the type size (but not below 64 px for a headline or the lower bound set by the preset card), then change the layout or propose a synonym in the summary. Especially check long compound words (in Russian — words of 12+ letters).

### A6. Small text only when it helps (locked — presets and layers can't relax it)
- By default there's no service text: only headline and body.
- Allowed if it helps orientation: a carousel number or section ("Text → Composition → Ending", "2/6"), a source or footnote for a number, a pillar name if it really distinguishes posts.
- **Carousel cover and Reels cover:** the logo is always placed — the file from the Design System, not redrawn, small, in the same place on all of the brand's covers (a corner on the margins or top/bottom centre). It doesn't compete with the headline or cover a face; on a Reels cover — within x 72–940, y 250–1500. No logo file — a placeholder and a question in the summary.
- **Ads and the last carousel slide:** one logo (the Design System file, not redrawn, on the margin) and one CTA up to 4 words are allowed.
- **Exceptions from by-presets cards — only two:** (a) a small brand mark or pillar name in the same corner across a series, if the base preset or layer card suggests it; (b) a CTA on a promo slide (Promo layer). Everything else — per A6.
- **Legal text** is always placed when needed, at least 24 px, and isn't a violation of this rule. If it's unclear whether it's needed — ask or flag it in the summary. It covers disclaimers, restrictions and licence details (especially for brokers and fintech) and ad disclosures, which depend on the market:
  - **US:** FTC disclosure — "#ad", "Paid partnership"; US finance — "Member FDIC" / "Not FDIC insured" where applicable.
  - **UK:** ASA / CAP — "#ad", "Ad".
  - **Japan:** stealth-marketing rules — "広告" or "PR".
  - **South Korea:** KFTC — "광고" or "유료광고".
  - **Other markets:** ask the client for the local requirement.
- Forbidden: account name or handle "as filler", a logo on regular posts, dates and captions just to fill corners, decorative all-caps "frames".
- Corporate brands: only navigation, sources, legal text.
- "Corporate" is taken from the brand README; if it's not there — ask.

### A7. Number visualisation (locked — presets and layers can't relax it)
A7 is about visualising numbers. Structure diagrams (steps, flows, callouts, anatomy diagrams) follow the preset card; they share A7's requirements: one per slide, doesn't compete with the text, everything comes from the text. The preset may set its own line colour and weight.
- **When:** the text has a specific number or change, the brand README doesn't forbid it, and at least 25% of the artboard is free for it. No number — no visualisation.
- **How:** thin lines **2–3 px**, white or in a background tone. Sits behind or next to the text and doesn't compete with it. One per slide.
- **Accuracy:** shows exactly the number in the text. Build it in code so it's verifiable: a ring — SVG with `pathLength="100"` and `stroke-dasharray="53 47"`; a row of dots — exactly N of 100 highlighted; bars — heights strictly proportional to values.
- **A chart line only if the text has at least two data points** (before/after, by year). A single growth figure — two bars or an arrow, not an invented curve.
- In a carousel about numbers — one form on all slides.

| In the text | Visualisation |
|---|---|
| growth or decline, 2+ points | a chart line over the photo or background |
| growth as one figure ("2×") | two bars or an arrow with the number |
| share, percentage | a ring with a segment, percentage in a thin circle |
| people, "one in three" | a row of dots or simple figures, the right part highlighted in a tone |
| several indicators | a column or row of large numbers with captions |
| cycle, system | a circle with node dots and captions |
| stages, time | a horizontal line with marks |

### A8. Contrast
Calculate contrast from hex values: body text at least 4.5:1, large text (48 px+) at least 3:1. For text on a photo assess the lightest and darkest area under the text; if contrast drops anywhere — move the text to a calm zone or change the photo, don't darken.

### A9. Photo source
Order: brand files from the Design System → photos from the client in the conversation → free stock (Unsplash, Pexels) for generic shots → generation → a grey placeholder with a caption of what should be in frame.
- **Stock (Unsplash, Pexels).** Only for generic shots: background, texture, nature, city, interior, objects, unbranded food, atmosphere, symbolic people from behind or in motion. Not for: the client's product and packaging, its team, customers and testimonials, speakers, real places (a residential complex, a venue, a specific car model) — stock isn't passed off as them. No others' logos or recognisable brands in frame; people should resemble the brand's audience (match the market's demographics, not random stock faces), no staged "smiles at the camera". The photo matches the preset (light, colour, shooting character) with one treatment for the whole series. If the photo can't be loaded into the layout directly — use a placeholder and a link to the chosen shot. In the summary — links to each stock photo and the note "stock, replace with a shoot if desired".
- **Stock is forbidden** in the brand README, "Style from practice" or project instructions ("own shoots only", "no stock") — don't use it: go on down the order (generation if allowed, otherwise a placeholder or a layout without a photo).
- Don't generate the product or packaging: real photos only. No photo — a placeholder or a layout without the product.
- Generated people and scenes — only if the brand allows it; note in the summary that the photo is generated.
- No photo — use layouts without photos (L3, L4, L5, L9, L10, L15, and L19, L21, L24 and other photo-free ones from the preset card) and say so.

### A10. Carousel
- **Cover:** a hook headline (and, if needed, one visual anchor) and a small logo per A6. Understandable without the other slides.
- **Inner slides:** 1–2 repeating layouts, the headline in the same place, one thought per slide.
- **Last slide:** a conclusion or CTA, a separate layout; a logo is allowed here (A6).
- Number or section — per A6.

### A10b. Reels cover
The cover is seen twice: large in the Reels feed and as a small tile in the profile grid. It must work in both.
- **Size and zones.** Artboard 1080×1920. The profile grid shows only the central 1080×1440 (y 240–1680). In the Reels feed the bottom ~420 px is taken by the caption and audio, the right ~140 px by buttons. **Headline and face — within x 72–940, y 250–1500.** Background and photo bleed.
- **Reads as a tile.** In the profile grid the cover is ~125 px wide, so: headline 2–6 words, no more than 3 lines, type size at least 110 px (better 120–160), one weight step bolder than the brand's normal headline, contrast per A8 with a margin. No small text on the cover except a pillar tag (A6, at least 36 px); logo — always (A6).
- **One hero.** A face with emotion, a product or an action + a hook headline (what I'll learn / what I'll see). The face is clear (A12): headline above the head, below the chin or to the side.
- **Frame.** Best — from the video itself (a still from the client), so the cover doesn't mislead; otherwise a designed cover by the brand preset. No frame — a placeholder and a hint on which frame to choose (A9).
- **Series and profile grid.** A pillar has one cover template: the same headline position, font, size, pillar tag, pillar colour from the brand palette. Before delivery show the cover in a profile grid mock-up (3 columns, 3:4) next to the brand's neighbouring posts, if any: the feed should look coherent.
- **Style** — from the brand preset (by-presets); these rules are only about format and readability.

### A10c. Interactive Stories
Polls, questions, quizzes, sliders, countdowns, links, "swipe". The sticker itself is added in Instagram at publishing — the design prepares the background and **leaves space for it**. Style — from the brand preset.
- **Sticker zone.** An empty area of about 800×400 px (poll, question, quiz — taller, up to 800×600) in the middle part, not above y 250 and not below y 1580. Mark it in the layout with a dashed outline and a caption "poll sticker" (remove the outline in the final file). No text or faces in this zone.
- **Question on top, sticker below.** The question headline above the sticker zone, short (up to 10 words), large. Don't duplicate the answer options as text — they're in the sticker.
- **Yes/no or A/B poll.** Two photos side by side are OK (A on the left, B on the right), the sticker in the middle or below.
- **Answering questions.** On top — space for the sticker with the follower's question, below — the answer as text per A1 (up to 25 words) or a photo. A series of answers — one template.
- **Countdown and link.** The occasion (date, event) as the headline; space for the sticker below; an arrow or "tap" hint — only if it doesn't clash with the preset.
- **Stories series.** Within one story sequence — one template and one headline position; interactive no more often than every 2nd–3rd Story, so as not to tire. In the summary write which sticker and with what text to add at publishing.

### A11. Font and glyphs
Check that the brand font contains all characters of the text — e.g. Cyrillic; for Japanese — kana and kanji (a Latin font has none: set a CJK font for the whole text, and a Latin font for Latin letters and numbers only if the brand wants it); for Korean — Hangul; and for Kazakh ә, ғ, қ, ң, ө, ұ, ү, һ, і; for other languages their special letters and diacritics. If not — the browser silently substitutes another font: report it in the summary and propose a replacement.

**How many fonts.** A font here is a typeface (family: Inter, Playfair, a script, a mono); different styles of one family (bold, italic) are one font.
- The headline is in one font, and across the whole carousel (Stories series) headlines use the same font. An accent word in another font inside the headline (an italic serif, a script) — only if the preset suggests it; it's a decorative accent.
- No more than 3 text fonts per carousel or series, one per role: headline, subheading, body. Two are usually enough (subheading in the headline or body font); the third is a reserve. Each role is set in the same font across the carousel.
- One rule for all formats: post, carousel, Stories, Reels cover, ads and motion (animated posts and Stories, titles and plates in Reels). In motion the whole video counts as one series, in Stories — the whole sequence.
- Decorative fonts don't count toward the limit: large hero figures (a huge number like "14 years" in L4, a large date, a sale percentage, a full-frame symbol word — together with the unit caption next to it), mono for tags, script accents and stickers, fonts inside graphics (receipts, price tags, interface), the logo, lettering on product photos. But no more of them than the device needs, and the same decorative font throughout the series.
- Fonts come from the brand's Design System; if it has more than three — choose no more than three for the post and name them in the summary.

### A12. The face is clear
On any photo with a person the face (forehead to chin) is free: no text, plates, graphics, stickers or visualisations over it. A portrait isn't cluttered: next to the face — at most a headline and a caption (name, role); other text on another slide or in a free zone of the frame. A large headline can sit above the head or low over clothing, but not on the face. The face is well lit and readable when shrunk to 375 px wide.
- **When the face may be covered.** The rule protects the face of the person the post or Story is about (speaker, expert, story hero, customer, team). If the person in frame isn't the main subject — the post is about a product, texture, application, mood, and the face plays the role of a background or carrier (skin under chips, a model in a cream ad) — text, chips and graphics may overlap the face. Even then the text reads per A8 and the overlap looks like an intentional device, not an accidental cover; note in the summary that the face is covered intentionally. In doubt whether the person is the main subject — keep the face clear.

### A13. Two languages
Many projects are bilingual (e.g. a national language plus a second widely used language). Learn this from the brand's published materials, README or "Style from practice"; if it's not visible — ask once and offer to record it. Below, the **primary language** is the one the brand puts first (usually the national language of the market), the **second language** is the other one.
- **The primary language leads:** higher and/or larger; the second language is the second level. The order is the same on all of the brand's layouts.
- **Languages differ by position, size and tone** — no "EN / RU" labels, flags or other markers. One method for the whole carousel or pillar.
- **Three paths, chosen by text volume:**
  1. **Duplicate slide** — in a carousel each slide comes as a pair: first in the primary language, then the same layout in the second. For texts that won't fit together on one slide per A1. The cover is one, mixed (item 3). Mind Instagram's slide limit.
  2. **Switch in animation** — one layout, the text changes: primary language first, both languages get equal time on screen. Details — in the motion skill.
  3. **Mixing on one layout** — by one of the methods below.
- **Headline only (or a short phrase):**
  - **Weighted pair:** the same font, the second language 2–2.5× smaller and in a tone right below the primary.
  - **Diagonal:** equal size, primary top left, second bottom right in a tone; the middle — air or photo.
  - **Shared hero:** the main element needs no translation (number, percentage, date, product, logo), languages only in a short caption.
  - **Photo + field:** the photo is clean, both languages on the field as a weighted pair.
  - **Stories at the edges:** primary on top, second at the bottom, the middle — photo or sticker.
- **Headline + body:**
  - **Two blocks, top and bottom:** the primary-language block (headline + text) large on top; the same block in the second language at the bottom — smaller headline, everything in a tone; air between them.
  - **Pair + two columns:** headlines as a weighted pair, body in two columns: primary on the left, second on the right in a tone.
  - **Photo in the middle:** the primary block above the photo, the second below; the photo separates the languages.
  - **Mirrored columns:** two identical blocks side by side, the second in a tone; best in 1:1 and landscape.
  - **Photo + field with columns:** a clean photo on top, on the field — a pair of headlines and text in two columns.
  - **Second language in a card:** primary on the field, second in a calm card in the background tone at the bottom.
- **Techniques from practice (bilingual carousels of large brands):**
  - **Don't translate what's the same in both languages.** Numbers, dates, cities, names, brand names are placed once; only the word next to them changes. Example: a large "21", to the right stacked "September" in both languages; one line of city names for both languages.
  - **Hero number + two captions.** One large number; next to it a caption in the primary language (bolder, may be in the brand accent colour) and below it the second language — smaller and in a tone. A row of 3 lines or a 2×2 grid of such blocks with the same geometry (like L9/L15), above them a section title as a weighted pair. The easiest method for reports and numbers.
  - **Second-language kicker over a primary-language hero.** On the cover the second language is a small subheading in a corner on the margin, the primary is a huge headline over half the frame. Hierarchy is held by size, not order.
  - **Two equal blocks across a photo.** In 3:4 the primary block on top, the second at the bottom, a large shot or shape (mountain, circle) between them. Sizes may be equal: the languages are so far apart they don't compete, and the top position makes the primary the main one.
  - **Colour instead of size.** The primary-language headline in the brand accent colour, the second in the main text colour and smaller. This doesn't count as a second accent per B3 if the colour is the same throughout the series.
  - **"Photo + column" spread anchored to the photo edges.** In landscape a photo or video on the left, a column on the right: the primary paragraph aligned to the top edge of the shot, the second to the bottom edge; a second shot may sit between them. A "1/6" counter and the logo in one corner on all slides (A6); a thin progress bar on top instead of the counter, if it suits the preset.
- **Magazine mode — when there's a lot of text and both languages must be on screen at once.** The difference between levels grows: the headline larger than usual, the body smaller.
  - Sizes: primary headline at least 3.5× the body; the second-language headline 2–2.5× smaller than its pair; body 24–28 px (not below 24), leading 1.35–1.45.
  - Text in two columns (primary on the left, second on the right in a tone), line length 30–45 characters, a gap of at least 48 px between columns. Columns mirror each other: paragraphs, highlights and numbers at the same height, the same things in bold in both.
  - Left-aligned, not justified: justification creates gaps between words, especially in agglutinative languages with long words.
  - Limit — up to 80 words per artboard for both languages together (the A1 ceiling with a clear structure), in Stories — up to 50. More — split into slides. A 3:2 spread is ideal for long-text slides.
  - 3:2 spread layouts: cover — a field with a pair of headlines + a photo on half; a photo strip across the spread, columns above and below; a photo column in the centre between the languages; one column (primary over second across a thin rule) + a photo on half. Spread margins 56–64 px, a small slide number in a corner is allowed (A6).
  - In 3:4 and 4:5: a large pair of headlines on top (or under the photo), text in two columns at the bottom past a thin rule; air between them.
  - The mode changes sizes and the limit only for bilingual slides; the rest of layer A applies.
- **Don't overload:** on a mixed layout A1 limits count both languages together (in magazine mode — up to 80). Doesn't fit — path 1. Two equally prominent headlines (same size and colour) — an A2 violation. Plan block width by the longer version.
- **Font** — the same for both languages, with a glyph check per A11; the second language doesn't add a font.
- **Don't invent the translation:** the client provides the second language. No translation — ask; if you translate yourself, note in the summary "translation — have a native speaker check".

## Layer B — default (the brand may change it)

### B1. Levels and sizes
- 2–3 type sizes per layout: headline, body, and if needed service text. A huge number is a separate element and doesn't count.
- The headline is at least 2.5× larger than the body. Almost no medium sizes.
- Guidelines for 1080 width: headline 72–120 px; body 28–36 px; service and legal — at least 24 px.
- Huge number: the glyph height itself is 40–60% of the artboard height, and the number fits within the margins by width.
- Leading: headline 1.0–1.1, body 1.3–1.45.
- Body line length 30–45 characters (CJK — 15–25 characters, see A4).

### B2. Headline case
Sentence case: first letter capital, the rest lowercase. Not all caps and not Title Case Every Word.

### B3. One accent in the text
No more than one accent per layout: an inverse plate on words or a bold last sentence of a paragraph — not colour or underline. A two-tone headline doesn't count as an accent.

### B4. Alignment
Left-aligned, ragged right. Centred — only short text (a question, a name) in centred layouts.

## Layer C — style preset

Described in the by-presets skill: how to choose a preset and the preset cards. If by-presets is unavailable — use Neutral: a neutral grotesque, light background, dark text, one accent, all layer B defaults — and say so in the summary.

## Layout library

A layout is a structure. The look comes from the brand and preset. Layouts L16 and beyond are described in the by-presets cards. Geometry is described for portrait posts (4:5 / 3:4); for other formats adapt per "Formats and grid".

**L1. Photo + headline.** Full-frame photo, headline in the bottom or top third on the left margin, block width 60–80%, 1–3 lines of text below. Text in a calm zone of the photo, no darkening or shadows under the text; face, eyes and main object free. No calm zone — another photo or another layout.

**L2. Question on a portrait.** Full-frame portrait, a short question in the centre over a calm zone (background above the head or to the side, clothing); over the face — only if the person isn't the main subject (A12). A row of numbers below is OK.

**L3. Field + headline.** A colour field, gradient or blurred photo. Headline on the left margin near the vertical centre, a short explanation below. No photo.

**L4. Huge number.** The number is the main element (sizes per B1). The explanatory headline above or below it, small text at the bottom. No photo.

**L5. Text manifesto.** Text only, large, full frame within the margins. For opinions, letters, positions. No photo.

**L6. Card on a field.** A photo or gradient, on top — a text card with its own inner padding (at least 48 px). The card is a layout, not a "backing just in case".

**L7. Magazine spread.** A light field, a small photo placed asymmetrically, a headline and one column of text (in 4:5 two columns don't fit at 28+ px).

**L8. Quote.** A large quote, hanging quotation marks outside the column edge, the author's portrait beside or above, the name small under the quote.

**L9. Row of numbers.** Headline on top, 3–4 indicators in equal columns below: a large number, a small caption. No photo.

**L10. Column of numbers.** Headline on the left, 2–3 large numbers stacked on the right with captions. No photo.

**L11. Large product + text.** The product fills 40–65% of the frame and may bleed off the edge (intentional crop), a text column or data beside it. The product has a shadow or support, packaging text isn't covered.

**L12. Product in the centre + benefits.** The product centred, 2–4 short benefits around it, numbered or read clockwise from top left, type size at least 28 px.

**L13. Texture + text.** A macro texture of the product or ingredient (cream, gel, fibres) full frame, headline on top.

**L14. Diagram over a photo.** A photo or silhouette with a thin diagram per A7 on top (circle, chart, rings) with captions.

**L15. Card grid.** 2–4 identical cards in a row or grid with equal spacing — for lists and comparisons. No photos or small photos in the cards.

Additionally (used inside layouts): **composition table** — rows separated by thin rules, name on the left, value on the right; **tags** — in thin rounded outlines, no more than 5–6.

### Content → layout

| Content | With photo | Without photo |
|---|---|---|
| Thought, opinion, position | L1, L6 | L5, L3 |
| Question to the audience | L2 | L3 |
| One number | L14 | L4 |
| Several numbers | L2 (+ row), L14 | L9, L10 |
| A person's quote | L8 | L5 |
| Product, its benefit | L11, L12 | L13 (if there's a texture), L15 |
| Composition, ingredients | L11 + table | L15, table on L3 |
| Announcement, launch | L1, L11 | L3, L4 |
| List, comparison | L15 | L15, L9 |
| Story, case | L7 | L5 |
| Carousel cover | L1, L2 | L3, L4, L5 |
| Reels cover (A10b) | a frame with a face/product + large headline in the central zone | L3, L4 |
| Story with a poll / question (A10c) | a photo or two "A / B" photos + sticker zone | large question + sticker zone |
| Carousel ending, CTA | L6, L11 | L3 |

## Learning on the project

Goal: over time layouts look more and more like this specific project, not the preset. The preset is a starting point; every approval and every edit by the user shifts the style toward the project.

### Where it's stored
- In the brand's Design System — a section file `project/learned.md` titled "Style from practice". Claude Design reads the Design System itself, so the memory works in any chat and project.
- No Design System — first create one per "Starting a new brand".

### Starting a new brand
When the brand has no Design System:
1. **A short questionnaire** in one message: logo files (SVG or PNG), fonts (names or files, or "none"), colours (hex or a screenshot), the account or published materials, what's off-limits, languages (A13), publishing method (step 0b). Whatever isn't answered — take from the brand's account if there is one, and say what was taken from there.
2. **2–3 directions** for the first post — covers only, on different presets or layouts, with one phrase on how they differ.
3. **Lock in the chosen direction:** create the brand's Design System in Claude Design — tokens (fonts, colours, margins), a README with rules and prohibitions, the logo, `project/learned.md` with the base preset and layers. Show the user before saving.

### Sources, by strength
1. **The user's edits and rejections** ("we don't do that", "bigger headline", "remove the gradient") — the strongest signal.
2. **Approved work** ("approved", "sent to the client", "keeping it"). Analyse what repeats in it: layout, type sizes, colours, photo, visualisation.
3. **New things in the Design System** (fonts, colours, assets) — applied immediately, no separate record needed.
4. **Competitors and references the user pointed to** (an account, board, post). Open and analyse them the same way as a reference board; lower weight — status "observation" until approved work or the user confirms it.

### How to record
- After an approval, edit or reference analysis formulate 1–3 **specific, verifiable** rules: "headline always in the top third, 96 px", "photos only with people, warm light", "we don't use L7", "accent — orange only". Not "it got better" and not matters of taste.
- Record format: **rule** · source (which post / what the user said / which reference, date) · status · what it replaces in the preset or layer B.
- Statuses: **observation** (seen once or only in a reference) → **rule** (confirmed 2+ times or the user said it directly). Said directly by the user — a rule straight away.
- **Ask before recording:** show the wording as one short group (can be at the end of the work) and record only what the user confirmed. Someone else's Design System — only with the owner's permission.
- **A conflict** between a new and an old rule — don't overwrite silently: ask which to keep; mark the old one "replaced (date)".
- A rule that contradicts layer A isn't recorded — say why.
- About every 10 records — compress the file: merge duplicates, remove replaced items, promote confirmed observations to rules (with the user's OK).

### How to apply
- Rules are mandatory (below layer A and brand tokens, above the preset). Observations are preferences: follow them unless there's a reason not to.
- The more is learned about typography, colour, photo and layouts, the less the preset decides — it remains for what the rules are silent about.
- Approved layouts are the best example: if they're on the canvas or in the Design System, look at them before new work of the same type. Their links can be stored in `learned.md`.
- In the summary note which learned rules were applied and propose new ones if they're visible from the work.

### What worked — by statistics
Once a month or on request ("what worked", "analyse the stats"), if Metricool is connected or there's a stats export:
- Take the brand's posts for 30–90 days. Key metrics: saves and shares per reach, reach per follower, carousel completion (if available), retention for Reels. Likes are secondary.
- Link posts to the publishing log in `learned.md` (format, layout, preset and layers, cover type); a post not in the log — identify from the image.
- Compare groups of at least 3 posts. Remember that topic, timing and promotion affect results more than design: compare promoted posts separately, similar topics with each other.
- Conclusions are only **observations** with numbers ("L4 with a number: saves 1.8× above average, 5 posts"). They become rules after the user's OK or confirmation the next month.
- Show briefly: what works, what doesn't, 1–3 proposals for next month. Don't publish or change anything in Metricool without the user's request.

### `learned.md` template

```markdown
# Style from practice — <brand>
Base preset: <preset> · layers: <layers or "none">

## Rules
- Typography: … · source, date · replaces: …
- Colour: …
- Photo: …
- Layouts: we use … / we don't use …
- Visualisation: …
- Text and tone: …

## Observations
- … · source (reference / once)

## Approved examples
- <link> — what's good about it

## Publishing log (last ~30)
- <date> · <pillar> · <format> · <layout> · <preset/layers> · <cover: face / product / text> · <link>
(compress old entries into one summary line once a month)

## Replaced
- … (date, replaced by what)
```

## Check

Five steps: 1 → 1b → 2 → 3 → 4. After any fixes levels 1 and 1b are repeated (they're cheap).

**Modes:**
- **Full** (default for carousels, ads, the first layouts of a new brand, anything going to a client): all levels.
- **Quick** (a single post or Story in an established brand system, or the user asks for speed): 1, 1b, 3 and 4; level 2 — by one reviewer combining both roles.

**Independence.** If subagents can be run in the session, each level 2–3 reviewer is a separate subagent, run them in parallel. Each gets: artboard images, the post text, the brief (what's main, for whom), the brand README and **the full text of its rules copied from this skill** (not numbers, the sections themselves). It doesn't see the building process or your reasoning. If there are no subagents — do one pass by roles yourself and write in the summary: "the check was a self-check".

**A finding:** artboard → specific place → what's wrong → rule → how to fix → level:
- **Blocker** — breaks reading, meaning, reading order; violates layer A; violates the font, colour, logo or a direct prohibition in the brand README. Must be fixed.
- **Important** — noticeably worsens the layout. Fix.
- **Minor** — at discretion. A finding without a specific place and rule number is always minor.

No more than 5 findings per reviewer, in descending importance. No findings — write so: "No findings". Inventing findings for volume is forbidden. Devices the brand allowed contrary to layers B and C are not violations.

### Level 1 — from the code

- [ ] The A4 search finds no matches; dashes, numbers, hyphens formatted per A4.
- [ ] The frame is in place: `hyphens: none`, manual `<br>` or `text-wrap: balance` on headlines, `text-wrap: pretty` on paragraphs.
- [ ] Text volume within A1.
- [ ] Type sizes per B1 (or the brand); service and legal at least 24 px.
- [ ] Margins one value; the format's safe zones respected (including the profile-grid zone for 4:5 and Reels covers).
- [ ] Reels cover: headline and face within x 72–940, y 250–1500; headline ≤ 6 words, ≤ 3 lines, ≥ 110 px; reads as a profile-grid tile (shrink the render to 125 px wide and check).
- [ ] Interactive Story: the sticker zone is free of text and faces, within y 250–1580; the dashed marker removed in the final file.
- [ ] Small text only as allowed by A6; the logo is on carousel and Reels covers (in one place for all of the brand's covers); otherwise logo and CTA only in ads and on the last slide.
- [ ] Visualisation per A7: values in the code match the text; a chart line only with 2+ points.
- [ ] Contrast per A8 calculated.
- [ ] Fonts and colours from the brand's Design System; the font contains all characters of the text (A11).
- [ ] Count `font-family` in the code: headlines in one font; no more than 3 text fonts (headline, subheading, body) per carousel; decorative ones don't count (A11).
- [ ] Product and packaging are real photos (A9).
- [ ] No element overlaps the face of the post's main person; next to a portrait — no more than a headline and caption (A12). An intentional overlap of a "non-main" person's face is noted in the summary.

### Level 1b — after rendering

Render each artboard to PNG at actual size (if the environment allows; if not — say so in the summary).
- [ ] Text doesn't go beyond the artboard and margins; nothing is cut off.
- [ ] The brand font loaded (no fallback font), images loaded.
- [ ] Count the actual headline lines: is the A3 80% met; no dangling short words and no single word on the last line.
- [ ] The longest word fits (A5).

### Level 2 — two roles

**Form** (typographer + compositor). Gets sections A1–A5, A10, A11 (number of fonts), B1–B4, the layout library, the base preset card (for Bold — with the sub-style rules), layer cards and descriptions of the L16+ layouts used. Looks at: lines in an even block and line breaks, hierarchy and size contrast, one main element, order of prominence matches the logic of the text, the layout fits the content, everything on the margins and grid, enough air, nothing sticks to the edge or to each other, in a carousel the headline and margins don't jump between slides. Plus typos, double spaces, correct quotation marks for the language (« » in Russian, “ ” in English, 「」 in Japanese and Traditional Chinese, “ ” in Simplified Chinese), correct dashes.

**Photo and brand.** Gets the brand's "Style from practice", sections A6–A9, A11, A12, the base preset and layer cards from by-presets and the brand README. Not launched if the layouts have no photo or product — then "Form" checks the brand. Looks at: the photo's focus isn't covered by text, text in a calm zone without darkening, cropping is intentional, the product takes the right share and has support, no generation artefacts (extra fingers, crooked letters, melting edges), fonts/colours/photo character/tone match the brand, nothing the README forbids, small text and logo per A6.

### Level 3 — viewer test

A separate reviewer **without the brief and the post text** — only the images, shrunk to 375 px wide (as on a phone). For a carousel — first only the cover: "Would I swipe further? What does this post promise?" — then the other slides.

Questions for each artboard:
1. What did I read first, second, third?
2. What is this post about, in one phrase?
3. Where did I stumble or what's unclear?
4. Would I stop in the feed? (An answer for the summary, not a blocker.)

If the reading order or meaning (questions 1–2) don't match the brief — **blocker**: redo the layout or hierarchy, not just the details.

### Level 4 — art director's summary

You do this.
1. Collect findings into one table, remove duplicates.
2. Resolve conflicts by priority: readability → reading order → brand → composition → aesthetics.
3. Fix blockers and "important", minor ones if they don't break something else. Repeat levels 1 and 1b.
4. If there were blockers — repeat levels 2–3 only for the fixed artboards. Two rounds maximum. A blocker remains — don't hide it: show the layout and say directly what didn't work and why ("this photo has no calm zone for the headline, another photo is needed").
5. Together with the layout show the user a short summary:
   - check mode and how many rounds; which levels couldn't run and why;
   - what was fixed — one line per item;
   - proposed shortenings of the client's text (before → after);
   - what needs the user's decision: generated photos, whether legal text is needed, brand conflicts with layer A, font replacements, which preset was chosen and why (if it wasn't named explicitly).
   No retelling of the rules and no process report.

## Delivery
- **Size:** exactly the artboard size for the format (1080 wide), no scaling.
- **File:** PNG — for graphics, text, plates; JPG quality 90+ — for full-frame photos. sRGB. If Claude Design doesn't let you choose the format — export as is and say so in the summary.
- **Names in Latin characters, no spaces:** `brand_pillar_YYYY-MM-DD_01.png` — the slide number in two digits in carousel order; Stories `_story01`, Reels cover `_cover`, ad `_ad-4x5`, second language `_<lang code>` (e.g. `_ru`), new version `_v2`. Example: `brand_tips_2026-12-03_01.png`.
- **One publication — one folder or archive** with the same name without the number.
- **Alt text** for each slide — in the summary, 1–2 sentences in the post's language: what's depicted and the slide's main text. It goes into Instagram under "Advanced settings → Alt text".
- If there are stickers (A10c) or a second language (A13) — remind in the summary what to add and where at publishing.
- After publishing offer to add a line to the publishing log in `learned.md`.

---
Author: Sanira Baitasova. Part of the by skills collection.
