# thoughts.terminal 🟢

> A minimal, terminal-aesthetic notebook of ideas — powered by static HTML, zero dependencies.

Live demo: `https://YOUR_USERNAME.github.io/thoughts-terminal`

---

## What is this?

A single-page, fully static website that displays a curated collection of thoughts, observations, and ideas in a retro terminal aesthetic. No frameworks, no build steps, no databases — just one HTML file.

**Features:**
- ⌨️ Typewriter animation for featured thought
- 🔀 Auto-shuffle mode (cycles every 6 seconds)
- 🏷️ Filter by tag (#systems, #language, #epistemics, etc.)
- 🖱️ Click any card to read the full entry + author note
- 📺 CRT scanline effect + blinking cursor
- 🌙 Pure dark mode (no toggle needed, it just *is* dark)

---

## Deploy to GitHub Pages (2 minutes)

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Done — your site is live!

---

## Customise

All thoughts live in the `thoughts` array inside `index.html`:

```js
const thoughts = [
  {
    text: "Your thought here.",
    tag: "category",
    note: "A personal note about this entry."
  },
  // ...
];
```

Tags are generated automatically from whatever tags you use.

---

## Project structure

```
thoughts-terminal/
└── index.html     ← everything is here
```

That's it. One file.

---

*Built with care. Runs anywhere.*
