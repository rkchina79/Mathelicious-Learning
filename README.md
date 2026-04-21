# Mathelicious Learning — Limits Quest

An interactive calculus puzzle game that teaches limits through three progressive learning modes: graphical exploration, conceptual reasoning, and algebraic evaluation. Built as a single self-contained HTML file — no frameworks, no dependencies, no install.

---

## What's Inside

### Part 1 — Graphical Limits
Students explore limits visually using **dual interactive sliders** — one approaching from the left, one from the right. The graph updates in real time as sliders move, showing y-values converging (or not) toward the limit point.

Covers:
- Continuous functions — limit always exists
- Rational functions with holes — limit can still exist
- Vertical asymptotes — left and right go opposite directions (DNE)
- Piecewise jump discontinuities — left ≠ right (DNE)
- Limits at infinity — function settles toward a horizontal asymptote
- Both sides approaching +∞ or −∞ together

### Part 2 — One-Sided Limits & Squeeze Theorem
Students work with left-hand and right-hand limits **separately**, then compare them. Includes the Squeeze Theorem with three curves shown simultaneously on the graph.

Covers:
- Right-hand and left-hand limits in isolation
- Two-sided limit existence and non-existence
- ln(x) → −∞ as x → 0⁺
- Squeeze Theorem (x²·sin(1/x) and similar)
- Oscillating limits (sin(1/x)) — DNE
- Floor function one-sided limits
- Both sides approaching infinity from the same direction

### Part 3 — Algebraic Methods (Drag & Drop)
Students build step-by-step solutions by dragging tiles into blanks. Every blank must be filled correctly before the answer is revealed. Tiles are reusable and shuffled on each attempt.

Covers:
- Direct substitution
- Factoring (difference of squares, trinomials — both factors blank on harder problems)
- Rationalisation (conjugate method for square roots)
- Limit laws (sum law, product law)
- Infinity rule (divide by highest power)

---

## Features

| Feature | Detail |
|---|---|
| **Interactive graphs** | Chart.js scatter plots with live marker tracking |
| **Dual sliders** | Left fills left→right (blue), right fills right→left (green) |
| **Proper math notation** | Stacked fractions, superscripts, lim with x→a subscript |
| **No answer spoilers** | Limit value hidden until student selects correct answer |
| **Retry on wrong** | Wrong answers flash and allow unlimited retries with progressive hints |
| **Commutative factoring** | Factor order doesn't matter — (x−2)(x+3) = (x+3)(x−2) both accepted |
| **Scoring** | 10–15 pts for correct answers, partial credit for retries |
| **Streak tracker** | Visual dot history of recent answers |
| **Responsive** | Works on laptop, tablet, and mobile |
| **Zero dependencies** | Single HTML file, loads Chart.js from CDN only |

---

## How to Use

### Option A — Run locally
Download `index.html` and open it in any browser. No server needed.

### Option B — Host on GitHub Pages
1. Fork or upload `index.html` to a public repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/(root)` folder
4. Your site is live at `https://yourusername.github.io/repo-name/`

### Option C — Embed on your website
```html
<iframe
  src="https://yourusername.github.io/mathelicious-puzzles/"
  width="100%"
  height="850px"
  style="border:none; border-radius:12px;">
</iframe>
```

---

## Problem Breakdown

| Part | Problems | Topics |
|---|---|---|
| Part 1 | 10 | Continuous, holes, asymptotes, jumps, infinity, both-sided ∞ |
| Part 2 | 10 | One-sided, DNE, squeeze theorem, oscillation, floor function, both-sided ∞ |
| Part 3 | 12 | Substitution ×2, factoring ×3, rationalisation ×2, limit laws ×2, infinity rule ×2, both-factor-blank ×3 |

**Total: 32 problems across 3 parts**

---

## Tech Stack

- **Vanilla HTML/CSS/JavaScript** — no build step, no framework
- **[Chart.js 4.4.1](https://www.chartjs.org/)** — graphs (loaded from CDN)
- **[Google Fonts](https://fonts.google.com/)** — Nunito + Space Mono
- All game logic, rendering, and state management hand-written in ~1,300 lines

---

## Project Structure

```
mathelicious-puzzles/
└── index.html        ← The entire app (HTML + CSS + JS)
└── README.md         ← This file
```

---

## Roadmap

- [ ] Derivatives module (definition as a limit, power rule, chain rule)
- [ ] Integrals module (Riemann sums, area under curve)
- [ ] Score persistence (localStorage)
- [ ] Teacher mode — track class progress
- [ ] Printable problem sets

---

## About

Built for **Mathelicious Learning** — interactive calculus puzzles designed to build genuine understanding, not just procedural recall.

> *"The goal is not to memorise the answer — it's to see why the answer must be what it is."*

---

## License

MIT — free to use, adapt, and share with attribution.
