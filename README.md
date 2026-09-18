# LWG — Meadow Harvest

**Little Walks With God™ — Harvest Meadow Collection**
Picture-book project: **"The Golden Leaf of Harvest Meadow"** — Amara (~5) & Micah (~3).

## Folder structure

```
assets/                  Reference art (attached to every generation)
  amara/                 Amara sheets: front, closeup, back, profiles, scripture print
  micah/                 Micah sheets: turnaround, closeups, full-body, scripture print
  mama/                  Mama turnaround, expression sheet, hero full-body
  papa/                  Papa turnaround, expression sheet, hero full-body
  family/                Full-family lineup / scale chart
  collection/            Collection title art
  canon/                 Setting/prop lock: house-porch, wagon, props
book/                    Generated book spreads (Units 1–15), TEXT MODE A (integrated text)
docs/                    Production docs: adapter, canon decisions
CATALOG.md               Full asset inventory + book-unit checklist
```

## How book images are made here

Every spread is generated with visual anchors (not words alone):

1. **References** from `assets/` — character faces/outfits + `assets/canon/` sheets
   (house = exactly 3 steps, wagon build, basket/Bible/blanket/jug).
2. **Prompts** from `docs/golden-leaf-chatgpt-adapter-15-units.md` + legacy character
   block in `docs/canon-decisions.md`.
3. **TEXT MODE A** — story text rendered in the illustration, then QA'd
   character-for-character; failures regenerate (max 2x) before fallback.

Locked look = **legacy**: sunflower bows + rust bandana on Amara; no scarf on Micah.
See `docs/canon-decisions.md`.

## Status

- [x] Assets organized, duplicates removed, cataloged
- [x] Canon kit: house, wagon, prop sheets
- [x] Canon locked: legacy look + integrated text
- [ ] Pilot spreads: Units 1–3 (1, 12 approved; 2, 3 next)
- [ ] Batch: Units 4–15
- [ ] Final QA + print layout
