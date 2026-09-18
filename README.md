# LWG — Meadow Harvest

**Little Walks With God™ — Harvest Meadow Collection**
Picture-book project: **"The Golden Leaf of Harvest Meadow"** — Amara (~5) & Micah (~3).

## Folder structure

```
assets/                  Character reference & collection art (canon look)
  amara/                 Amara sheets: front, closeup, back, profiles, scripture print
  micah/                 Micah sheets: turnaround, closeups, full-body, scripture print
  mama/                  Mama turnaround, expression sheet, hero full-body
  papa/                  Papa turnaround, expression sheet, hero full-body
  family/                Full-family lineup / scale chart
  collection/            Collection title art
book/                    Generated book spreads (Units 1–15) — TEXT MODE B (no text)
docs/                    Production docs (adapter sheet with all 15 prompts + full text)
CATALOG.md               Full asset inventory + book-unit checklist
```

## How book images are made here

Yes — we generate them in this repo with the image tool, using:

1. **References** from `assets/` (faces, skin tones, watercolor style).
2. **Prompts** from `docs/golden-leaf-chatgpt-adapter-15-units.md` (scene, continuity, exclusions).
3. **TEXT MODE B** — illustrations are generated *without* text (avoids paraphrase/garbled-letter
   risk); the exact manuscript text is typeset separately in layout.

Art direction follows the adapter canon: small muted-rust bows low near Amara's ears
(no sunflower bows), no bandana/neckerchief/scarf, no jewelry. Legacy reference art in
`assets/` still shows the older accessories — it is kept for face/style consistency only.

## Status

- [x] Assets organized, duplicates removed, cataloged
- [x] Sample spreads: Unit 1, Unit 12
- [ ] Remaining spreads: Units 2–11, 13–15
- [ ] Layout with typeset text (preview + print)
