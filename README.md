# Business Card — freeCodeCamp Lab (AI-Driven Development Practice)

A responsive, styled **digital business card** built for the [freeCodeCamp "Design a Business Card" lab](https://www.freecodecamp.org/learn/full-stack-developer/lab-design-a-business-card/).

> **🎯 Primary goal of this repo:** practice **AI-driven development** using [Cline](https://cline.bot/) (in VS Code) with a GLM model (`glm-5.3-flash`) — not just to finish the lab, but to explore how far an agentic coding workflow can take a task end-to-end: reading specs, planning, implementing, and validating against automated tests.

---

## 📖 About This Project

The business card displays:

- A **profile image** with a meaningful `alt` description
- **Full name**, **designation**, and **company**
- **Email** and **phone** contact details
- A **Portfolio** link and **social media** links (Twitter, LinkedIn, GitHub)
- All wrapped in a centered 300px card on a `rosybrown` background

Beyond the lab requirements, the card includes some personal styling touches: gradient accents, hover effects, a circular profile photo with a ring, and pill-shaped link buttons.

## 🤖 Why This Exists — AI-Driven Development Practice

This project is a deliberate exercise in **agentic coding workflows**:

| Practice area | What was exercised |
|---|---|
| **Spec-driven prompting** | Feeding the lab's 41 user stories + test list to Cline and letting it derive the implementation |
| **Plan vs. Act modes** | Using Cline's plan mode to align on structure before writing any code |
| **Context handling** | Working with `AGENTS.md` as the workspace-level task specification |
| **Iterative refinement** | Requesting styling polish ("give it your own personal style") through follow-up prompts |
| **Validation loop** | Checking the generated HTML/CSS against the lab's automated test suite (41/41 passing) |

**Stack used:** Cline + `glm-5.3-flash` model, inside VS Code.

## 🗂️ Project Structure

```
business-card/
├── index.html      # Business card markup (semantic HTML)
├── styles.css      # All styling (layout, gradients, hover effects)
├── AGENTS.md       # Lab specification: user stories + test checklist
├── package.json    # Project metadata
└── README.md       # This file
```

## 🚀 Getting Started

No build step or dependencies required — it's plain HTML + CSS.

**Option 1 — Open directly:**

```bash
open index.html   # macOS
```

**Option 2 — Serve locally (recommended):**

```bash
npx serve .
# or
python3 -m http.server 8080
```

Then visit the printed URL (e.g. `http://localhost:3000` or `http://localhost:8080`).

## ✅ Requirements Fulfilled

The implementation satisfies all **41 lab tests**, including:

- ✅ One main `div.business-card` containing all elements
- ✅ `img.profile-image` with valid source and meaningful `alt`
- ✅ `p.full-name`, `p.designation`, `p.company` (in order, after the image)
- ✅ Two `hr` dividers — one before contact info, one after the portfolio link
- ✅ Email and phone `p` elements
- ✅ `a.portfolio-link` with text "Portfolio" and a valid `href`
- ✅ `div.social-media` containing `h2` "Connect with me" + Twitter/LinkedIn/GitHub links
- ✅ `styles.css` linked via `<link rel="stylesheet" href="styles.css">` in `<head>`
- ✅ Page background `rosybrown`; font `Arial, sans-serif`
- ✅ `.business-card`: `width: 300px`, valid `background-color`, `padding: 20px`, `margin-top: 100px`, `text-align: center`, `font-size: 16px`, left/right margins `auto`
- ✅ `.profile-image`: `max-width: 100%`
- ✅ All `p` elements: `margin-top/bottom: 5px`
- ✅ All links: no underline

## 🧪 Testing

The lab's automated test suite runs on the freeCodeCamp platform. To verify:

1. Open the [lab page](https://www.freecodecamp.org/learn/full-stack-developer/lab-design-a-business-card/) and start the project.
2. Paste the contents of `index.html` and `styles.css` into the editor.
3. Run the tests — all 41 should pass.

## 🛠️ Tech Stack

- **HTML5** — semantic markup
- **CSS3** — flexbox-free simple layout, gradients, transitions, `::before`/`::after` decorations
- **Cline (AI agent)** + **GLM model** — AI-driven development

## 📄 License

For educational purposes as part of the freeCodeCamp curriculum.
