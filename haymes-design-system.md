# Haymes Paint — Design System
**For:** Claude Design  
**Source key:** [BG] HAYM101_Brand_Guidelines_v1 · [SG] 2022 style guide (gap-fill only) · [VI] visual inference

---

## 1. COLOUR

### Brand palette
```css
:root {
  --color-primary:     #021D49;  /* PMS 2768C · C100 M90 Y13 K61 · R2 G29 B73 — dominant, all material */
  --color-secondary-1: #0077C8;  /* PMS 3005C · C100 M35 Y0 K2 · R0 G119 B200 — supporting only */
  --color-secondary-2: #54585A;  /* PMS 425C · C63 M51 Y45 K33 · R84 G88 B90 — labels, captions */
  --color-accent:      #5BC4DF;  /* PMS 3265C · C60 M0 Y30 K0 · R91 G196 B191 — Paint Shop/e-commerce ONLY */
  --color-white:       #FFFFFF;
  --color-cream:       #E8E3D8;  /* Part A sidebar */
  --color-teal-bg:     #D4E8EA;  /* Part B sidebar */
}
```

### Colour rules
- Primary is dominant in every piece — secondary supports, never overpowers
- Accent restricted to Paint Shop contexts (e-commerce, recruitment) — never tinted, always 100%
- Tints (80/60/40%) of primary and secondaries: charts and diagrams only — never branding, swoosh, headings
- Logo on backgrounds: navy logo on white/light · white logo on dark/navy/dark photography · never white logo on light photography or light swatches

---

## 2. TYPOGRAPHY

### Font families
Brand fonts are Muller (sans) and Monarcha (serif). Mulish and Newsreader are the implementation fonts in Claude Design — Mulish stands in for Muller, Newsreader for Monarcha.
```css
:root {
  --font-brand:    'Mulish', 'Arial', sans-serif;             /* implementation of Muller — all communication */
  --font-campaign: 'Newsreader', 'Monarcha', 'Muller', serif; /* implementation of Monarcha — YBIB campaign headlines */
  --font-fallback: 'Arial', sans-serif;                       /* Microsoft Word / non-graphic desktop only */
}
```

### Weight-to-role mapping
| Role | Weight | Size |
|---|---|---|
| Large display headings (posters, marketing) | Muller Black or Bold | Display — no max |
| Section number on hero divider | Muller ExtraBold | ~52px |
| Section subtitle on hero divider | Monarcha Regular italic | ~52px |
| Sidebar section heading | Muller Bold | 14–15px |
| Subheadings | Muller Medium | Secondary headings only |
| Body copy | Muller Light or Regular | 8pt minimum |
| Sidebar body / small labels | Muller Light | 11–13px |
| Copyright, page numbers | Muller Light | 11px |
| Directions, diagrams | Muller Light | 6pt minimum |
| Campaign headline (YBIB context) | Monarcha Regular | Display scale |

**Warnings:** Black/Bold too heavy for body copy — headings only. Black/ExtraBold at large sizes requires manual kerning.

### Casing, tracking, spacing [SG]
- Default: sentence case
- Tracking: −5 to +5 only. Paragraph spacing: 1mm minimum after each paragraph

---

## 3. LAYOUT SYSTEM

**Page:** 1920×1080px landscape

**Padding — full page:** left 120px · top 90px · right 120px · bottom 40px


### Master rules — all templates
- **Text top left:** "Haymes Paint" / "Brand Guidelines" on two lines (line break before "Brand", no slash) · Mulish Regular, 14pt
- **Disclaimer:** Mulish Regular, 9pt

### Five page templates

| Template | Use for | Key feature |
|---|---|---|
| **Hero / section divider** | Opens every section | Full-bleed photo. Text top right: Newsreader Regular, 20pt. Title text: sits 270px from top, Mulish Bold, 64pt. Subtitle text: sits 400px from top, Newsreader Regular, 50pt |
| **Standard content — white panel** | Spec-heavy pages (logo, colour, type rules) | Sidebar 500px width cream/teal + white panel 1420px width |
| **Standard content — no panel** | Narrative/list pages (e.g. Sections 2–3) | Full-bleed cream/teal. Sidebar heading in same 500px left zone. Body in 1–4 columns: bold header + rule + body + closing rule. No colour-block charts, no large numerals, no rotated labels |
| **Rules / do-don't grid** | Misuse pages | 4-col white panel. 3× ✕ Incorrect + 1× ✓ Correct (last col). 0.5px primary colour dividers. Verify column order per page — not always last-correct |
| **Feature / message grid** | Parallel feature callouts | Sidebar + panel subdivided into equal image-led columns. No ✕/✓ labels |
| **Placeholder / gap page** | Unfinished sections | Sidebar normal. Panel: "Insert work" or "Copy to come" only — never fabricate content |
| **Executional 2-page spread** | Part B channel executions — used for each message pillar or channel sub-section | Page 1: Social + POS artwork. Page 2: Website + eDM artwork. Each page: left ~40% = 100-word Lorem ipsum blurb (placeholder — copy supplied by Spinach progressively). Right ~60% = artwork examples at appropriate format sizes. Teal sidebar. Each sub-section gets its own 2-page spread. |

**Sidebar colour:** Part A = `#E8E3D8` (Sections 1–13) · Part B = `#D4E8EA` (Sections 14–21)

**Sidebar elements (all templates):** Title: Mulish Bold, 32pt · Body: Mulish ExtraLight, 18pt

---

## 4. LOGO SYSTEM

### Primary logo [BG]
Script "Haymes" + "PAINT" (Muller Bold all-caps, centred beneath). Navy on light · white on dark. Use: corporate comms, brand/marketing material, packaging.

### Secondary logo [BG]
Primary logo + strapline "Australia's first family of paint." + "SINCE 1935" boxed badge (Muller Bold, all-caps, rule lines above and below). Use when baseplate is inappropriate: corporate, sponsorship, some marketing (e.g. t-shirts).

### Clearspace and minimum sizes [BG]
- Clearspace: descender height of Haymes script on all four sides
- Print: 20mm · Digital/video: 90px · Social favicon: 16×16px

### Logo misuse — never [BG]
Use script alone without "PAINT" · recreate or replace elements · add words · edit weight or stroke · distort/stretch/tilt/rotate · use multiple colours or effects · alter strapline configuration

---

## 5. BASEPLATE SYSTEM [SG]

Three variants: **Corner** (corporate, lifespan 1yr+) · **Corner campaign** (marketing, lifespan <1yr, includes award logo) · **Full bleed** (presentations, brochures, PowerPoint).

Elements (all variants): can render or logo · navy swoosh `#021D49` · strapline · AMAO logo · award logo (campaign only) · third-party logos (left side only).

Misuse: never use lifestyle photography instead of can renders · never edit/stretch/warp can render · never reconfigure, add, remove, or recolour elements · at recall situations: primary logo only, no award logos.

---

## 6. ICON SYSTEM [SG]

Artboard 50×50mm · clearspace 5mm · stroke 3pt · solid colour only, no gradients or effects · simple and minimal.  
Sizes: print 10mm · digital 28px.  
Set: Roller · Brush · Spray · Hawk & Trowel · Texture Pump · Re-coat 24hrs · Touch Dry 2hrs · Water Wash-up · Thinners/Acetone Wash-up.

---

## 7. GRAPHIC DEVICES

**Colour swatches [BG/SG]:** Square chip · colour name top-left · logo top-right · colour code bottom-left · used as social media graphic device.

**Colour blobs [BG/SG]:** Organic paint-drop shape showing light/shadow/reflection · online selectors, Instagram, moodboards, sample pot ordering.

**Black brushstroke [VI]:** Organic black shape for retail promotional callouts · white Muller Black text on top · animation: stroke → type → product → YBIB.

**Colour wall background [BG]:** Pre-built coloured walls in various Haymes colours · white skirting at base · can render in front · holds different product labels.

**AMAO logo [BG]:** Australian Made & Owned green triangle · placed beside can render at lug/handle height in all campaign material · always present, never absent.

**Canstar Blue badge [BG]:** "Most Satisfied Customers 2025" circular award · navy and teal with star ratings · campaign and announcement material alongside AMAO logo.

**TRADE ONLY OFFER badge [VI]:** Navy pill shape · "TRADE ONLY OFFER" white all-caps · never alter colour or type treatment.

---

## 8. SUB-BRAND SYSTEM [SG]

Sub-brand device always legible at small sizes · Haymes Paint logo visually equal to sub-brand mark · Haymes logo always single colour when used with sub-brand · never add to, edit, or replace the Haymes logo.  
Clearspace and minimum sizes: same rules as primary/secondary logo.

---

## 9. SPACING TOKENS [VI]
```css
:root {
  --space-xs:  4px;   /* tight internal gaps */
  --space-sm:  8px;   /* inline element spacing */
  --space-md:  16px;  /* component internal padding */
  --space-lg:  32px;  /* between content blocks */
  --space-xl:  48px;  /* between major sections */
  --space-2xl: 64px;  /* large block spacing */
  --space-3xl: 96px;  /* extra-large block spacing */
}
```

---

## 10. CAMPAIGN PLATFORM RULES [BG]

**YBIB lockup variants:** Inline ("You bet it's better." — single line) · Stacked ("You bet / it's better." — two lines).

**Size rule:** YBIB lockup always 25% larger cap height than the preceding Monarcha campaign headline. Never equal, never smaller.

**Approved signoff combinations:** Inline YBIB + logo · Inline YBIB + can + AMAO (at lug height) · Stacked YBIB + logo · Stacked YBIB + can + AMAO (at lug height).

**Colour on backgrounds:** Dark/navy wall or dark photography → white · Light wall → navy `#021D49`.

**Channel rules:** OOH/brand: stacked or inline per format · Retail social: inline centred in retail headline · Trade eDM: stacked left-aligned to headline and offer · Video end frame: stacked.

---

## 11. PHOTOGRAPHY DIRECTION [BG]

| Category | Direction |
|---|---|
| **People** | Candid environmental portraiture. Most comfortable/relaxed moment. Editorial, minimal direction. Genuine unguarded expression. Familiar surroundings — factory, store, on-site. |
| **Lifestyle interiors** | Colour-forward rooms. Paint is always the hero. Dark moody to bright/playful. Warm natural light. Lived-in, not over-styled. |
| **Lifestyle exteriors** | Capture the finish and intent. Painted surface, not architecture. Heritage and contemporary Australian homes. |
| **Paint still life** | Overhead or slight angle. Open cans, brushes, swatches, sample pots. Clean white/neutral surfaces. Brand-consistent brushes with Haymes branding visible. |
| **Trade** | Candid simple moments. Painters on-site — active or relaxed. Haymes branded navy apparel visible. Never studio-staged. |

---

## 12. CLAUDE DESIGN INSTRUCTION BLOCK

Paste this at the start of every Claude Design session:

```
BRAND: Haymes Paint Brand Guidelines 2026

COLOURS:
  Primary (dominant):  #021D49
  Secondary 1:         #0077C8
  Secondary 2:         #54585A
  Accent (Shop only):  #5BC4DF — never tinted
  Content bg:          #FFFFFF
  Part A sidebar:      #E8E3D8
  Part B sidebar:      #D4E8EA

TYPOGRAPHY:
  Implementation fonts: Mulish (stands in for Muller — all communication) ·
    Newsreader (stands in for Monarcha — campaign headlines).
  Weights: Mulish ExtraLight body · Regular lockup/labels · Bold headings.
  Tracking: −5 to +5. Casing: sentence case.

LAYOUT:
  Page: 1920×1080px landscape
  Padding — full page: left 120px · top 90px · right 120px · bottom 40px.
  Re-read before every section. Do not drift from earlier pages in this session.

  Master rules (all templates):
    Text top left: "Haymes Paint" / "Brand Guidelines" on two lines
      (line break before "Brand", no slash) · Mulish Regular 14pt.
    Disclaimer: Mulish Regular 9pt.

  Templates (pick by content type):
    Hero divider: full-bleed photo · text top right Newsreader Regular 20pt ·
      title 270px from top, Mulish Bold 64pt ·
      subtitle 400px from top, Newsreader Regular 50pt.
    Standard — white panel: sidebar 500px width cream/teal + white panel 1420px width.
    Standard — no panel: full-bleed cream/teal · sidebar heading same 500px left zone ·
      body in 1–4 columns: bold header + rule + body + closing rule.
      No colour-block charts, no large numerals, no rotated labels.
    Rules grid: 4-col white panel · 3× ✕ Incorrect + 1× ✓ Correct
      (verify order per page) · 0.5px primary colour dividers.
    Feature grid: sidebar + panel in equal image-led columns · no ✕/✓.
    Placeholder: sidebar normal · panel "Insert work" only · never fabricate content.
    Executional 2-page spread (Part B channel sections): each sub-section
      = 2 pages. Page 1: Social + POS artwork · Page 2: Website + eDM.
      Each page: left ~40% = 100-word lorem ipsum block (placeholder copy) ·
      right ~60% = artwork at stated format sizes. Teal sidebar.

  ASSETS (Part B is asset-heavy — follow exactly):
    [ASSET REF — filename]: place the supplied file as-is. Never recreate,
      restyle, or approximate it. Preserve its aspect ratio.
    [PLACEHOLDER — description]: render a labelled placeholder frame at the
      stated format size. Never fill with generated imagery or copy.
    Video: always a supplied keyframe image (play button already in the
      frame). Place as-is — never build a player UI or embed.

  Sidebar (all templates): Title Mulish Bold 32pt · Body Mulish ExtraLight 18pt.
  Part A = #E8E3D8 (Sections 1–13) · Part B = #D4E8EA (Sections 14–21)

LOGO: Never modify. Navy on light. White on dark or dark photography.

VOICE: Genuine · Inventive · Quirky · Feisty. Warm, direct, proudly Australian.

AVOID: Gradients · extra colours · cramped layouts · corporate tone ·
       accent in tints · white logo on light backgrounds.
```

## PART B — EXECUTIONAL PAGE LAYOUT RULES

Content panel grid: 12 columns, 24px gutter. Every artwork edge lands on a grid column — no arbitrary widths.

Format-family display: when multiple sizes of one asset exist, show ALL as scaled thumbnails
in one cluster — proportional to true pixel dimensions, common baseline per row.
Never list sizes as text.

Cluster scaffolding: each artwork group opens with a 1px hairline rule spanning the group,
small label top-left ON the rule (e.g. "SUPPLIED FORMATS — AMAO"). Filename + dimensions
in small mono BELOW each artwork as caption. Never combine label and filename on one line.

Vertical fill: artwork blocks scale to end at a consistent bottom margin — 80px above the
page number. No page ends with more than ~15% empty panel height.

Top alignment lock: sidebar heading baseline and first content-panel element share the same
top line (90px top padding). Applies to every page.

Placeholders follow the same grid and cluster rules as real artwork — structure visible now,
assets swap in later.
