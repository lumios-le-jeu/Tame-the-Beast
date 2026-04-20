# ⚡ Lean Canvas Risk Validator

> **Turn a startup idea into a validated action plan — in 3 steps.**  
> Built for entrepreneurship students who need to de-risk fast, not plan forever.

🔗 **[Live Demo → GitHub Pages](https://your-username.github.io/lean-canvas-risk-validator/)**

---

## What it does

| Step | Name | Goal |
|------|------|------|
| 1️⃣ | **Lean Canvas** | Fill all 9 boxes under time pressure |
| 2️⃣ | **Risk Assessment** | Qualify each hypothesis by colour-coded risk level + type |
| 3️⃣ | **Prioritization** | Generate a weighted, sorted de-risking roadmap |

---

## Features

### Step 1 — Timed Canvas Writing
- **9-box Lean Canvas** (Problem, Customers, Solution, UVP, Revenue, Channels, Key Metrics, Unfair Advantage, Cost Structure)
- **Global session timer** with Play / Pause / Reset
- Tracks **total sessions** and **longest session**
- **Guided navigation** — "Next Field" button cycles through boxes in logical order with visual focus highlight
- **Auto-numbered lists** in Problem & Solution boxes (press Enter → next number appears automatically)
- Everything **auto-saved** to `localStorage` — no account needed

### Step 2 — Risk Qualification
- Every line of canvas text becomes a clickable bullet
- **Click the coloured dot** → context menu to assign one of 5 risk levels:

| Colour | Level | Meaning |
|--------|-------|---------|
| 🟣 Violet | Extreme | Not tested + intuition of impossibility |
| 🔴 Red | High | Not tested + high-risk intuition |
| 🟡 Yellow | Medium | Not tested + low-risk intuition |
| 🟠 Orange | Moderate | Field surveys done, no sale yet |
| 🟢 Green | Low | Pre-sold before product existed |

- Assign a **type** per hypothesis: `Product`, `Market`, or `Customer`

### Step 3 — Antigravity Prioritization
- Set **3 profile weight sliders** (1–3) for Product / Market / Customer risk sensitivity
- Click **"Generate Priority Table"** to compute:
  ```
  Score = Colour Value × Profile Weight
  ```
  *(Violet=5, Red=4, Yellow=3, Orange=2, Green=1)*
- Results sorted **highest score first** — your most dangerous unknowns surface first
- Each row has a **"Test Path"** free-text field: *How will you test this risk before building?*
- **Export to JSON** for sharing or archiving

---

## Tech Stack

| | |
|--|--|
| **Framework** | None — pure HTML / CSS / JS |
| **Storage** | `localStorage` (browser-side, no backend) |
| **Fonts** | Inter + Space Grotesk (Google Fonts) |
| **Hosting** | GitHub Pages (static, no server needed) |

---

## Deploy to GitHub Pages

```bash
# 1. Create a new repo on GitHub
# 2. Push this folder
git init
git add .
git commit -m "feat: lean canvas risk validator"
git remote add origin https://github.com/YOUR_USERNAME/lean-canvas-risk-validator.git
git push -u origin main

# 3. In repo Settings → Pages → Source: "main branch / root"
# Your app is live at: https://YOUR_USERNAME.github.io/lean-canvas-risk-validator/
```

---

## Data Persistence

All data is stored in the browser's `localStorage` under the key `lean_canvas_v2`.  
**No data is ever sent to a server.** Students own their data entirely.

Use **Export JSON** (Step 3) to back up or share a session.

---

## License

MIT — free to use, fork, and adapt for your courses.
