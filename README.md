# A Model-Based Framework for Dexterous In-Hand Tweezers Manipulation

A single-page reading edition of the paper, typeset in a **Kandinsky / Bauhaus constructivist** style.

## What this is

Dexterous hands are usually just graspers — the arm does the moving. This framework flips that
around: with the wrist locked, finger articulation alone drives the tweezer tip through a ±5 mm
Cartesian workspace, and the hand ends up looking like a small, redundant manipulator with the
*tool tip* as its end effector.

## Pages

| File | Edition |
|---|---|
| `index.html` | English (primary) |
| `zh.html` | 中文精读版 |

Both editions carry a switch chip in the hero meta row.

## Design

| Dimension | Approach |
|---|---|
| Palette | rice-paper `#F2EEE3` + charcoal `#131313` + Bauhaus primaries (vermilion `#DF3524` / chrome yellow `#F0C200` / ultramarine `#1D3FA6`), flat fills only |
| Type | Jost (geometric sans, Futura-adjacent) for display, Noto Sans SC for body, IBM Plex Mono for numerals |
| Layout | square corners, no gradients, no shadows, hard-edged rules; left spine, right section nav, tri-colour reading progress |
| Artwork | hero and inline plates are pure geometric compositions (circle / triangle / square / concentric arcs / hard diagonals) |
| Maths | every equation rendered live with KaTeX — selectable, copy-ready LaTeX |
| Motion | staggered hero reveal, scroll reveal, section tracking nav, `prefers-reduced-motion` aware |

## Files

```
.
├── index.html            # English edition (self-contained design system; CDN fonts + KaTeX only)
├── zh.html               # Chinese edition
├── assets/images/        # 5 Bauhaus plates
├── .nojekyll             # disable Jekyll
└── README.md
```

## Series

- Part 1 (this page) — pure analytical kinematics, fixed wrist
- [Part 2 — Model + Vision + Touch](https://fangde.github.io/kandinsky-tweezers-vision-touch/)

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Licence

The paper text and figures remain the property of the original authors; this repository only
presents the typography and reading experience.
