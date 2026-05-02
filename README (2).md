# Mathelicious Learning

An interactive calculus learning library — each quest teaches one big idea through hands-on exploration, drag-and-drop reasoning, and graphical intuition. No memorisation required.

Every quest is a **single self-contained HTML file** — no frameworks, no dependencies, no install.

---

## Live Site

> **[rkchina79.github.io/Mathelicious-Learning](https://rkchina79.github.io/Mathelicious-Learning)**

---

## The Quest Library

| Quest | Topic | Problems | Status |
|---|---|---|---|
| **Limits Quest** | What limits mean, graphically and algebraically | 32 | ✅ Live |
| **Derivatives Quest** | Slopes, differentiation rules, L'Hôpital's Rule | 30 | ✅ Live |
| **Integrals Quest** | Riemann sums, area under a curve, antiderivatives | — | 🔜 Coming soon |
| **Series Quest** | Convergence, divergence, common series tests | — | 🔜 Coming soon |

New quests are added to the library over time. Each one builds on the last.

---

## Quest 1 — Limits Quest (`Limits.html`)

Builds intuition for what limits mean before touching any algebra.

### Part 1 — Graphical Limits
Dual interactive sliders approach from both sides. The graph updates in real time showing values converging (or not).

Covers: continuous functions · rational functions with holes · vertical asymptotes · piecewise jumps · limits at infinity · both sides → ±∞

### Part 2 — One-Sided Limits & Squeeze Theorem
Left-hand and right-hand limits explored separately, then compared.

Covers: one-sided limits · two-sided existence · ln(x) → −∞ · Squeeze Theorem · oscillating limits (sin 1/x) · floor function · both sides → ∞

### Part 3 — Algebraic Methods (Drag & Drop)
Step-by-step solutions built by dragging answer tiles into blanks.

Covers: direct substitution · factoring · rationalisation · limit laws · infinity rule (divide by highest power)

---

## Quest 2 — Derivatives Quest (`Derivatives.html`)

From slopes on a curve to the full differentiation toolkit. Builds directly on Limits Quest.

### Part 1 — Graphical Derivatives
Tangent line slider + dual-graph shape problems + two-slider differentiability check.

Covers: slope at a point · tangent lines · shape of f′(x) · left = right derivative · |x| not differentiable at 0

### Part 2 — Differentiation Rules (MCQ + Drag & Drop)
Progressively harder — power rule → product → quotient → chain → combined.

Covers: power rule · product rule · quotient rule · chain rule · chain + product combined

### Part 3 — L'Hôpital's Rule (Drag & Drop)
Identify the indeterminate form, verify the condition, then differentiate top and bottom step by step.

Covers: 0/0 form · ∞/∞ form · applying twice · when the rule does NOT apply · connection back to Limits Quest

---

## Shared Features (all quests)

| Feature | Detail |
|---|---|
| **Interactive graphs** | Chart.js with live tangent lines and dual-graph derivative building |
| **Randomised answer choices** | MCQ options shuffled on every render — correct answer never in the same position |
| **Backward navigation** | Click any completed problem to review it; explanation shown immediately |
| **Proper math notation** | Stacked fractions, superscripts, lim with x→a subscript, prime notation |
| **No answer spoilers** | Answer hidden until student selects correct option or fills all blanks |
| **Progressive hints** | Wrong answers unlock hints one at a time, never reveal outright |
| **Partial credit** | 10–15 pts for first attempt, reduced for retries |
| **Responsive** | Works on laptop, tablet, and mobile |
| **Zero dependencies** | Single HTML file per quest, Chart.js from CDN only |

---

## How to Use

### Option A — Run locally
Download any `.html` file and open it in any browser. No server needed.

### Option B — GitHub Pages (current setup)
The repo is already configured. Any file added to the root is live at:
```
https://rkchina79.github.io/Mathelicious-Learning/filename.html
```

### Option C — Embed on your website
```html
<iframe
  src="https://rkchina79.github.io/Mathelicious-Learning/Limits.html"
  width="100%"
  height="850px"
  style="border:none; border-radius:12px;">
</iframe>
```

---

## Repo Structure

```
Mathelicious-Learning/
├── index.html          ← Landing page (links to all quests)
├── Limits.html         ← Quest 1: Limits
├── Derivatives.html    ← Quest 2: Derivatives
└── README.md           ← This file
```

As new quests are added, each one is a single new `.html` file dropped into the root and linked from `index.html`.

---

## Tech Stack

- **Vanilla HTML / CSS / JavaScript** — no build step, no framework
- **[Chart.js 4.4.1](https://www.chartjs.org/)** — interactive graphs (CDN)
- **[Google Fonts](https://fonts.google.com/)** — Nunito + Space Mono
- All game logic, rendering, state management, and drag-and-drop hand-written

---

## Roadmap

- [x] Limits Quest
- [x] Derivatives Quest
- [ ] Integrals Quest
- [ ] Series & Sequences Quest
- [ ] Teacher mode — track class progress
- [ ] Score persistence across sessions

---

## About

Built for **Mathelicious Learning** — interactive calculus experiences designed to build genuine understanding, not just procedural recall.

> *"The goal is not to memorise the answer — it's to see why the answer must be what it is."*

---

## License

MIT — free to use, adapt, and share with attribution.
