# Print Prep — KDP + Etsy Spec Sheet
*Gathering Meadow Treasures product line · measured 2026-10-02 · all art AI-generated PNG (no PIL metadata, sRGB assumed)*

## 0. Measured inventory (actual pixels)

| Product | Files | Pixels (W×H) | Ratio | Native print size @300 DPI |
|---|---|---|---|---|
| Storybook spreads U1–U14 | `book/unit-01…14` | 1456 × 720 | 2.02:1 | 4.9″ × 2.4″ ❌ too small for print |
| Storybook finale U15 | `book/unit-15-page-32` | 1024 × 1024 | 1:1 | 3.4″ × 3.4″ ❌ |
| Coloring cover + p01–p12 | `coloring-book/*` (13) | 912 × 1168 | 0.78:1 | 3.0″ × 3.9″ ❌ |
| Wall art 01, 02, 03, 06 | `wall-art/print-*` | 928 × 1152 | 0.806:1 (≈4:5) | 3.1″ × 3.8″ ❌ |
| Wall art 04, 05 (scripture) | `assets/*/amara-scripture…`, `micah-scripture…` | 1122 × 1402 | 0.80:1 (≈4:5) | 3.7″ × 4.7″ ❌ |

**Bottom line for all three products: the art is WEB resolution. Every piece needs AI upscaling before print.**
Do NOT use basic resize — use an AI upscaler (Topaz Gigapixel, Magnific, Photoshop Super Resolution, or equivalent), then downsample to the exact targets below.

Key rules from Amazon: KDP requires every interior image ≥ **300 DPI effective** (pixels ÷ printed inches — metadata alone means nothing) ([1](https://publishing.co.uk/guides/kdp-error-low-image-dpi/), [2](https://cambric.pub/guides/kdp-image-resolution-too-low/)); full-bleed interiors must extend art **0.125″ past trim** on top/bottom/outer edges (no bleed at spine) ([3](https://kdp.amazon.com/en_US/help/topic/G201857950)); minimum page count is **24 pages** ([3](https://kdp.amazon.com/en_US/help/topic/G201857950)); covers need 0.125″ bleed all sides + 300 DPI ([4](https://kdp.amazon.com/en_US/help/topic/G201953020)).

---

## 1. 📖 Storybook → KDP paperback

**Recommended trim: 8.5″ × 8.5″ square** — the most popular KDP children's size ([5](https://kidillus.com/learn/book-trim-sizes-bleed-margins)) and the best ratio match: a full-bleed spread at this trim is 17.125″ × 8.75″ (ratio 1.96:1) vs our art at 2.02:1 — only a ~3% side crop.

| Item | Target size (full-bleed PDF) | Pixels @300 DPI | Prep from source |
|---|---|---|---|
| Spreads U1–U14 | 17.125″ × 8.75″ | **5138 × 2625** | 4× upscale → 5824×2880 → crop/downscale |
| Finale U15 (single page) | 8.625″ × 8.75″ | **2588 × 2625** | 3× upscale → 3072² → downscale |
| Interior PDF | 32 pages, one PDF, fonts embedded (n/a — art only) | — | pp 1–3 front matter + pp 4–32 art |
| Cover | Via [KDP Cover Calculator](https://kdp.amazon.com/en_US/help/topic/G201953020) (32 pp, color ink) | 300 DPI, 0.125″ bleed | New layout: title art + spine + back copy |

**Safe areas (24–150 pp, with bleed):** keep all baked-in text ≥ **0.375″ from outer trim edges** and ≥ **0.375″ from gutter** ([3](https://kdp.amazon.com/en_US/help/topic/G201857950)). ⚠️ After the upscale+crop, QA every spread: our integrated text sits close to edges in some units and the 3% side crop + trim could nick letters. Fix by nudging crop, not by re-typing (verbatim lock stands).

**Still to create:** pp 1–3 front matter (half-title, copyright, dedication), full-wrap cover (front/spine/back + ISBN barcode — KDP's free ISBN is fine), back-cover blurb.

---

## 2. 🖍️ Coloring book → KDP paperback + Etsy printable

**Recommended trim: 8.5″ × 11″** (standard coloring/activity size). Our art ratio 0.781 vs page 0.773 — near-perfect fit.

| Item | Target size (full-bleed PDF) | Pixels | Prep from source |
|---|---|---|---|
| Each page (cover + p01–p12) | 8.625″ × 11.25″ | **2588 × 3375** @300 | **4× upscale** → 3648×4672 (≈420 DPI — crisp lines; 300 is the KDP minimum, line art looks better higher ([2](https://cambric.pub/guides/kdp-image-resolution-too-low/))) |
| Interior PDF | **24 pages**: 12 designs single-sided + blank backs (standard — prevents marker bleed-through; also satisfies the 24-page minimum) | B&W ink setting (cheaper print + correct category) | Export flattened PDF, no compression artifacts on lines |
| Cover | KDP cover calculator (24 pp, B&W ink) | 300 DPI + bleed | Upscale `cover-coloring-book.png` 4× for front |

**Etsy printable version:** same 13 pages as ONE flattened PDF (JPEG-quality print inside, < 20 MB — easily achievable) + optionally a ZIP of 13 individual 300-DPI JPEGs. One listing, 2 file slots used. See §4 for general Etsy rules.

---

## 3. 🖼️ Wall art → Etsy digital downloads

Etsy hard limits: **5 files per listing, 20 MB per file**; use JPEG (≈85–90 quality) not PNG; no variations for digital — buyers get ALL files, so bundle every size in ratio-organized ZIPs ([6](https://snaptosize.com/etsy-digital-download-file-size), [7](https://snaptosize.com/etsy-digital-download-size-variations)).

| Print | Master after upscale | Listable sizes @300 DPI |
|---|---|---|
| 01, 02, 03, 06 (928×1152) | 3× → **2784 × 3456** | up to 9×12″ / A4 / **11×14″** (264 DPI — acceptable) |
| 04, 05 scripture (1122×1402) | 3× → **3366 × 4206** | up to **11×14″** @300 ✓ |
| For 16×20″ offerings | 4–6× upscale required | Only list sizes your master truly supports @300 |

**Listing strategy (recommended):** 6 individual listings (one per print) + 1 bundle listing (all 6). Each individual listing: up to 5 ratio ZIPs — 4:5 (8×10, 12×15, 16×20¹), 3:4, 2:3, ISO A-series, Extras (5×7) ([7](https://snaptosize.com/etsy-digital-download-size-variations)). ¹Only include 16×20 if you did the 4×+ upscale. Center-crops are safe on these portraits (airy watercolor backgrounds) but QA each crop — never crop through faces, baskets, or verse text.

**Listing images:** mockups ≥ 2000 px on the short side (Etsy recommends 2700×2025) ([8](https://ratioready.com/guides/etsy-digital-downloads)) — *still to create (see Next steps).*

---

## 4. Checklists

### KDP upload (per book)
- [ ] All art AI-upscaled, final effective DPI ≥ 300 everywhere (verify: pixels ÷ trim inches)
- [ ] Interior PDF page size = trim + bleed (storybook spread 17.125×8.75″; coloring page 8.625×11.25″)
- [ ] No crop marks, comments, or metadata in PDFs ([3](https://kdp.amazon.com/en_US/help/topic/G201857950))
- [ ] Cover built from KDP's calculator numbers (spine width depends on page count + ink)
- [ ] KDP Previewer checked: no text in trim/gutter zones, no blank-page surprises
- [ ] Page count even and ≥ 24 (storybook 32 ✓ planned / coloring 24 ✓ planned)
- [ ] **Do NOT enroll in KDP Select** if selling the same book/PDF on Etsy (Select = Amazon-exclusive ebook)

### Etsy listings
- [ ] Every file < 20 MB, ≤ 5 files per listing ([6](https://snaptosize.com/etsy-digital-download-file-size))
- [ ] Print files are JPEG @300 DPI (not PNG — 3–5× too big)
- [ ] Keywords in first 40 characters of title; lifestyle mockups in photos
- [ ] Listing text states: digital download, no physical item, print sizes included, print-at-home or print-shop recommended

## 5. Next steps (in order)
1. **Upscale all art** (Topaz/Magnific/etc.): storybook 4×/3×, coloring 4×, wall art 3×+ → save masters (not in git — too big; keep local/Drive).
2. **Assemble PDFs** (Affinity Publisher / InDesign / Scribus-free): storybook 32-pp interior + wrap cover; coloring 24-pp interior + wrap cover.
3. **Create front matter + back-cover copy** (need your author name, ISBN choice, blurb).
4. **QA in KDP Previewer**, fix text/trim collisions.
5. **Etsy mockups** (framed prints on walls, book mockups) — I can generate these next if you want.
6. Publish: KDP paperbacks → Etsy digital listings → 🚀
