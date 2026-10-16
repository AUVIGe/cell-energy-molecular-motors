# From a Meal to Lifting a Barbell

**How cells spend energy, and how molecular motors lift you up** — an interactive, offline-friendly
illustrated explainer. Zero background assumed: from food → ATP → one myosin power stroke →
muscle contraction → a barbell leaving the floor.

**Live:** https://auvige.github.io/cell-energy-molecular-motors/

## What is inside

| Page | Contents |
|---|---|
| [`index.html`](index.html) | English interactive 3D network: 21 nodes, 22 procedural 3D models, per-sentence narration, nine guided steps |
| [`zh.html`](zh.html) | The same 3D network in Chinese |
| [`article-en.html`](article-en.html) | English long read: 12 data figures, 8 tables, 11 collapsible Q&A, quick-reference appendix |
| [`article.html`](article.html) | Chinese long read |

Every page is a single file with no external requests: three.js is inlined, and the 3D models are
generated procedurally in code, so the 3D pages work offline from `file://` as well.

## Features

- **Nine-step guided tour** — deposit (food) → withdrawal (respiration) → cash (ATP) →
  payment (hydrolysis) → command (nerve and calcium) → power stroke → superposition →
  result (the barbell rises) → audit (78% becomes heat).
- **Bilingual everywhere** — UI, step cards, node labels, the 64 annotations inside the 3D models,
  80 stage narrations, the mini animation window and the narration voice itself.
  Text inside the two hand-drawn SVG diagrams switches with the language too.
- **Narration that finishes before advancing** — each sentence is queued and the next step only
  starts after the speech engine reports it has actually stopped, so nothing is cut off.
- **Mini animation window** — a grey-backdrop inset in the top-right shows the exact molecular
  process being described, synchronised to each sentence.
- **Real processes, not just spinning** — the models run actual mechanisms: γ-phosphate dropping
  off ATP, protons crossing the membrane, the cross-bridge cycle, sarcomere sliding,
  calcium release and re-uptake, force adding up from 4 pN to hundreds of newtons.

## Key numbers used

| Quantity | Value |
|---|---|
| Free energy of ATP hydrolysis | ≈ 8×10⁻²⁰ J per molecule (ΔG ≈ −50 kJ/mol) |
| Body ATP stock / daily turnover | ≈ 50–60 g / ≈ 50–75 kg |
| One myosin stroke | ≈ 10 nm, ≈ 4 pN, one ATP |
| Sarcomere | 2.2 µm → 1.6 µm (A-band constant) |
| Lifting 20 kg by 1 m | 196 J of external work, ≈ 1,950 J metabolic, ≈ 0.47 kcal |

## Sources

Huxley & Niedergerke (1954) and Huxley & Hanson (1954) on sliding filaments; Hill (1938) on the
force–velocity relation; Finer, Simmons & Spudich (1994, *Nature*) on single-molecule force and step
size; Kinosita and colleagues on F₁-ATP synthase rotation; single-molecule kinesin work by Block,
Svoboda, Vale and others; plus *Guyton & Hall*, *Lehninger* and *Alberts* as textbook references.

Values are order-of-magnitude estimates meant to build intuition and check self-consistency.

## Note

The figures are regenerated from scripts, not hand-edited: PNG data figures come from
matplotlib scripts and both structural diagrams are bilingual SVG.
