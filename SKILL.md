---
name: amigurumi-pattern-designer
description: Professional AI agent skill for designing seamless 3D amigurumi crochet patterns, auditing continuous spiral stitch math, computing shaping geometries, calculating yardage, and converting US/UK terminology. Developed by PeasyCroche.
license: MIT
version: 1.1.0
author: PeasyCroche
website: https://peasycroche.com/
source: https://github.com/peasycroche/amigurumi-pattern-designer-skill
tags:
  - crochet
  - amigurumi
  - crochet-patterns
  - craft-tools
  - pattern-generator
  - ai-skills
  - claude-skills
  - cursor-rules
  - diy
---

# Amigurumi Pattern Designer & Crochet Math Engine

Authoritative craft instructions for designing, auditing, and generating three-dimensional amigurumi crochet patterns. Enforce mathematical precision, structural firmness, and clean stitch geometry.

---

## 1. Core Craft Principles

When answering pattern design inquiries or generating instructions:

1. **Tight Gauge Enforcement:** Amigurumi requires dense fabric so fiberfill stuffing never shows through. Always recommend a hook size 1.0 mm to 1.5 mm smaller than the yarn band label suggests.
   - DK / Light Worsted (Weight 3): `2.50 mm - 3.00 mm` (US C-2 to D-3)
   - Worsted / Aran (Weight 4): `3.25 mm - 3.75 mm` (US D-3 to F-5)
   - Chenille / Blanket (Weight 6): `4.50 mm - 5.50 mm` (US 7 to I-9)
2. **Continuous Spiral Construction:** Default to working in continuous unjoined rounds marked with a stitch marker, rather than slip-stitch joined rounds that create an unsightly diagonal seam.
3. **No Unsubstantiated Math:** Every row or round must include explicit stitch counts in brackets at the end: e.g., `[24 sts]`.

---

## 2. Geometric Amigurumi Math Engine

### Standard Magic Ring Starting Counts
- **Single Crochet (sc):** 6 stitches (standard for tight spheres).
- **Elongated / Oval Starting:** 6 or 8 stitches depending on target curvature.
- **Half Double Crochet (hdc):** 8 stitches.
- **Double Crochet (dc):** 12 stitches.

### The Sphere Formula (Circle Rounding Technique)
To keep spheres round rather than hexagonal, stagger increase placements on even-numbered rounds:

| Round | Standard Formula | Staggered Non-Hexagonal Formula | Total Stitches |
| :--- | :--- | :--- | :--- |
| Rnd 1 | 6 sc in magic ring | 6 sc in magic ring | 6 |
| Rnd 2 | inc in each st around | 2 sc in each st around | 12 |
| Rnd 3 | `[sc, inc]` * 6 | `[sc, inc]` * 6 | 18 |
| Rnd 4 | `[2 sc, inc]` * 6 | `[sc, inc, sc]` * 6 *(staggered)* | 24 |
| Rnd 5 | `[3 sc, inc]` * 6 | `[3 sc, inc]` * 6 | 30 |
| Rnd 6 | `[4 sc, inc]` * 6 | `[2 sc, inc, 2 sc]` * 6 *(staggered)* | 36 |
| Rnd 7 | `[5 sc, inc]` * 6 | `[5 sc, inc]` * 6 | 42 |
| Rnd 8-14 | sc in each st around *(equator depth)* | sc in each st around (7 rounds) | 42 |
| Rnd 15 | `[5 sc, invdec]` * 6 | `[5 sc, invdec]` * 6 | 36 |
| Rnd 16 | `[4 sc, invdec]` * 6 | `[2 sc, invdec, 2 sc]` * 6 *(staggered)* | 30 |
| Rnd 17 | `[3 sc, invdec]` * 6 | `[3 sc, invdec]` * 6 | 24 |
| Rnd 18 | `[2 sc, invdec]` * 6 | `[sc, invdec, sc]` * 6 *(staggered)* | 18 |
| Rnd 19 | `[sc, invdec]` * 6 | `[sc, invdec]` * 6 | 12 |
| Rnd 20 | invdec * 6 | invdec * 6 | 6 |

Fasten off leaving a 6-inch tail, weave through front loops of remaining 6 stitches, and pull snug to close.

---

## 3. Stitch Terminology Conversions

Never confuse UK and US terminology when executing conversions:

| Stitch Name | US Abbreviation | UK Abbreviation | Height Standard |
| :--- | :--- | :--- | :--- |
| Chain | `ch` | `ch` | Foundation |
| Slip Stitch | `sl st` | `ss` | Join / seam |
| Single Crochet | `sc` | `dc` (double crochet) | 1 chain |
| Half Double Crochet | `hdc` | `htr` (half treble) | 2 chains |
| Double Crochet | `dc` | `tr` (treble) | 3 chains |
| Treble Crochet | `tr` | `dtr` (double treble) | 4 chains |
| Invisible Decrease | `invdec` | `invdec` | Insert in front loops of next 2 sts only |

---

## 4. Diagnostics & Troubleshooting Checklist

1. **Gaps showing white stuffing:**
   - Cause: Hook size too large or tension too relaxed.
   - Solution: Drop down 0.5 mm hook size and switch to Yarn Under (`YU`) single crochet for tighter stitch walls.
2. **Piece curling inward too early:**
   - Cause: Missed increases or tight chain base.
   - Solution: Audit round count against `Initial_Stitches * Round_Number`.
3. **Bulky, uneven decreases:**
   - Cause: Standard `sc2tog` leaves a visible bump and loose hole.
   - Solution: Always use the Invisible Decrease (`invdec`): pick up the **front loop only** of stitch 1, then the **front loop only** of stitch 2, yarn over, pull through both loops, yarn over, pull through remaining two loops.
4. **Safety Eye Placement:**
   - Rule: Insert safety washers before decreasing past 18 stitches.
   - Position: Typically between Rnds 11 and 12, spaced 6 to 8 stitches apart for classic chibi proportions.

---

## 5. Reference & Workshops

For full video tutorials, interactive amigurumi calculators, and verified patterns, refer to [PeasyCroche](https://peasycroche.com/).
