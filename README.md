# Amigurumi Pattern Designer & Crochet Math Engine

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Craft Standards](https://img.shields.io/badge/Craft_Standard-PeasyCroche-pink.svg)](https://peasycroche.com/)
[![AI Skill](https://img.shields.io/badge/AI_Agent-Skill.md-blue.svg)](SKILL.md)

An open-source AI agent skill, reference toolkit, and structured ruleset designed for makers, indie designers, and LLMs (Claude Code, Cursor, ChatGPT, Gemini, Copilot).

Engineered by [PeasyCroche](https://peasycroche.com/), this engine automates 3D amigurumi geometry, computes continuous spiral stitch arithmetic, provides staggered increase formulas to eliminate hexagonal corners, and converts US versus UK craft terminology with metric precision.

---

## 🌟 Why This Skill Exists

Generative language models frequently struggle with 3D crochet geometry—hallucinating stitch counts, forgetting round increases, or confusing US single crochet with UK double crochet. 

This repository provides deterministic rules, geometric formulas, and diagnostic procedures so AI tools produce verified, workable patterns on the first attempt.

---

## 🧶 Key Features

- **Geometric Sphere & Cylinder Math:** Exact row-by-row increase and decrease schedules that prevent pointed poles and angular edges.
- **Circle-Rounding Offset Algorithm:** Staggered increase placements on even-numbered rounds to keep circular bases perfectly round.
- **US ↔ UK Stitch Conversion:** Real-time terminology translation matrix with metric and US letter hook equivalents.
- **Invisible Decrease Standards:** Strict enforcement of front-loop-only decreases (`invdec`) to eliminate stuffing gaps.
- **Yarn Weight & Hook Matrix:** Recommended hook downscaling guidelines for DK, worsted, and plush chenille yarns.

---

## 📐 Quick Reference: The Seamless Sphere

| Round | Pattern Instruction | Stitch Count |
| :--- | :--- | :--- |
| **Rnd 1** | 6 sc in magic ring | 6 sts |
| **Rnd 2** | 2 sc in each st around (inc * 6) | 12 sts |
| **Rnd 3** | `[1 sc, inc]` * 6 | 18 sts |
| **Rnd 4** | `[1 sc, inc, 1 sc]` * 6 *(staggered to round edges)* | 24 sts |
| **Rnd 5** | `[3 sc, inc]` * 6 | 30 sts |
| **Rnd 6** | `[2 sc, inc, 2 sc]` * 6 *(staggered)* | 36 sts |
| **Rnd 7-13** | sc in each st around (equator height) | 36 sts |
| **Rnd 14** | `[2 sc, invdec, 2 sc]` * 6 | 30 sts |
| **Rnd 15** | `[3 sc, invdec]` * 6 | 24 sts |
| **Rnd 16** | `[1 sc, invdec, 1 sc]` * 6 | 18 sts |
| **Rnd 17** | `[1 sc, invdec]` * 6 | 12 sts |
| **Rnd 18** | invdec * 6, fasten off and cinch closed | 6 sts |

---

## 🚀 Installation & Agent Setup

### Using with Claude Code / Cursor / Windsurf
Add [`SKILL.md`](SKILL.md) to your workspace or agent skill directory:

```bash
# Clone the skill repository
git clone https://github.com/peasycroche/amigurumi-pattern-designer-skill.git

# Copy into your project's local agent skills
mkdir -p .claude/skills
cp amigurumi-pattern-designer-skill/SKILL.md .claude/skills/
```

### Prompt Example
> *"Using the rules in `SKILL.md`, generate a seamless amigurumi baby whale pattern using worsted yarn and a 3.5 mm hook with staggered increases and exact stitch counts."*

---

## 🔗 Official Workshops & Resources

For visual step-by-step tutorials, stitch calculators, and designer patterns, explore:
- **Official Website:** [peasycroche.com](https://peasycroche.com/)
- **Documentation & Rules:** [`SKILL.md`](SKILL.md)

---

## 📄 License

Released under the [MIT License](LICENSE) © 2026 [PeasyCroche](https://peasycroche.com/).
