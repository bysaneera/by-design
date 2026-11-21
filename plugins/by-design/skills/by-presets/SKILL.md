---
name: by-presets
description: "Style presets for social media visuals (Neutral, Editorial, Corporate, Fintech, Health, Bold, Minimal, Playful, Street, Lifestyle) and layers (Food, Promo, Beauty, Auto, Real Estate, Holidays, Cultural code): how to choose and combine them. Use together with by-composition."
---

# by.presets — style presets

A preset is a visual character: typography, colour, photo, graphics, suitable layouts. It works together with the by-composition skill:
- **Layer A of by-composition** (readability, reading order, even lines, prepositions, small text, visualisation, a clear face, checks) — no preset overrides it.
- **The preset** replaces layer B defaults where its card says so explicitly ("Changes in layer B").
- **The brand's Design System and the project's "Style from practice" outrank the preset.** Their fonts, colours, logo, prohibitions and learned rules aren't touched. The preset fills in what they're silent about. The more the project has learned, the less the preset decides.

Layout numbers L1–L15 are from by-composition. L16–L70 are additional, described in the preset cards (they can be used in other presets too unless the card forbids them).

**Colour in presets is an example, not a requirement.** The preset governs composition, hierarchy, typography, photo character, graphics and devices. Colours in the cards are what often appears in references, not a rule. The palette comes: (1) from the brand book / brand Design System; (2) if the brand is silent or gives freedom — from the aesthetics and mood of the specific post; (3) only if neither — from the card's examples. A dark background with acid-yellow 3D, if that's the brand — fine. Don't change brand colours for the sake of a preset. Of the colour rules only these are mandatory: contrast (A8), the number of accents the preset sets, and what the card calls a device (tonality in Health, no gradients in Minimal) — in the brand's colours.

**Examples are not content.** Texts, numbers, names and brands in the cards ("3.7% per year", "835 km", "Which car is this?") are examples of form. Only the client's text and data go into the layout; whatever's missing — a placeholder in square brackets ("[price]") and a question in the summary. Reference pins are examples of a device: others' compositions one-to-one, slogans, characters and logos aren't copied.

**Text in the cards is a criterion, not permission to rewrite.** If the client's text doesn't meet the card's requirements ("simple and clear", "humour", "term explained"), propose a version in the summary (before → after) per step 1 of by-composition.

**Names for the "Preset: X" record.** Base: Neutral, Editorial, Corporate, Fintech (/ Friendly Tech), Health, Bold (/ sub-style), Minimal, Playful (= Cute), Street, Lifestyle. Layers: Food, Promo, Beauty, Auto, Real Estate, Holidays, Cultural code.

**Layout index.** L16, L22–L24 — Fintech; L67–L70 — Fintech, Friendly Tech sub-style; L17, L48–L50 — Promo; L18, L41–L43 — Street; L19–L21 — Corporate; L25–L27, L59 — Health; L28–L34 — Bold; L35–L37 — Minimal; L38–L40 — Playful; L44–L46 — Lifestyle; L47 — Food; L51–L52 — Beauty; L53–L55 — Auto; L56–L58, L60 — Cultural code; L61–L63 — Real Estate; L64–L66 — Holidays.

**Formats.** Stories, Reels covers and ads: preset and layers give the character, the geometry comes from A10b/A10c and by-composition safe zones. Carousel layouts don't transfer to a single format. On a Reels cover the size and weight follow A10b even in Minimal and Editorial. In layouts with an element spanning several slides (L48, L49, L55, "Property name across two frames") the first slide reads as a finished cover on its own (A10), the cut doesn't go through a letter, the edge keeps a 72 px margin.

## How to choose a preset

Go through the steps, stop at the first that applies.

1. **Named explicitly.** In the request ("in Bold style") or in the brand Design System README / project instructions as a line "Preset: X". Take it.
2. **There's a brand Design System.** Read the README and tokens.json and add up the signals from the table below. One preset clearly ahead — take it.
3. **Can't decide confidently** (two presets close or few signals) — ask the user one short question with 2–3 options and an explanation of the doubt. Example: "The font is neutral, but there are gradients and 16 px radii. Closer to Corporate or Fintech?" Offer "show both": then build a cover or one slide in 2–3 presets side by side and let them choose by eye. If there's no one to ask (a task without a person) — take the closest and explain the choice in the summary.
4. **No Design System.** Decide from the brief and industry ("For whom" in the cards). Unclear and no one to ask — **Neutral**.

**Lock in the choice.** When the preset was determined by steps 2–4, offer to add a line "Preset: X" to the brand Design System README or the project instructions. Don't edit someone else's Design System without permission.

### Signals

| Signal | Points to |
|---|---|
| Monochrome or 1 muted colour, lots of white, small text, strict grid, photos at different scales; a serif or thin grotesque | Minimal |
| Neutral grotesque, 1 calm brand colour (blue, dark green, graphite), radii 0–8 px | Corporate |
| Grotesque, gradients, interface components (buttons, chips, cards), glass panels, radii 12–32 px | Fintech / Tech |
| Bold / wide / display fonts, 2+ saturated colours, high contrast | Bold |
| Rounded or retro fonts, pastels, hand-drawn doodles, text on a circle or wave, stickers, characters | Playful |
| Earthy and dusty colours, soft photos, grotesque 300–400, tonal combinations | Editorial |
| Warm homely colours, product in an interior and in hands, soft fonts | Lifestyle |
| Collage assets, all-caps grotesque or mono/typewriter, handwritten strokes, photocopy, flash, lookbooks | Street |
| Price tags, discount plates, retail brand book | Promo layer + base by character (mass retail — Bold, electronics — Corporate, premium — Minimal) |
| README: bank, investments, insurance, B2B, consulting | Corporate |
| README: app, service, fintech, SaaS, AI | Fintech / Tech |
| README: premium, jewellery, watches, designer clothing, studios, galleries | Minimal |
| README: car dealer, car brand, car service | Auto layer + base by character (premium — Minimal, mass — Bold or Corporate) |
| README: developer, residential complex, real estate, architecture firm | Real Estate layer + Editorial, Minimal or Corporate |
| README: interior, furniture, lighting, finishing materials | Lifestyle / Home (premium — Minimal) |
| README: kids, cafés, desserts, toys | Playful |
| README: home appliances, cookware, textiles, home and living goods, packaged products | Lifestyle |
| README: restaurant, café, coffee shop, bar, food delivery, fast food, patisserie | Food + a second preset (see the Food card) |
| README: fashion, footwear, youth, streetwear | Street |
| README: cosmetics, skincare, make-up, hair dye, salons | Beauty layer + Editorial (or Minimal, Cute, Health — by character) |
| README: water, natural products, wellness "about sensations" | Editorial |
| README: local brand with a strong national identity, public sector, culture | + Cultural code layer on top of the base |
| README: health, supplements and vitamins, nutrition, clinics, labs and tests, telemedicine, pharma, science-based wellness | Health |
| Deep tonal palettes (forest green, wine, terracotta), mono labels, scientific diagrams, macro textures | Health |
| README: energy drinks, delivery, mass-market services, sport | Bold |

**Layers.** Food, Promo, Beauty, Auto, Real Estate, Holidays and Cultural code aren't a brand character but layers: they always sit on top of the base preset. First choose the base preset by the steps above, then add layers by sphere, occasion and pillar. The base sets the approach (fonts, grid, energy, amount of decoration), the layer — its elements and hierarchy. Layers can be stacked: "Food + Street + Promo" — a burger chain's promotion.

## Combining presets

A brand can take devices from several presets. One rule: **one base preset sets the language, the others contribute individual devices.**

- **Base** — fonts, colour, photo character, grid, graphics. Always one, so the feed looks like one brand.
- **Additional (1–2, no more)** — only what's named explicitly: a visualisation type, specific layouts, a device (e.g. chips from Fintech, the "meaning → visualisation" table from Corporate). An additional device is drawn in the base preset's colours and fonts.
- **By pillar** — separate pillars may follow another preset: promotions → + Promo layer, reports and numbers → Corporate. Fonts and colours still come from the brand, so the feed stays coherent.

**How to record** in the Design System README or project instructions:
"Preset: Health. Additionally: Corporate — data visualisation and L19; Fintech — chips. Pillar 'Promotions' → Promo."

**Conflicts.** If base and additional disagree — the base wins, except for devices explicitly named in the record. A layout ban in the base is lifted only if the additional preset is named for that layout. Layer A, the brand and "Style from practice" outrank both.

**Combine poorly** (check before mixing): Minimal + Street / Bold; Playful + Corporate; Street + Corporate. Minimal + Promo — only a quiet sale per the table in the Promo card. Good: Health + Corporate, Health + Fintech, Corporate + Fintech, Editorial + Lifestyle, any preset + layers.

**When choosing a preset:** if the brand's signals honestly split between two presets, propose a combination ("base Health, additionally Corporate for numbers") rather than picking one at random.

In the summary after the work state what was taken from which preset.

## Extending presets with your own boards (optional)

The presets were compiled from analysing several hundred references in total (dozens per preset and layer). You can keep refining them with your own Pinterest boards: name them by convention and give the profile link once (it's saved in memory or the project instructions).

| Board name | Feeds |
|---|---|
| `composition` | Editorial + the by-composition foundation |
| `preset-corporate` | Corporate |
| `preset-tech` | Fintech / Tech (and Friendly Tech) |
| `preset-health` | Health / Science |
| `preset-bold` | Bold / Pop (all sub-styles) |
| `preset-minimal` | Minimal |
| `preset-cute` | Cute / Playful |
| `preset-street` | Street / Fashion |
| `preset-home` | Lifestyle / Home |
| `preset-beauty`, `preset-auto`, `preset-real-estate`, `preset-holidays`, `preset-cultural`, `preset-food`, `preset-promo` | the matching layers |
| `motion-design` | the by-motion technique library |

A new `preset-…` board = a candidate for a new preset or sub-style. When asked to "analyse the boards" (or on a weekly scheduled task the user sets up), open each board in the browser, look at pins added since the last analysis (new pins are on top; keep a small table "board · pins at last analysis · date" in memory or the project), and propose edits to the cards: a new device, a new layout number, a refined rule. Edits are applied only after the user's OK.

## Sphere and occasion layers

Like Food and Promo: a layer sits on top of the base style. **The approach (fonts, grid, energy, amount of decoration) comes from the base preset, the sphere's elements and objects — from the layer.** Objects from the base preset are translated into the sphere's language (like tags → receipts in Food). Record: "Preset: Editorial + Beauty". Layers can be stacked ("Minimal + Real Estate + Promo"). Layer devices are drawn in the base preset's language: if a device breaks it (plates in Minimal), take another device from the layer. A sphere without its own layer (events, education, etc.) is served by the base preset — most often Corporate.

**General layer rules**
- **Layers don't change layer B on their own.** Handwriting, all caps, centring, text on a circle — only if the base preset or the brand allows it; otherwise take another device from the layer. Fonts and tones in layer cards ("serif", "black slides", "dark tones") are observations from references: font and colour remain from the brand and the base preset.
- **The base preset's layout bans apply to layers too:** take only non-banned layouts from the layer's list. L17 via Promo is allowed in Health, Corporate, Fintech, Bold, Playful, Street, Lifestyle; in Minimal and Editorial instead — a "quiet sale" (L37 or L3 with a small price).
- **How many layers.** As many as suit the post (e.g. a burger chain's promotion for a national holiday: Food + Promo + Holidays + Cultural code). Each layer must be needed by this particular post — don't add a layer "for flavour". Hierarchy is set by Promo if present, otherwise by the sphere layer; occasion layers (Holidays, Cultural code) add 1–2 elements each. The layout is overloaded — remove elements of the layer least important for the post, but not the promotion's hierarchy.
- **Layers in Bold** are drawn with the chosen sub-style's means: bursts and plates — only in Pop graphics, Text plates and Asian poster; in 3D — a volumetric percentage; in Y2K — a "TV shop" price plate.
- **Illustrations and marks.** Complex illustrations, ornamental marks and diagrams — from the Design System or the client; otherwise a placeholder and a list of "what to draw or generate", anything generated is noted in the summary. Simple shapes are drawn right away. Recognisable buildings and monuments — from the client's photos, not from memory.

### Beauty
Board for refinement (optional): `preset-beauty`.
- **For whom:** cosmetics, skincare, hair dye, make-up, beauty salons, nails. Common pairs: Editorial + Beauty, Minimal + Beauty, Cute + Beauty, Health + Beauty (dermocosmetics).
- **Elements:** swatches and textures large; a shade palette with numbers (for hair dye — strands or colour plates labelled like a catalogue); before/after — only the client's real photos, same light and angle, no retouching of the result; "how to apply" in steps; ingredients and actives; the product in hand and on skin.
- **Attention:** the shade colour isn't distorted by preset filters or toning; effect claims — only from the client's text. Don't generate skin, hair, the result or the shade on a person (A9). Study percentages — only from the client, with a footnote (who, how many people, when). Paired with Health, before/after — only skin or hair in close-up, with the client's and the person's consent, without promising a medical result; figure and body — never.
- **Devices from references:**
  - **Swatches next to the product:** products in a column or row, each with a smear or drop of its shade and a thin callout with the name; a palette — circles in a row with captions "for lips / for cheeks".
  - **Actives as drops:** ingredients — drops, bubbles or raw materials (oil, fruit, leaf) large, thin captions with their action next to them; concentrations — a chain "1.5% → 3.5% → 5.5%" above the product; study results — a row of numbers (96% · 93% · 90%) with a footnote per A6.
  - **Concerns as chips on skin:** a large portrait, translucent pill chips on zones ("dullness", "uneven tone"), each with a line to the zone.
  - **Product card over a portrait:** a full-frame portrait, the product on a white or light card covering part of the frame (not the face); the set's name large next to it.
  - **Routine by time:** narrow horizontal frame strips one under another, each with a time (08:00, 13:30, 21:00) and the moment of use.
  - **Still life with a natural object:** a bottle on a stone, an orange, a leaf; shadow and reflection; no text or a caption in a corner. Macro skin with drops and textures (foam, a smear of cream) — as separate carousel slides.
  - **Reviews as a chat:** question and answer bubbles, customer photo circles — only the client's real reviews.
- **L51. "Yes — but".** The frame splits horizontally in half: on top the problem large (dry hair, scalp, a comb) captioned "yes, dryness", below — the ingredient in nature captioned "but — moringa". Captions small, centred on the dividing line. A series of 4–6 posts in one grid.
- **L52. Callouts on a face.** A portrait in the centre; thin lines from zones (cheekbones, lips, eyelids) to product names or to the products themselves at the frame edges ("shop the look"); variant — handwritten marks on the photo, like a make-up artist's notes. Lines don't cross the eyes or each other.

### Auto
Board for refinement (optional): `preset-auto`.
- **For whom:** car dealers and car brands, car service, car accessories.
- **Elements:** the car is the hero of the frame, classic angles (3/4 front, profile, detail), dynamics, interior; specs as large numbers per A7; trim levels as a comparison; test drive and showroom address.
- **Attention:** the car and logo aren't generated (A9), the body colour doesn't change; credit and leasing terms — as legal text per A6. Specs, range, prices, rates and body colours — only from the client or the model's official website, with the source.
- **Devices from references.** The car is almost always shown through life and swipe play, not as a showroom:
  - **Range and numbers in a thin font:** 2–3 numbers in a row over a landscape or the car (835 km · 770 km · 760 km) with small trim captions.
  - **Handwritten notes over a trip:** a documentary photo of the road or a stop, arrows and short handwritten captions to details (360 camera, boot, "100% electric"), the route drawn as a line; interface elements (a voice message, a navigation card) in frosted-glass style fit.
  - **Colour choice:** the car in profile, below it circles of body colours like a configurator — only the model's real colours.
  - **Words around the car:** short scenario words over the free field around the frame ("beach", "cottage", "concert").
  - **The rate large:** "3.7% per year" — the hero per L17, the car below it, terms per A6; for holidays — the car "wrapped" as a gift (only if the client provides the photo or edit).
- **L53. Guess the model.** Cover — a question ("Which model is this?") over the interior; slides 2–4 — one detail each with a "Hint 1…" tag and "swipe on"; ending — the whole car, the name and one benefit.
- **L54. Lines in the cabin.** A series of interior shots; on each — one line as a messenger bubble ("coffee run?", "where do we put our stuff?"), the detail itself answers (cup holder, boot). The bubble sits away from the main detail.
- **L55. Camera pull-back.** Slide 1 — a fragment (view from the window, a detail) and the caption "swipe to zoom out"; each next one is wider; ending — the wide shot and a benefit headline ("First-class seats"). A reverse-psychology variant: "don't swipe…" → "seriously" → "since you're swiping" — a thin caption in the centre of trip shots.

### Real Estate
Board for refinement (optional): `preset-real-estate`.
- **For whom:** developers, residential complexes, real estate agencies, rentals, architecture and construction firms.
- **Character from references:** not "selling square metres" but an editorial story about architecture, materials and people: a serif or thin grotesque, dark and warm tones, lots of air, little text on photos. Most often paired with Editorial, Minimal or Corporate.
- **Elements:** renders and photos of the property, floor plans (clean, with areas), a location map with times to points, construction progress by date, amenities as chips or icons, purchase terms.
- **Attention:** prices, areas, completion dates and instalment/mortgage terms — only from the client, legal text per A6; a render is labelled as a render if the client does so.
- **Devices from references:**
  - **A quote in the air:** a short serif phrase in quotation marks ("Location, location, location", "Architecture is also emptiness") over a minimal interior or light field, the author and continuation small in italics.
  - **Material details:** a series of close-ups — wood, lit niches, wall texture, a hand touching a surface; one short phrase in the centre or no text (like L44).
  - **Property name across two frames:** the complex's name in a huge thin font runs from one photo to the next (facade and detail), captions small in the corners.
  - **Numbers as a strip:** 3–4 numbers ("98% · 5 min · 12 years · 24/7") in a thin font on a colour plate or over a photo, captions under each.
  - **Grid of spaces:** 4 photos of zones with captions ("lobby", "courtyard", "gym", "co-working") or website pages as slides in a phone mock-up.
  - **A drawing over a photo:** thin lines of a drawing, facade or perspective grid laid over a render or an empty floor — to show the intent.
- **Layouts:** L61, L62, L63, L44, plus the base preset's layouts.
- **L61. Property and numbers.** A render or photo of the building full frame, the tower or facade shifted to the edge; the name large on top; in the free sky — 2–3 numbers in a very thin font (floors, apartments, minutes to the centre) with small captions; a promise phrase at the bottom. Numbers — only from the client.
- **L62. Construction explained.** A construction-progress carousel: cover — a documentary photo of scaffolding or the frame and a question in 2–3 lines ("Can less… do more?"); then full-frame photos alternate with black slides of the architect's explanation as a paragraph and a small photo; ending — the finished interior. Logo and pillar as a line on top in one place. Stage dates — only real.
- **L63. Focus frame.** A b/w documentary photo with people (residents, builders, neighbours in the courtyard); one person in a thin square frame in the accent colour, next to it a short caption in the same colour in caps ("for her", "for him"). The series rests on one frame and one phrase. A universal device — fits any brand's community. Only real photos with the consent of the people in frame.

### Holidays and season
- **For whom:** any brand. The calendar depends on the **brand's market** (from design settings or the brief; ask if unclear) — take the market's own holidays plus global ones. Examples by market:
  - **US:** New Year's, Valentine's Day, Super Bowl, St. Patrick's Day, Easter, Mother's Day, Memorial Day, Pride Month, Father's Day, Fourth of July, back to school (August), Labor Day, Halloween, Thanksgiving, Black Friday and Cyber Monday, Small Business Saturday, Giving Tuesday, Hanukkah, Christmas, New Year's Eve.
  - **UK:** Pancake Day, Mother's Day (March), Easter, bank holidays, summer holidays, Bonfire Night, Black Friday, Christmas markets, Boxing Day.
  - **Continental Europe:** Carnival / Fasching, Easter, Mother's Day (May in most countries), Midsummer (Nordics), summer and winter sales seasons, St Nicholas (6 December), Christmas markets, Three Kings (6 January, Spain).
  - **Kazakhstan / CIS:** New Year (the main winter holiday), 14 February, 8 March, Nowruz (21–23 March), 1 September, Independence Day, Black Friday, local city days.
  - **Japan:** Shōgatsu (New Year, the biggest holiday — nengajō cards, osechi, fukubukuro lucky bags), Coming of Age Day, Valentine's Day (women give chocolate), White Day (14 March, return gifts), sakura / hanami season (late March–April, forecast by region), new school & work year (April), Golden Week (late April–early May), rainy season, Tanabata (7 July), summer festivals and fireworks, Obon (mid-August), autumn leaves (kōyō), Halloween, Black Friday, Christmas (a couples' holiday + Christmas cake and fried chicken), year-end parties (bōnenkai).
  - **South Korea:** Seollal (Lunar New Year), Valentine's Day, White Day (14 March), Black Day (14 April), Children's Day (5 May), Parents' Day (8 May), Teachers' Day, cherry blossoms, summer vacation, Chuseok (autumn harvest holiday), Hangul Day (9 October), Suneung exam day (November), Pepero Day (11.11), Christmas (couples), year-end.
  - **China / Greater China:** Spring Festival (Lunar New Year, red envelopes), Lantern Festival, 520 (20 May, "I love you"), 618 shopping festival, Dragon Boat Festival, Qixi (Chinese Valentine's), Mid-Autumn Festival (mooncakes), National Day Golden Week, Double 11 (Singles' Day).
  - **Southeast Asia:** Lunar New Year, Ramadan and Hari Raya / Lebaran, Songkran (Thailand, April), 9.9 / 10.10 / 11.11 / 12.12 mega sales.
  - **Global / cross-market:** Lunar New Year, Ramadan and Eid, Diwali, International Women's Day, Earth Day, Singles' Day 11.11, World Kindness Day.
- **Works as a layer:** the brand stays itself, the holiday adds 1–2 recognisable elements (a symbol, a seasonal object, an accent colour within the palette) and an occasion in the text. No stock clichés (clip-art trees, pumpkins and turkeys from stock, ready-made card templates). National holidays and state days — together with the Cultural code layer.
- **Sensitivity:** religious and cultural holidays — only if the brand marks them, with respect and without making them a sales gimmick (Ramadan, Hanukkah, Diwali, Easter); heritage and remembrance days (Memorial Day, Juneteenth, MLK Day, Veterans Day) — respectful tone, no "sale" framing unless the client insists and it's common practice in the market; Pride — only if the brand genuinely supports it.
- Board for refinement (optional): `preset-holidays`. References fall into three groups: cultural and national (national holidays, city day, statehood days), spring and seasons, autumn and winter holidays.
- **Cultural and national:**
  - an ornament or textile as the poster's framework, an invitation in a carpet frame;
  - stills from classic national cinema with the title and year — only with rights;
  - a dense illustration of the city for City Day (many recognisable buildings, the date and slogan large);
  - the city's architecture in arched window fragments or shot upwards under a large name.
- **Spring and seasons:**
  - one flower — as a cut-out, a line on a flat background, pressed in a notebook or with a tag;
  - a botanical drawing over a vintage photo;
  - four seasons as quarters of a circle;
  - a photo in a postage-stamp frame;
  - a polaroid with a handwritten note over a bouquet;
  - words formed by a stem or flowers.
- **Halloween and autumn (US and growing worldwide):**
  - the product "in costume" or as a jack-o'-lantern cut-out, drawn by the brand's own means, not stock pumpkins;
  - a spooky-cute palette within the brand colours (one dark tone + one accent), drawn outline ghosts, bats or spider webs over a photo;
  - Thanksgiving: a long shared table from above, "what we're grateful for" lists, a recipe card; Black Friday / Cyber Monday — via the Promo layer.
- **New Year and winter:**
  - a December calendar with handwritten notes — an advent calendar or promotions schedule;
  - drawn outline gifts over a photo of a person;
  - text around a Christmas bauble;
  - a large word ("Garland") over a warm photo of a tree;
  - a geometric tree made of stacked shapes;
  - a seasonal lookbook as a series of frames from one shoot;
  - an illustration of a festive table;
  - aeroplane windows with a winter view — for travel.
- **Attention:** occasions about tragedies, wars and charity — no festive decor or promotions, only in agreement with the client. Religious and heritage days — see "Sensitivity" above.
- **Layouts:** L64, L65, L66, plus the base preset's layouts.
- **L64. Gift guide.** A carousel: cover — a "Gift guide" card over a winter photo; then on each slide one set on a paper card with a clip or perforation: a handwritten title ("Set A"), who it's for, 2–4 cut-out items, the price or a "budget" in a circle. One background for the whole series.
- **L65. Photo inside a symbol.** The brand's photos and moments fit into the holiday's shapes (baubles, portholes, arches, petals); next to them a large headline — handwritten or serif — and the event date small.
- **L66. Holiday palette.** Two to four colour plates as shade cards with names ("Olive grove", "Rose petal"), or a mood illustration headed "The season's palette". For design, interior, cosmetics and fashion brands; colours — from the brand's palette or products.

### Cultural code
Board for refinement (optional): `preset-cultural`.
- **For whom:** local brands with a national identity, the public sector, national holidays, collaborations with culture. The motifs come from the **brand's market** (the user's local market by default; ask if unclear).
- **Principle:** stylish and contemporary, not souvenir-like. The ornament works as a grid, texture or detail, not a border along the edge; local textures and objects; text in the national language — with a check of all the font's glyphs (A11).
- **Translating foreign examples.** References from other cultures are a model of approach, not of motifs: take the device (how a Chinese Year of the Horse poster builds typography around a sign, how an Uzbek tea bowl becomes the hero of an illustration), while the signs, objects and words come from the brand's own culture. Ornaments of one culture aren't transferred to a brand of another.
- **Motif hints for East Asia** (starting points, verify with the client): **Japan** — wagara patterns (seigaiha waves, asanoha hemp leaf, ichimatsu checks, shippō), noren curtains, washi paper, hanko red seal stamps, cranes, maneki-neko, sakura, Mount Fuji, ukiyo-e flat colour and line, vertical text; **Korea** — dancheong colour patterns, obangsaek five colours, hanbok silhouettes and fabrics, bojagi patchwork, hanok roofs and lattice doors, celadon, the taegeuk curve (state symbol — not as decor), minhwa folk painting, Hangul letterforms as graphics; **China** — cloud and lattice motifs, red and gold, paper-cut (jianzhi), the zodiac animal of the year, lanterns, ink wash.
- **Motif dictionary.** Build it for the brand's culture before the first post: ornaments, animal symbols, dwellings and architecture, household objects, textiles, food rituals, instruments, flowers and landscape, rock art. Ask the client or a cultural source; don't invent "pseudo-national" patterns. **Worked example — Kazakh:** қошқар мүйіз and other ornaments; animal symbols (argali, tazy hound, horse, golden eagle, swallow, bird); the yurt, shanyrak (per the sacred-symbols rule below), kebeje chest, syrmak and tekemet felt carpets, tea bowl, kazan, dastarkhan, dombra, tulips and the steppe, petroglyphs.
- **Devices from references:**
  - **Sign silhouette:** an animal or bird assembled from ornament curls as a flat silhouette — like a logo; one sign per frame, lots of air.
  - **Ornament in a modern material:** extruded 3D, frosted glass, chrome, a keychain pendant, embossing on paper — instead of a flat appliqué.
  - **Pixel and embroidery:** an ornament or animal assembled from small squares, like cross-stitch or pixel art; often in red over a b/w archive photo.
  - **Archive + graphics:** an archive b/w photo (portrait, everyday life) with a bright ornament on top that fills the clothing or runs through the frame; a quote or historical text small next to it.
  - **Cut-out:** the ornament as a paper or felt cut-out, a patterned silhouette over a photo or splitting the frame in two halves.
  - **Sign set:** 6–9 ornament elements in a grid like stickers or icons — for pillars, highlights, merch.
  - **White icons over a landscape:** a dwelling, horse, flower, bird as white cut-out silhouettes on a photo of the landscape; the headline large on top.
  - **Naive painting and everyday illustration:** a festive table, stacked bowls, a cauldron; a handwritten italic caption — a warm phrase or joke in the national language.
  - **Pixel-ornament construction:** a huge ornament element made of squares, cropped by the frame edges — as the poster's architecture; text in columns in its voids. Variant: the squares "dissolve" the edge of a photo, turning into the background.
  - **Woven ribbons:** ornamental belts and strips bend, fold into a wave, a number or a letter; a flat background.
  - **Name over a pattern:** large letters of the name spread across the whole frame, dense ornament in 2–3 colours between and beneath them.
  - **Silhouette with texture:** simple silhouettes (a tulip, a jug, a branch) filled with the texture of a carpet or embroidery.
  - **Monochrome and embossing:** the ornament tone-on-tone with the background, in barely visible relief — for calm and premium brands.
  - **Engraving of everyday life:** a b/w illustration in linocut manner (festive table, national dish, bowls) with a caption in large letters below.
  - **Stamps with photos on a landscape:** red square stamps with cut-out photos and short words scattered over a landscape photo.
  - **Ornament frame for a series:** in a post grid, faces or products in identical ornamental frames — the series rests on the frame.
  - **Bilingual:** the national language and a second language in different weights of one font, the national language leads.
  - **Vertical carriers:** bookmarks, labels, tickets with an ornament frame and a photo window — for packaging, merch, invitations.
- **Layouts:** L56, L57, L58, L60, plus the base preset's layouts.
- **L56. Sign in the centre.** One large symbol (an animal silhouette made of ornament, an element in 3D or chrome) centred on a flat background, taking 40–60% of the frame; the headline or greeting small above or below, in the national language and, if needed, a second language. For national holidays and announcements.
- **L57. Archive and ornament.** An archive or documentary b/w photo full frame; an ornament in the brand colour fills clothing or an object or runs as a strip (pixels are OK); text — a quote, fact or date — as a column in a free zone. Photos only with rights (the client's archive, a museum with permission).
- **L58. Household object as hero.** An illustration or photo of one object (a bowl, a cauldron, a chest, an instrument) in the centre, with the brand's story inside or around it (flowers, a mini house, the product); a handwritten italic caption below. A series of 3–6 objects in one manner.
- **L60. Cell grid.** The frame is a 4×5 or 3×4 grid: some cells hold engravings, object photos or ornament, the rest — the headline, dates and text broken across cells. Background colour — one from the brand palette, thin grid lines. For exhibition, festival and event announcements.
- **Attention:** sacred and state symbols (coat of arms, flag, sacred architectural symbols) aren't distorted or used as decor without agreement. National-language text (greetings, jokes, captions) — from the client; your own version is only proposed in the summary marked "have a native speaker check". Ornaments — from the motif dictionary, no invented "pseudo-national" patterns; a sign "like a logo" doesn't replace the brand's logo.

## Default fonts

Only if the brand has no fonts of its own. The first five groups are Google Fonts with Latin and Cyrillic; for languages with special letters still check A11.
- Neutral grotesque: Inter, Manrope, Onest, Golos Text.
- Wide / display: Unbounded, Montserrat Alternates, Rubik.
- Serif: Playfair Display, Cormorant, Lora, PT Serif.
- Rounded: Nunito, Comfortaa, M PLUS Rounded 1c.
- Monospace (service): JetBrains Mono, IBM Plex Mono.
- Japanese: Noto Sans JP, Zen Kaku Gothic New, M PLUS 1p (sans); Noto Serif JP, Shippori Mincho (mincho). Korean: Pretendard (not on Google Fonts — use it only from a CDN or the brand's files, otherwise Noto Sans KR), Noto Sans KR, IBM Plex Sans KR (sans); Noto Serif KR, Nanum Myeongjo (serif). Chinese: Noto Sans SC / TC, Noto Serif SC / TC. Pair a CJK font with a Latin font of similar weight and check that numbers and Latin letters look consistent.

## Preset cards

### Neutral — base
- **For whom:** a fallback when the style isn't determined; service and informational posts of any brand.
- **Character:** clean, calm, no pronounced mood.
- **Typography:** neutral grotesque 400–500, headline 500. All layer B defaults.
- **Colour:** light background (white or very light grey), dark text, 1 accent.
- **Photo:** natural, unstylised; plays the lead, text beside it.
- **Graphics:** minimal — thin divider lines, no decoration.
- **Layouts:** all L1–L15.
- **Changes in layer B:** nothing.

### Editorial / Soft
Board for refinement (optional): `composition`.
- **For whom:** wellness, cosmetics and skincare, water, natural products, brands "about sensations".
- **Character:** soft, editorial, lots of air, quiet.
- **Typography:** grotesque 300–400, accent by size, not weight. A two-tone headline: the first part in the main colour, the continuation quieter ("Anyone can launch. Few launch to last."). A serif as a rare accent: quotes, large numbers, one italic word in a grotesque phrase ("*Balance* your barrier").
- **Colour:** natural, earthy, dusty; at most one bright accent. Tonal typography — text in a shade of the background colour (contrast per A8).
- **Photo:** soft natural light, shallow depth of field, muted colours; blur and gradient instead of flat fill. The product in its environment: moss, an ingredient, a texture.
- **Graphics:** thin lines and rings, outline tags.
- **Layouts:** best L1, L2, L3, L5, L6, L7, L8, L13, L14. Don't use L17.
- **Changes in layer B:** nothing.

### Corporate
Board for refinement (optional): `preset-corporate`.
- **For whom:** banks, brokers, insurance, consulting, B2B, business education, the public sector.
- **Character:** modern corporate — clear, structured, calm, but not boring. **The main thing — the meaning of the text is clear to everyone, and it's shown visually.**

**Text and structure**
- The text is written very simply and clearly: short sentences, no officialese or unexplained terms.
- A strict slide structure: (a section tag per A6, if needed) → **headline** → **body** → **visualisation of the meaning**. Headline and body are always separated by size and spacing.
- There can be more text than usual: body up to 60 words, up to 80 in total per artboard — but only structured: paragraphs up to 3 lines, lists as numbered lines with thin rules.
- **Lots of text — don't add a picture "just because".** Better a clean text slide (L19), a visualisation of the meaning or more carousel slides. A photo is used only when it says something itself (speaker, team, place, product).

**Visualising the meaning — the preset's main device**
Not only numbers (those per A7) but any structure present in the text. The visual is built from the text, not added on top for beauty; decorative illustrations without meaning aren't used.

| In the text | Visualisation |
|---|---|
| process, steps, "first… then…" | 3–5 steps: cards on a line or growing bars, the last step in the accent colour (L21) |
| a list of points, questions, principles | numbered lines with thin rules and a small accent-colour tag ("01 / Goal") (L19) |
| comparing two options | two columns or two blocks of different tone, the same structure in each |
| a system of parts, an ecosystem | cards in a grid or a diagram with nodes |
| data, shares, growth | per A7: a row of numbers, bars, a ring, dots |
| deadline, speed, time | a scale or a dial arc with the exact value |
| a simple statement without structure | no visualisation needed: large headline + text (L3, L5) |

**Typography**
- Neutral grotesque; headline 400–600, sentence case; body 400. Serif — only if it's in the brand book.
- Accent — the brand colour on key words of the headline (one phrase: "Withdrawal **in two hours**") or a two-tone headline (continuation in grey).
- A large quote — with hanging quotation marks in the brand colour.

**Colour**
- Light backgrounds (white, warm white, light grey) or a deep brand colour (dark green, graphite); one brand accent colour.
- Soft gradients are OK in visualisations (bars, cards) if they don't contradict the brand.

**Photo**
- Real people: speakers, experts, the team. A clean portrait, calm light, a plain or blurred background, looking into the camera or natural. No staged stock and no "smiles at the camera".
- The face is clear per A12 (by-composition): text to the side or below, a large headline above the head or over clothing. Name and role — as a small caption or a neat plate at the edge of the photo.
- Documentary shots of the office and work — if they're about the post's topic.

**Graphics**
- A visible grid: thin divider lines, numbering, cards. Line icons of one weight. Radii 0–12 px.

**Layouts:** L19, L20, L21, L9, L4, L5, L3, L10, L15, L14, L8. Don't use L13, L18.

**L19. Structured text.** Headline in the top third; 1–2 lines of explanation below it; below that 2–4 numbered lines separated by thin rules: a small accent-colour tag ("01 / Goal") + the point's text. No photo.

**L20. Speaker / expert.** A portrait at 50–65% of the height, the face clear (A12). Beside or below it — the topic or a quote (headline), name and role small. For podcasts, interviews, webinars, mentor cards and introducing the team. Variant: the quote on top, below it a card with a small portrait, name and role.

**L21. Process.** Headline and 1–2 lines of text on top; in the lower half — 3–5 steps from left to right (cards on a line of equal height; growing bars — only if the text has growth in numbers, otherwise for a broker they read as returns) with short captions; the final step in the accent colour. Steps come from the text, not invented.

**Changes in layer B:** headline up to 600; colour accent on the headline's key phrase instead of B3; text limit up to 60 / 80 words with structure (see A1).
**Attention:** for financial brands legal text per A6 is almost always needed — check.

### Fintech / Tech
Board for refinement (optional): `preset-tech`.
- **For whom:** apps, fintech services, SaaS, AI services, online platforms, digital products.
- **Character:** digital, modern, "like an interface". As in Corporate, **the text's meaning and data are visualised**, but in the language of an interface: buttons, chips, cards, notifications, flows. The difference from Corporate: there strict tables and thin lines, here live product elements, radii, glass, gradients.

**Text and structure**
- The same structure as Corporate: headline → body → visualisation; the text is simple and clear. Word limits — basic (A1): here meaning is shown more than described.
- A section tag per A6 can be styled as a chip ("Research", "Mission").

**Visualisation in the language of an interface — the preset's main device**

| In the text | Visualisation |
|---|---|
| process, automation, a chain of actions | a flow: node plates connected by lines, the active step in the accent colour (L24) |
| checklist, instructions, "how to" | a list with numbers in circles or checkboxes inside a card |
| features, capabilities, categories, segments | chips / tags (2–4) around a person or product (L23) |
| a user action ("sign up", "send") | an interface fragment with a button (L22) |
| result, event, review | a notification card or a chat message |
| data, growth, shares | per A7: bars, a 100-dot grid, large numbers "+10K"; chart points labelled with tooltips |
| connections, team, network | a grid of nodes with avatars and chip captions |
| a question to the audience | a search bar or input field with the question |

Interface elements are content, not decor: every chip, button or node carries a word from the text. No empty buttons or chips "for show". No more than 4–5 interface elements per slide. A button inside a product demo is part of the visualisation; a real call to action (CTA) — per A6.

**Real product vs abstract interface.** Full screens and phone mock-ups — only with the client's real product (screenshots from them). Abstract elements (a chip, button, card, node) can be drawn as a visual language, but they must not pretend to be a real screen with invented data (amounts, balances, rates — only from the text or the client).

**Typography**
- A clean grotesque, headline 400–600, sentence case, tight tracking. A two-tone headline and a colour accent on the key phrase — as in Corporate. A serif — a rare contrasting accent in the headline, if the brand allows.
- Tabular figures (`font-variant-numeric: tabular-nums`). Text inside chips and buttons — at least 24 px.

**Colour**
- Light airy gradients (light blue, lilac, peach) or a deep dark background (dark green, black); a saturated gradient with grain — for covers.
- 1 brand accent for the active element (button, active step, highlighted number).

**Photo**
- Real people in action (with a phone, at a laptop, laughing), bright and lively; the photo is often in a rounded card (radius 24–32 px).
- Interface chips around a person — at the edges of the figure, the face clear (A12).

**Graphics**
- Cards and chips with 12–32 px radii, soft shadows; glass panels (translucent background + blur) over a gradient or photo — text on them with contrast per A8.
- Icons — line or in rounded squares (like app icons), of one style.

**Layouts:** L22, L23, L24, L16, L4, L9, L19, L21, L6, L14, L15. Don't use L7, L13, L18.

**L16. Phone mock-up.** A phone with the product's real screen at 45–60% of the height, slightly turned or straight; the headline on top or to the side; 1–2 callouts with thin lines to screen elements.

**L22. Interface demo.** Headline on top; in the centre — a glass or white card with an interface fragment (calendar, form, chat, list) showing the action from the text, with one accent button; the background — a gradient or blurred photo. Below the card — 1–2 lines of explanation.

**L23. Person + chips.** A photo of a person full frame or in a rounded card; around them — 2–4 chips or mini cards with features from the text (icon + 1–3 words), placed at the edges of the figure, not on the face (A12); the headline in a free zone.

**L24. Flow.** Headline and 1–2 lines on top; below — 3–6 node plates with short captions connected by lines (left to right or top to bottom); the active or final node in the accent colour. Steps come from the text.

#### Friendly Tech sub-style — people and pillars
Modelled on business-messaging app accounts. For services and apps that speak through their customers and experts: small business, fintech for people, education, case studies, interviews. The same interface language, but warmer: instead of glass and gradients — real people, stickers and hand doodles.
- **Palette:** one brand colour in 2–3 tones (deep dark, bright, light) + cream and white. Dark text tiles alternate in the grid with photos and light tiles ("Grid plan" in by-composition).
- **Typography:** a large grotesque 400–500 in sentence case; alternating roman and italic of one family by line ("How a coincidence / *in pyjamas* / became my / *biggest drop*") — italics on meaningful words, this isn't a second font (A11). The headline can be two-tone (light brand + dark).
- **Pill stickers:** text in rounded plates with an outline, sometimes with a tail like a message and tilted 2–4°; white cards with a question or hint. No more than 3 plates per frame, text in them at least 28 px.
- **Hand doodles:** stars, curls, "spark" strokes in the brand colour, 2–3 per frame, one line weight for the whole series; a wavy or torn edge of the colour field.
- **Photo:** real people at their workplace (workshop, coffee shop, studio), documentary and warm; a phone in hand with the product's real screen.
- **Pillars with their own mark:** each pillar ("Ask an expert", "A conversation with…", "A day in the life", "Step by step") has its own lettering or plate, the same in every episode. The pillar lettering (caps, outline, arc) is a decorative mark, not a headline: up to 3 words, doesn't count toward the A11 font limit.

**L67. Cut-out hero.** A person cut out along the outline with an 8–12 px white stroke stands on a colour field (dark or light) with a wavy top edge; 2–3 doodles around; at the bottom over the clothing — a stack per L68. The face is clear (A12). For interviews, heroes, Reels covers.

**L68. Pill stack.** A caption made of 2–3 plates in steps: the pillar (brand colour, large) → a small connector ("with") → the name (white) → the role (dark, small). A slight tilt and offset of the plates relative to each other. Used on photos, on L67 and on pillar covers.

**L69. Chat over life.** A real photo or a collage of 2–3 stacked shots; on top — 1–3 product elements: a message bubble, a time stamp "8:03", a notification, a plate with the business name. A day's story or a case told through messages. Texts and times — from the client's text, no invented data.

**L70. Text tile with a sticker.** A dark or light brand field, a large headline on the left margin (sometimes with italics on words), 1–2 lines of text; in a corner — one sticker icon or object on the topic (a gift, a lamp, a trolley), slightly over the edge or on a photo in a round frame below. Covers for tips and announcements.

In motion (by-motion): pills pop in one by one with a slight bounce, doodles draw in (M9), chat bubbles appear like messages (M7). Tempo — like Playful, but calmer.

**Changes in layer B (sub-style):** up to 2 accents (italics on words + a pill); pillar lettering in caps; tilted plates. Don't use in the sub-style: glass and grainy gradients, several brand colours at once.

**Changes in layer B:** headline up to 600; colour accent on the headline's key phrase instead of B3; centred alignment is allowed in L22.
**Attention:** in fintech legal text per A6 is often mandatory — check.

### Health / Science
Board for refinement (optional): `preset-health`.
- **For whom:** supplements and vitamins, nutrition, clinics and labs, tests and biomarkers, telemedicine, pharma, evidence-based wellness.
- **Character:** "science that's pleasant to read". Calm, precise, trustworthy; the body and nature in close-up. The difference from Editorial: there sensations and atmosphere, here explaining the mechanism and evidence. The difference from Corporate: the same principle of "meaning visualised", but the language is biological (cells, molecules, organs, textures), not tables.

**Text and structure**
- An explainer carousel: a hook cover (a question or myth: "Does creatine make you bulky?", "Your eyes get more tired than you think") → the mechanism step by step → what to do → the product (if needed). Slides numbered 01 / 02 / 03, the same template for the whole series.
- The headline is one thought; the key term highlighted in bold or colour ("**Anthocyanins** are pigments that…"). The body is simple, terms explained immediately.
- **Health claims — only from the client's text or with a source.** Numbers, studies, "proven" aren't invented. Footnotes ¹ and the source — small text per A6. A medical disclaimer — if the brand or format requires it (ads for supplements, medicines); check.

**Visualising the scientific meaning — the preset's main device**

| In the text | Visualisation |
|---|---|
| mechanism, "what happens in the body" | a diagram with an organ or cell, 2–3 thin callouts with captions |
| composition, ingredients, benefits | the product or a capsule in the centre, benefits around it on thin callout lines or in circles (L27) |
| substance, molecule | a thin line formula or structure + property chips |
| path, intake, course | a route of dots and a line (mouth → gut), a "Day 1–3 / Day 4+" chart with capsules |
| before / after, with / without | two identical diagrams side by side, the difference in colour |
| statistics | cards with large numbers (95% · 70% · 37 trillion), one accented; per A7 |
| factors, habits, biomarkers | tag chips (Cortisol, Sleep, Stress) or a numbered list with mono tags |
| individuality, body data | a dot cloud along a contour (ear, hand), a wave line |

**Typography**
- A clean grotesque 300–500, sentence case, tight tracking; the accent word in bold or colour.
- A serif (incl. one italic word) — for soft large headlines and covers, if the brand allows.
- A mono font in caps — for series and section tags ("FIBRE SCIENCE", "01 / MECHANISM") and captions on diagrams; it's a tag per A6, not a decoration.

**Colour**
- Tonal palettes: the whole slide in one colour and its shades — forest green, wine/burgundy, terracotta/orange, warm sand, deep black. Text light or a tone darker than the background (contrast per A8).
- A soft glow and radial gradients (a warm spot behind a hand or product) are OK as a background.
- Within a series the colour may change by slide topic, but the diagram and grid stay the same.

**Photo**
- Macro of the body and nature: skin, eye, lips, hand, berries, leaves, moss, mushrooms, bubbles, cellular textures. Warm soft light, shallow depth of field, light grain.
- Motion blur (stress, fatigue, workout) — for emotional slides, text in a calm zone.
- Product: a capsule on a palm, a jar on a texture, the product in its environment; never generated (A9).
- The face is clear (A12); for an eye or face macro — text to the side, not on the eye.
- No frightening medical images, blood or body "before/after".

**Graphics**
- Thin 1–2 px lines across the frame, a crosshair or small diamond marker on the photo (point of interest) + a chip caption — "scientific markup".
- Rounded chips, translucent or outlined; line icons of one weight; a small logo mark in a corner is OK (per A6 — only navigation/caption).

**Layouts:** L25, L26, L27, L59, L21, L19, L1, L3, L5, L9, L14, L15. Don't use L17 (except promotions via Promo), L18.

**L25. Scientific markup.** A full-frame macro photo; a thin horizontal line at the level of the point of interest, a marker on it and a chip caption ("From week 4"); headline and 1–2 lines in a calm zone. A series keeps the line at the same height from slide to slide.

**L26. Split photo + meaning.** A macro photo on the left or top (50%), next to it a tinted block of the same colour with the headline, key term and 2–3 bulleted points. For explaining a substance or effect.

**L27. Annotated diagram.** The product, a capsule or an organ in the centre; 3–5 benefit captions around it, connected by thin callouts or in outline circles; headline on top, source small at the bottom.

**L59. Symptom → what it means → what to do.** Cover — a serif question with an italic accent ("Is your scalp telling you something?") over a large photo. Then one symptom per slide: the symptom's name in serif centred in the top third, below a mono tag "WHAT IT MEANS" and the cause in one line, at the bottom a row of three small square photo tiles with tip captions. The background — a photo of the same zone (hair, skin) with one treatment for the whole series. Causes and tips — only from the client's or a doctor's texts (see "Health claims").

**Other devices from references:**
- **Q&A letters:** huge "Q" and "A" at the left margin, the question and answer next to them as normal text; the background — a calm texture of skin or product. For a FAQ pillar.
- **Numbered facts on a dark macro:** a full-frame macro photo (bubbles, drops, fabric), 3–4 facts in small text with [1] [2] [3] markers scattered over the grid; brand and pillar as a line on top.
- **"Science + person" split:** half a microscope or lab photo, half a large fragment of a face; a question in the centre at the seam.
- **Dentistry and body care:** a large photo of a mouth or smile, two large brand words above and below the frame around the face, or typewriter text centred over the photo.

**Changes in layer B:** accent in bold or colour on the key term instead of B3; mono caps for series tags; centred alignment is allowed in L27.
**Attention:** advertising of supplements and medicines is regulated in many markets — check the disclaimer and wording with the client.

### Bold / Pop
Board for refinement (optional): `preset-bold`.
- **For whom:** energy drinks, beverages, food and delivery, fast food, taxis, mass-market services, sport, youth brands, events, sales with character.
- **Character:** loud, bold, with humour; seen in half a second. The freest preset: lots of graphics, illustrations, textures, play with type. That's exactly why the aesthetics are chosen strictly.

**Umbrella rules**
- **The brand chooses one sub-style** (table below) and records it: "Preset: Bold / Scrapbook". Fonts, graphics, textures come from it. A second sub-style — only per "Combining presets", stating what exactly is taken from it.
- **Don't mix sub-styles in one layout.** The sub-style isn't named — determine it from the brand and references; unsure — ask or show the cover in 2–3 sub-styles side by side.
- **Freedom is in the graphics, not the text.** Tilts, curves, overlaps, collage, stickers — fine. Layer A — no exceptions: the main text reads at 375 px, the reading order is kept (A2), faces are clear (A12), decoration doesn't crawl over text and product. A curved or tilted line — only for a headline of up to 5 words; body text is straight.
- **One hero per layout:** headline, product or person. Everything else is surroundings and noticeably smaller.
- **Illustrations, stickers and 3D assets** — from the brand's Design System or the client. None — propose a list of what to generate or shoot, and leave a neat placeholder in the layout. Simple vector graphics (rays, bursts, circles, confetti, doodles, frames) are drawn right away. Product and packaging aren't generated (A9). Others' characters and logos aren't used.
- **Humour is in the text and delivery:** short bold phrases, lines in bubbles, a dialogue with the reader, repetition with variation in a series ("Meetings can wait. Cleaning can wait. The sale can't").

**Sub-styles**

| Sub-style | Typography | Photo and graphics | Colour in references (example; palette — from the brand) |
|---|---|---|---|
| **Text plates** | bold grotesque; words or phrases on separate colour highlight plates, scattered in steps | a full-frame photo of a person; emotion stickers (eyes, lines), cut-out photos | lime / yellow plates + black text |
| **Curved type** | retro display or a bold condensed grotesque, in an arch or wave, volume / shadow / outline | photos through a fisheye or a strong wide angle, the line follows the frame's curve (L28) | scene colours + yellow/white type |
| **Scrapbook** | lowercase grotesque, label captions on plates, chat bubbles | photo cards in thick colour frames askew, a cut-out product, food large in hand, a street background (L30) | blue / yellow / red frames |
| **Asian poster** | huge characters (Hangul, Chinese characters) or Latin/Cyrillic in the same manner over the whole background. Characters always mean something: the brand name or the post's gist (1–3 words) translated into Korean, Chinese or Japanese; in the summary — the back-translation and a note "have a native speaker check"; a font with the needed characters (A11). Meaningless characters for decoration — no; a small info block | repeating cut-outs and patterns, burst badges, flat illustrations, colour circles over photos | red, yellow, green, pink, high contrast |
| **Pop graphics** | a very bold condensed or wide grotesque, caps up to 4 words, headline 50–70% of the artboard; large lowercase colour words over a photo | a cut-out person or product on colour, burst rays, confetti, doodles, a grid of colour cells with product photos | 2–3 saturated: lime, red, pink, blue |
| **Y2K (00s)** | a classic serif centred (short headline + tagline), a bold magazine logo, small text columns like a magazine; for the "screen" variant — a techno grotesque | print ads of the era: a hero product at surreal scale or fanned colour versions (L33); a magazine portrait with flash, wind in the hair, headphones and gadgets; an outfit breakdown with circle callouts (L34); confetti dots and cut-out stars over a photo; a "TV shop" frame (low resolution, price and phone number on a plate); magazine scan texture, grain; as an accent — chrome and gloss | warm film tones or clean white; hot pink, red, pastels |
| **3D** | a clean bold or rounded grotesque, large; "inflated" 3D letters — only for 1–2 headline words | soft toy-like shapes: inflated icons (star, arrow, heart), matte clay and soft-touch, glossy plastic, chrome or iridescent foil accents, clear glass; fluffy textures (felt, pompoms); soft studio light, soft shadows (L31, L32) | often a simple plain background (light, dark or juicy) with contrasting objects on it; specific colours — from the brand |

**3D — sub-style rules**
- 3D objects carry meaning: a star = the best, an arrow = a transition, category objects = the assortment. They replace flat icons rather than being added to them.
- One set of materials per series (e.g. matte clay + one chrome accent) and one light — otherwise the objects look gathered from different stock banks.
- The background doesn't compete with the objects in complexity (any brand background colour), text in a calm area; 3D doesn't cover headline lines (only touching the edge of a letter is OK if the word reads in full).
- Product renders — only from the client (A9). Abstract 3D shapes and icons may be generated: first propose a list of objects with material and colour, placeholders of the right shape in the layout.

**Y2K — sub-style rules**
- This is a stylisation of late-90s – 2000s print and TV ads: a simple idea, one hero product, a short headline, a tagline and the logo at the bottom. A centred composition is OK.
- The "00s" texture (grain, scan, low-res TV frame) goes on the background and photos; the main text stays sharp and contrasting (A8). Small "magazine" columns — only with real brand text and per A6, no placeholder text for decoration.
- We stylise an era, not a specific ad: others' logos, slogans and recognisable campaigns (Apple, Sony, etc.) aren't copied.
- Photos and portraits — from the client or a stylisation of their shoot (flash, warm grading, grain); the product isn't generated (A9). A reference that fits no sub-style is a candidate for a new sub-style, not a reason to mix.

**Photo (for all sub-styles)**
- Real people with emotion and movement, flash, unusual angles (from below, from above, fisheye), food large in hand. The product cut out or in a real scene.
- Distortion and angle come from the photo itself; don't deform faces and the product in the layout.

**Layouts:** L28, L29, L30, L31, L32, L33, L34, L4, L1, L3, L11, L12, L17, L18. Don't use L7 (magazine spread), L19.

**L28. Fisheye + arc.** A full-frame photo of a person with a strong wide angle; the main word (up to 3 words) large, in an arc or tilted, following the frame's curve and not covering the face; a short lead-in on top and a punchline at the bottom in straight lines. A series — the same scheme, different scenes.

**L29. Photo + text plates.** A full-frame photo of a person; the phrase split into 2–5 pieces, each on its own colour plate, placed in steps over free areas; reads strictly top to bottom and left to right (A2), breaks by meaning, not after a preposition (A4).

**L30. Scrapbook.** The main photo (product in hand, street) + 1–3 photo cards in thick colour frames tilted up to 5°; the headline on a plate, details as small labels with an arrow to the right spot (no more than 3). Faces and the product aren't covered.

**L33. Y2K print ad.** Everything centred: a short serif headline (1–3 words) on top or above the tagline; in the centre — the hero product at 50–60% of the height (at surreal scale, as a fan of colour versions or on a clean background); at the bottom — a one-line tagline and the logo. Lots of air, no plates.

**L34. Outfit breakdown.** A full-length cut-out person in the centre on a calm background (an oval is OK); 3–6 circle callouts with details (the item large, a letter or number), thin lines to the right spot; at the bottom or side — a legend with names. For fashion, accessories, "what's in my bag" sets. The face is clear (A12).

**L31. Orbit.** The headline centred on a clean background; around it, as a ring or free orbit, 6–12 small 3D objects (products, categories, symbols from the text) in one palette and one light; a free field for text inside the ring. For "all in one", assortment, marketplaces.

**L32. 3D hero composition.** One sculpture of 3–7 objects (a stack, a floating group, the product with invented shapes around it) at 50–65% of the height; the headline large above or below, not crossing the composition. Variant: an inflated 3D word (1–2 words) becomes the hero itself, the caption in a normal font below.

**Changes in layer B:** bold headlines, caps up to 4 words, up to 2 bright accents, centred alignment is OK, tilt and curve of a headline up to 5 words, block tilt up to 5°.
**Check:** in Bold the viewer test (375 px) is especially important: if the main thing isn't clear in 2 seconds — remove one layer of decoration.

### Minimal
Board for refinement (optional): `preset-minimal`. This also covers premium and luxury.
- **For whom:** designer clothing and accessories, jewellery, watches, premium cosmetics, hotels, studios, architecture and interiors, galleries, cultural projects, archives and lookbooks.
- **Character:** quiet, structured, expensive; air is the main material. **The essence of the preset isn't in the text but in how the photos are shown:** their size, cropping and position on the grid. Playing with the image — yes, but never "put it there because it's pretty".

**The grid — the preset's main rule**
- **Grid first, then photos.** For each post (or series) set the grid explicitly: the number of columns (6 or 12 at 1080 px), gutter (16–24 px), margins, horizontal lines (top third, centre, bottom text line). Write it in CSS as variables (`--cols`, `--gutter`, `--col` = column width) and place everything through it (`grid-column: 3 / 6`), not by eye in pixels.
- **Every edge of a photo and text sits on a grid line.** Photo width is a whole number of columns. Captions are aligned to the left edge of their photo. If an element can't be explained by the grid ("sits on columns 2–4, top on the third line"), it's placed wrong.
- **Scale contrast.** Very different sizes sit next to each other: a large photo over 4–6 columns and small ones over 1–2. Identical medium photos in a row — boring, avoid.
- **Emptiness is part of the grid.** At least 50% of the artboard is free. Empty cells are left on purpose and not filled with decoration.
- **Cropping as a device:** a detail (a hand, fabric, part of a face), a narrow vertical strip, a photo running off the artboard edge (the crop also on a grid line or full bleed). A face may be cropped, but text doesn't cover it (A12).
- **A series — one grid.** In a carousel the grid, margins and caption position are the same on all slides; only the photo arrangement inside changes.

**Typography**
- Text is presented simply and calmly: a neutral grotesque 400 (or a serif / very thin grotesque for premium). The headline is small or medium; the photo makes the accent, not the font.
- Sometimes — one large calm paragraph (48–64 px, 400) at the top and photos below: text as a manifesto.
- Service captions under photos: a number ("01", "[ No. 01 ]"), date, name, material; mono is OK. These are navigation and captions per A6 — only with real content, not decoration. At least 24 px.
- Text near the artboard edge is anchored to the corners and margins of the grid (top left / bottom right, etc.).

**Colour:** by the brand (see "Colour in presets"). In references: white, off-white, grey, black; sometimes one colour field across the artboard (red, sage) with a small photo inside. The colours of photos in one post are matched (one tonality or b/w).

**Photo:** clean, calm, often b/w or muted; an object on an empty background, details, portraits, a full-frame landscape. No radii, shadows, frames or tilts.

**Graphics:** almost none — a thin 1 px line, a number, a small brand mark. No plates, icons, gradients.

**Layouts:** L35, L36, L37, L11, L1, L8, L5, L7, L3. Don't use L15, L17, L18, L28–L34 (a promotion — the "quiet sale" from the Promo card).

**L35. Modular photo layout.** 2–5 photos of different scale on a 6- or 12-column grid: one large (4–6 columns), the rest small (1–2 columns), all edges on lines; a number caption under each; free cells between them. The headline (if any) — small, in the top-left module.

**L36. Index / list.** 3–5 rows of one structure: in the left column — a tag (number, date, section), in the middle — a small photo, on the right — 1–3 lines of text; equal spacing between rows, lots of air. For collections, archives, services, projects.

**L37. Photo in a field.** One photo (or two, stacked / side by side with different crops) takes 20–45% of the area on a plain field (white or the brand colour), placed on the grid — centred or offset by a column; text small next to the photo or in the corners. Variant: a full-frame photo, text small in the corners on the margins.

**Changes in layer B:** the headline may be 40–80 px (contrast with text ×1.5–×2 instead of ×2.5); body may be 24–28 px; centred alignment is OK if the centre is a grid line; a serif for premium.
**Check (an addition to the "Form" role):** overlay the grid on the render and check that every edge of a photo and text lies on a line (2 px tolerance) and ≥ 50% is free. An element placed "by eye" is a blocker.

### Cute / Playful
Board for refinement (optional): `preset-cute`.
- **For whom:** kids' goods and toys, cafés and desserts, young cosmetics, concept stores and markets, cultural events, creative studios, hobbies, workshops.
- **Character:** cute and playful, but tasteful — "designerly", not kindergarten. Handmade and human (doodles, kids' drawings, stickers) on a neat, airy base. Play is in the details; grid and margins are kept.

**Typography**
- A soft grotesque or a retro serif with character; the accent word in italics or handwritten (one or two words). A rounded grotesque 600–700 — for kids' and very soft brands.
- **Text as play:** a short phrase in a circle (like a stamp sign, letters in circles), a word on a wave or along a rainbow, letters laid out like objects in a scene (on fruit, on the ground), words of different sizes. Only for 1–5 words; the main message and body are straight. In a circle — something that reads as a sign (name, slogan), not information.
- An editorial series: a large word in one corner, small caps text, a photo, a second word in the opposite corner ("marketing … emotional") — the same scheme for the whole carousel.

**Graphics**
- Hand-drawn: doodles, crayon flowers, brush ribbons, kids' drawings, rainbow lines, stars.
- Dots and circles: colour confetti over a photo, a grid of colour circles, photos in round cut-outs scattered over the field.
- Stickers and scrapbook: cut-out photos with a white outline, polaroids, pins, star badges; friendly brand characters (only from its Design System or by agreement).
- No more than two kinds of decoration per post (e.g. doodles + dots). One drawing style (line weight, crayon or brush texture) for the whole series. Simple shapes (dots, stars, waves, rainbows) you draw yourself; complex drawings and characters — from the brand or as a "what to draw" list.

**Colour:** by the brand (see "Colour in presets"). In references: a pastel background (pink, lilac, yellow, off-white) + one contrasting text colour (red, terracotta, green); dark text is a deep colour, not pure black.

**Photo:** lively playful moments (kids playing, a jump, laughter), film warmth, objects and toys large, hands. The face is clear (A12): doodles, dots and stickers around the figure or on the background, not on the face (exception — an intentional art device on request).

**Layouts:** L38, L39, L40, L1, L3, L4, L6, L11, L12, L15, L18, L31. Don't use L7, L19.

**L38. Finds catalogue.** Headline on top ("August finds"); 5–9 cut-out objects of different sizes on a clean background, with small numbers (1), (2)…; a legend with names small at the side or bottom. Objects don't overlap; air between them. For round-ups, assortment, markets.

**L39. A word in a circle / on a wave.** Up to 3 words run along a ring (letters in circles or text on a circle) around a photo, an object or an empty centre with the date and information; or a word runs along a wave/rainbow following the movement in the photo. Information (date, place, terms) — in straight lines. Works well as a series: the ring is a constant mark, the content inside changes.

**L40. Photo + drawing.** A photo (person, child, object) at 50–100% of the frame; over and around it — drawn doodles, flowers, a rainbow, stars or dots continuing the movement in the frame (a rainbow trailing from a skateboard); headline and text in a free zone, the accent word may follow the drawing. The drawing doesn't cover the face or the product.

**Changes in layer B:** up to 2 accents; centring is OK; an italic / handwritten word in the headline; text in a circle or on a wave up to 5 words; lowercase headline if that's the brand's way.
**Attention:** playful ≠ chaotic. Decoration doesn't cover text, product or faces and doesn't break A2; no less air than in layer B.

### Street / Fashion
Board for refinement (optional): `preset-street`.
- **For whom:** fashion, footwear, streetwear, vintage and resale, showrooms and pop-ups, youth brands, music, galleries and creative studios.
- **Character:** a fashion editorial from the street. Lively, slightly raw, "handmade" (photocopy, a scrawl, a tag, a scanner), but with the clear structure of a lookbook. Intentional imperfection is in the texture and photos, not in readability.

**Typography**
- A contrast of two voices: one large (a huge date or word across the full width, a bold condensed grotesque or a neutral white grotesque over a photo) and small service captions in the corners (mono, typewriter, drop numbers, sizes, dates).
- A handwritten scrawl (an ink signature, a hand-written name) — as a separate layer over a photo or paper; it's decoration and doesn't duplicate information, the main text is typeset.
- Diagonal text, a word cut by a photo, text running off the edge — only a decorative duplicate or 1–3 words; the body text is fully within the margins.

**Photo**
- City and documentary: the street from above, passers-by, city textures.
- Lookbook: a full-length person on a clean background, unusual poses; items cut out and laid out around.
- A flash flat lay on asphalt or floor (drop, vintage), strictly top-down.
- Photocopy / scanner: a b/w photocopy of an item, an object on the scanner glass with a glow; objects on paper (scissors, tags, patterns).
- Flash, film, grain, real people. The face is clear (A12): scrawls and stickers go over clothing and background, not over the eyes.

**Graphics**
- Technical look markup: thin (often red) frames around items, lines to thumbnails and captions (like L34, but drier and more precise).
- Tags, labels, tape, tracing paper over a photo, printed posters in a collage, hand-drawn background lines.
- Interface bits of a lookbook website (small menu captions in the corners) — only with real content per A6.
- Per post — one "handmade" device (a scrawl, or tape, or photocopy) and one "technical" one (markup, captions in the corners).

**Colour:** by the brand (see "Colour in presets"). In references: the colours of the photos themselves, grey and off-white paper, b/w photocopy + one accent (red markup, blue ink, an acid plate).

**Layouts:** L41, L42, L43, L18 (collage), L34, L36, L1, L4, L5, L15.

**L41. Drop flat lay.** Items of one look or drop laid out on asphalt/floor and shot from above with flash, full frame; a small caption in the corner (drop number, sizes, price on request). In a carousel — the overall shot first, then details larger.

**L42. Casting grid.** An even grid of 12–30 identically cropped faces or looks; one is larger over the grid or in place of several cells; the brand and collection caption small at the bottom. Only from the client's real photos.

**L43. A big date over the city.** A full-frame documentary photo; a date or 1–2 words across the full width of the margins in a white grotesque (top, centre or bottom — where there's a calm area and no faces); place, time and brand as small captions in the corners. For pop-up, drop and party announcements.
- **L18. Collage.** 2–4 photos or cut-outs of different sizes partially overlap (but not faces, A12); the headline is a separate clean block over a calm area; the reading order per A2 is kept.
- **Changes in layer B:** caps, bold headlines, block tilt up to 5°.
- **Attention:** "chaos" is only in the graphics. Layer A is checked just as strictly.

### Lifestyle / Home
Board for refinement (optional): `preset-home`. Restaurants and food presentation are a separate Food layer.
- **For whom:** home and living goods — interiors, furniture, lighting, finishing materials, kitchen and home appliances, cookware, textiles, home care, packaged food and drinks for the home, brand recipes.
- **Character:** warm, homely, about the usage scenario: the product in life, not in a shop window. References show two registers: dark interior (wood, deep tones, spot lighting) and light kitchen (beige, morning, window) — choose by the brand.
- **Typography:** a soft grotesque or a serif with character; handwriting — only as an accent of one or two words.
- **Colour:** by the brand (see "Colour in presets"); in references — warm homely: cream, terracotta, olive.
- **Photo:** the product in an interior and in hands, the moment of use, warm natural light, home details; the product is readable and in focus.
- **Graphics:** minimal; steps and scenarios — by numbers. Item captions — small text next to the item: name and size ("soup bowl, 7″"), material and colour as pill tags ("recycled paper", "beige"). The logo and a "save" icon — small, in the same corners across the series.
- **Devices from references:** renovation before/after — the frame split diagonally, both shots from the same point; a catalogue shot — the product centred on a light field, the name below; the product on a materials mood board (stone, wood, fabric samples as tiles).
- **Layouts:** L44, L45, L46, L1, L11, L13, L15 (steps), L7, L9, L21.
- **L44. A series of one space.** A carousel about one interior or material: overall shot → 3–6 details (edge, light, texture) → a mood board of samples → contacts. One light, tone and treatment for the whole series, almost no text needed.
- **L45. Features as hints.** Cover — "Checklist …" and the product in an interior; then one feature per slide: a check icon and 2–4 words top left, next to the relevant detail a translucent (frosted glass) explanation card; the kitchen background blurred, the product sharp and from one angle.
- **L46. Quiet still life with a hand.** The product takes 20–35% of the frame in a live scene (table, shelf, window), a hand enters the frame — pouring, taking, switching on; hard window light with shadows; text small in a corner or a caption under the photo.
- **Changes in layer B:** nothing.

### Food — a layer for food and restaurants
Board for refinement (optional): `preset-food`.
- **For whom:** restaurants, cafés, coffee shops, bars, street food, delivery, patisseries.
- **Important: Food isn't a standalone style but a layer.** It always comes paired with a second preset: restaurants are too different (a lively Italian trattoria and a minimalist Japanese place). Record: "Preset: Food + Minimal". The second half isn't set — choose by the brand's signals or ask; in doubt show the cover in 2–3 variants.

**Who does what**
- **The second preset — the approach:** the venue's character, composition, grid, typography, energy, amount of decoration.
- **Food — objects and elements:** how food is served and shot, the hero dish, menu and prices, the kitchen process, hands, interior, packaging. **Elements always come from Food.** If the second preset has a device with an object (a tag, a lookbook, a sticker), translate it into the language of food rather than carrying it over as is.
- One additional preset can be added per "Combining presets" — only 2–3 named devices are taken from it. Example: "Preset: Food + Street. Additionally: Bold — large bold type, plates, humour".

**Typical combinations**

| Venue | Preset |
|---|---|
| Burger joint, street food, hot dogs | Food + Street, additionally Bold |
| Fast food, delivery | Food + Bold |
| Italian trattoria, family restaurant | Food + Lifestyle |
| Japanese, omakase, fine dining | Food + Minimal |
| A coffee shop with its own crowd | Food + Street |
| Desserts, patisserie | Food + Cute |
| Wine and gastro bar | Food + Editorial |
| Healthy eating, bowls with ingredients | Food + Health |

**Translating elements into the language of food**

| Preset | Original | In Food |
|---|---|---|
| Street | tags, labels, drop flat lay | receipts, order stickers, kraft bags, wrappers, a flat lay of a set on the table |
| Street | look markup with frames | dish markup: ingredients, sauce, weight |
| Minimal | index, number captions under photos | dish numbers in the menu, name and price small |
| Bold | cut-out product, plates | cut-out food, price and promo plates |
| Cute | stickers, doodles | stickers on boxes, drawings on napkins, dessert stickers |
| Lifestyle | the product in home life | a dish on the table, hands, a shared table |
| Health | annotated composition diagram | a bowl's ingredients, macros as callouts |

No analogue in the table or Food references — invent a translation and name it in the summary.

**Devices from Food references**
- **Identity on the venue's objects:** the logo on plates (a stack from above), matches, glasses, a chef's jacket, business cards, boxes — the object as the hero of the post; a menu or card on the table next to the dish.
- **Receipt and kitchen ticket:** the pillar's text "printed" on a receipt, a receipt in the printer, a scan of thermal paper with monospaced text — the main translation of the "tag" for Food.
- **Mascot and icons:** a simple drawn mark of the venue (a fish, a star) and a row of ingredient icons joined by arrows ("oyster → olive → sun"); an icon can "fly" into a kitchen photo.
- **Manifesto over the staff:** a b/w photo of a chef or waiter, large narrow all-caps words about the venue.
- **Humour after the meal:** an empty plate captioned something like "the best review"; the venue's posters on a wall as a photo mock-up.
- **L47. Menu carousel.** Slides alternate: a text slide (a menu section — "To start", "Mains", a list of dishes with short descriptions and a small photo in the corner) and a full-frame top-down photo of a dish. Texts and prices — only from the client's menu.

**Food in frame (for any pair)**
- The dish is the hero: large, in focus, appetising; text and decoration don't crawl onto the food.
- Angle by the dish: flat — from above, tall (burger, cake, drink) — from the side or at 45°.
- The venue's real dishes aren't generated (A9): photos from the client, otherwise a placeholder and a shoot brief.
- Prices, ingredients, weight, allergens — only from the client's menu, not invented.
- Alcohol advertising is restricted in many markets — check with the client before posts with drinks.

**Layouts:** taken from the second preset (+ L17 for promotions via Promo, L38 for menu round-ups).

### Promo / Sale — a layer for promotions
Board for refinement (optional): `preset-promo`.
- **For whom:** promotions, discounts, sales, launches with a price, giveaways, promo codes, seasonal sales — for any brand.
- **Character:** clear and fast: what, how much, until when.
- **Promo is a layer, like Food.** Record: "Preset: Minimal + Promo" or by pillar: "Pillar 'Promotions' → + Promo". **The main styling comes from the first preset** (fonts, grid, photo, amount of decoration, brand colour). **From Promo — the promotion's hierarchy and promo elements** (price, percentage, old price, deadline badge, promo code, timer), but drawn in the first preset's language. Stylistic promo devices from Promo references can also be taken (as an additional device per the combining rule) if they don't break the first preset.

**What a promotion looks like in different presets**

| First preset | Promo elements |
|---|---|
| Minimal | no plates: the price or "−30%" small on a grid line, the old price with a thin strikethrough, dates as a caption in the corner; a large number in a thin font is OK |
| Corporate / Fintech | a neat terms card (rate, cashback, term), the number large, a deadline chip; legal terms are mandatory |
| Bold | burst badges, a huge percentage, plates, humour in the promo text |
| Cute | the price on a sticker or in a drawn circle, the deadline as a word in a circle |
| Street | a price tag, a receipt, a price in marker, the drop number and "only until…" in the corners |
| Editorial / Lifestyle | a soft approach: the benefit in a two-tone headline, the price calmly next to the product, no bursts |
| Health | the benefit as a card with a large number in the slide's tone, a mono deadline tag |
| Food | the price next to the dish, combo/set, a receipt or menu line — per the pair's second preset |

The main thing: the promotion must be recognisably "this brand". A Minimal brand with red bursts is a mistake, even if that's what Promo references look like.
- **Attention:** price, old price, percentage, deadline, promo code, stock left, giveaway terms — only from the client. No data — a placeholder "[price]", "[until what date]" and a question in the summary. The old price and a timer — only if the client confirmed they're real. Giveaways: rules and deadline from the client, legal text per A6.
- **Reading order (A2):** benefit (price or discount) → product → condition → deadline → CTA.
- **Typography:** the price or percentage is the main, largest element; the old price is struck through, smaller, quieter.
- **Colour:** the brand's base preset + 1 promo accent (from the brand book, if any).
- **Photo:** the product cut out or on a clean background, large, without extra surroundings.
- **Graphics:** a discount plate, a deadline badge; no more than two plates per layout.
- **Layouts:** L17 (price hero), L48, L49, L50, L11, L12, L15 (product round-up).
- **Devices from references** (taken only if they fit the first preset):
  - **Quiet sale:** a tone-on-tone background, the percentage in a thin serif or grotesque of the same colour slightly darker, captions small — for Minimal, Editorial, premium.
  - **A small percentage on a portrait:** a full-frame fashion photo, the discount and deadline as a small block in the corner; for Street, Editorial.
  - **A brush-lettered percentage** across the frame on a light field — for Editorial, Cute.
  - **The word "SALE" as a pattern** over a product photo, repeated at different sizes; promo letters in sticker circles; a stack of sticker flyers with the percentage — for Bold, Cute.
  - **A carrier object:** a price tag, a label, a keychain with tags — the promo words on it; for Street, Bold, Lifestyle.
  - **Word captions over a photo:** a short phrase split into words in small plates scattered over the frame — for Street, Bold.
  - **Teaser hint:** a mystery frame before the promotion (a silhouette, binoculars, "soon") — 1–2 days before the start.
- **L48. Teaser carousel.** The promo phrase split over 4–6 slides of 2–4 words in a huge font ("Guess what" → "No, really" → "For the" → "First time" → "Sale" → "−25%"); at the slide edge — a narrow photo strip running from slide to slide; on the last — terms and deadline; handwritten notes are OK.
- **L49. Panorama promo.** The promo word ("Winter Sale") in a huge font across 2–4 carousel slides; under it the products as cut-outs in a row, each fully within its own slide; terms small in the corners of the first and last.
- **L50. Letters and photos in a grid.** A 3×3 grid: the letters of the promo word alternate with photos of products or a model, the central cell holds the terms ("up to −50%, online and in stores").
- **L17. Price hero.** The price or discount takes 25–40% of the height; the product beside or below it; the condition and deadline in one line; a CTA at the bottom on the margin. The promotion's legal terms — per A6.
- **Changes in layer B:** bold prices and percentages; a CTA on a promo slide — per the A6 exception.
- **Combining:** the visual language (fonts, colour, photo) stays with the brand's base preset; Promo adds hierarchy and promo elements in the form the base preset allows (in Minimal — no plates).

---
Author: Sanira Baitasova. Part of the by skills collection.
