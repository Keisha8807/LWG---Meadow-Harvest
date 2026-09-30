# Product Line: Matching Family

Locked 2026-09-30: 12-page coloring book (with titles) + 6-print wall art set.
Both derive from approved storybook art, so faces/outfits/style stay in the family.

## Coloring book — `coloring-book/` (portrait 8.5×11)

Spec: pure black line art on white. No shading, grayscale, watercolor, or
cross-hatching. Bold closed shapes for ages 3–7. Short bubble-letter title per page.
Each page converts its source spread's composition (spread attached as reference).

| File | Title | Source | Status |
|---|---|---|---|
| `cover-coloring-book.png` | Harvest Meadow Coloring Book | new | ⬜ |
| `page-01-packing-the-wagon.png` | Packing the Wagon | Unit 1 | ⬜ |
| `page-02-our-first-treasure.png` | Our First Treasure | Unit 2 | ✅ approved (was style sample) |
| `page-03-acorns-for-the-squirrel.png` | Acorns for the Squirrel | Unit 3 | ⬜ needs approved U3 first |
| `page-04-feather-for-the-bird.png` | A Feather for the Bird | Unit 5 | ⬜ needs approved U5 first |
| `page-05-flowers-for-the-bees.png` | Flowers for the Bees | Unit 6 | ⬜ |
| `page-06-care-for-the-lamb.png` | Care for the Lamb | Unit 8 | ⬜ |
| `page-07-resting-under-the-oak.png` | Resting Under the Oak | Unit 9 | ⬜ needs U9 first |
| `page-08-whoosh.png` | Whoosh! | Unit 11 | ⬜ needs approved U11 first |
| `page-09-bridge-for-the-ants.png` | A Bridge for the Ants | Unit 12 | ⬜ |
| `page-10-five-blessings-shared.png` | Five Blessings Shared | Unit 13 | ⬜ needs U13 first |
| `page-11-coming-home.png` | Coming Home | Unit 14 | ⬜ needs U14 first |
| `page-12-hearts-were-full.png` | Hearts Were Full | Unit 15 | ⬜ |

Dropped as quiet/transitional: Units 4, 7, 10.

## Wall art — `wall-art/` (portrait 8×10) + 2 existing prints

Spec: same watercolor-on-cream nursery style as the existing scripture prints.
Verse text verbatim + heart + citation, upper-right open space.

| # | File | Subject | Status |
|---|---|---|---|
| 1 | `wall-art/print-01-amara.png` | Amara, pumpkin basket portrait | ⬜ |
| 2 | `wall-art/print-02-micah.png` | Micah, pumpkin basket portrait | ⬜ |
| 3 | `wall-art/print-03-siblings-meadow.png` | Amara & Micah, meadow, no verse | ⬜ |
| 4 | `assets/amara/amara-scripture-james-1-17.png` | James 1:17 (existing) | ✅ exists |
| 5 | `assets/micah/micah-scripture-philippians-4-13.png` | Philippians 4:13 (existing) | ✅ exists |
| 6 | `wall-art/print-06-psalm-107-1.png` | Psalm 107:1 thankfulness verse | ✅ approved (was style sample) |

Prints 4–5 are referenced in place (no duplicated binaries).

## Sequence & budget

1. Main book Batch 2: regens (3, 4, 5, 7, 11) + new (9, 13, 14) — 8 gens
2. Coloring book: cover + 11 pages — 12 gens (2 turns)
3. Wall art: prints 01–03 — 3 gens
