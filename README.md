# by-design — SMM design skills for Claude

Created by **Sanira Baitassova**.

| Skill | What it does |
|---|---|
| `by-composition` | The foundation for any social visual in Claude Design: formats and grid, reading order, typography, photo, product, number visualisation, 15 base layouts, multi-level checks, delivery, and learning each brand's style over time ("Style from practice"). |
| `by-presets` | 10 style presets (Neutral, Editorial, Corporate, Fintech, Health, Bold, Minimal, Playful, Street, Lifestyle) and 7 layers (Food, Promo, Beauty, Auto, Real Estate, Holidays, Cultural code) with 55 more layouts; how to choose and combine them. |
| `by-motion` | Animated Stories and graphic Reels: storyboard, timing, motion by preset, a library of 20 techniques, music and beat, checks. |
| `design-setup` | A guided first-run chat: market, languages, publishing method, your Pinterest preset boards, Instagram references, your first brand. |

Built for any market — holiday calendars and number/date/unit formats adapt to the market you set (US, UK/Europe, Japan, South Korea, China, Southeast Asia, Kazakhstan/CIS and others), including Japanese, Korean and Chinese typesetting. Ad-disclosure rules are built in for the US, UK, Japan and South Korea; for other markets Claude asks for the local requirement. Skills are written in English; Claude answers in the language you write in.

Looking for trend research and content ideas? See **[by-content](https://github.com/bysaneera/by-content)**.

---

## Install

### Option 1 — by link (recommended)
**Claude app (desktop / web):** Customize → **Plugins** → **Add marketplace** → paste
```
https://github.com/bysaneera/by-design
```
then install **by-design**. Plugins work where Claude runs tasks with tools (the desktop app's task mode and Claude Code), not in a plain chat.

**Claude Code:**
```
/plugin marketplace add bysaneera/by-design
/plugin install by-design@by-design
```

**Organisations:** organisation-wide sync from GitHub works only with private or internal repositories connected through the Claude GitHub App — an admin can fork this repo privately and sync that, or upload the file below.

### Option 2 — upload the file
Download [`dist/by-design.zip`](dist/by-design.zip) (or the identical [`dist/by-design.plugin`](dist/by-design.plugin)) and upload it in Claude: Customize → Plugins → upload a plugin file.

---

## First run — setup chat

After installing, start a task and write something like:

> Set up the design skills

Claude walks you through it step by step (every step is optional and can be changed later):
1. Market and languages, bilingual projects (primary / second language) — sets holiday calendars, number/date/unit formats and ad-disclosure defaults.
2. Publishing method (manual / auto-posting / ads) → default formats.
3. Pinterest boards for refining presets: `composition`, `preset-corporate`, `preset-tech`, `preset-health`, `preset-bold`, `preset-minimal`, `preset-cute`, `preset-street`, `preset-home`, `preset-beauty`, `preset-auto`, `preset-real-estate`, `preset-holidays`, `preset-cultural`, `preset-food`, `preset-promo`, `motion-design`.
4. Instagram accounts to use as references (read only).
5. Optionally your first brand's Design System.

Claude only **reads** your accounts — it never posts, pins, likes, follows or enters passwords (you log in yourself in your browser).

---

## How to use

- "Lay out this post: <text>" — format question → layout → check → PNG + alt text.
- "Make a carousel from this text", "Reels cover for …", "Story with a poll …"
- "Make it Bold / Scrapbook", "Preset: Food + Street"
- "Animate this as a 10-second Reel"
- "What worked last month?" (with Metricool connected)

---

## Requirements
- **Claude Design** for laying out visuals.
- A browser Claude can use (Claude in Chrome or the desktop app's built-in browser) for Pinterest and Instagram references.
- Optional: Metricool (stats, auto-posting).

## Privacy
No personal data, accounts or libraries ship with these skills. Every user's settings, libraries and brand memory live in their own Claude account.

## Author and licence
All skills in this repository were created by **Sanira Baitassova**. Licensed under [CC BY 4.0](LICENSE): you can use, share and adapt them, including commercially, as long as you credit the author.
