# thoughts.terminal 🟢

> 一個極簡的終端機風格筆記本，收錄各種想法與觀察 — 純靜態 HTML，零依賴。

Live demo: `https://gmyjade.github.io/w14-github`

---

## 這是什麼？

一個單頁、完全靜態的網站，以復古終端機風格呈現精選的思緒、觀察與想法。無框架、無建置流程、無資料庫——就是一個 HTML 檔案。

**功能特色：**
- ⌨️ 精選思緒的打字機動畫
- 🌐 中英文一鍵切換（右上角語言按鈕）
- 🔀 自動隨機播放模式（每 6 秒循環）
- 🏷️ 依標籤篩選（#systems、#language、#epistemics 等）
- 🖱️ 點擊任何卡片，閱讀完整內容與作者筆記
- 📺 CRT 掃描線效果 + 閃爍游標
- 🌙 純深色模式（不需切換，就是深色）

---

## 部署到 GitHub Pages（2 分鐘）

1. 將此 repo 推送到 GitHub
2. 進入 **Settings → Pages**
3. 來源設為 `main` 分支、`/ (root)` 資料夾
4. 完成——你的網站已上線！

---

## 如何自訂

所有思緒內容存放在 `index.html` 的 `thoughts` 陣列中：

```js
const thoughts = [
  {
    zh: "你的中文內容。",
    en: "Your English content.",
    tag: "category",
    note_zh: "關於這則條目的中文筆記。",
    note_en: "A personal note about this entry."
  },
  // ...
];
```

標籤會自動從你所使用的 tag 值生成。

---

## 語言切換

點擊右上角的 **EN / 中** 按鈕即可切換語言，所有文字（思緒、筆記、介面文字）都會即時更新。

---

## 專案結構

```
thoughts-terminal/
└── index.html     ← 一切都在這裡
```

就這樣。一個檔案。

---

---

# thoughts.terminal 🟢

> A minimal, terminal-aesthetic notebook of ideas — powered by static HTML, zero dependencies.

Live demo: `https://gmyjade.github.io/w14-github/`

---

## What is this?

A single-page, fully static website that displays a curated collection of thoughts, observations, and ideas in a retro terminal aesthetic. No frameworks, no build steps, no databases — just one HTML file.

**Features:**
- ⌨️ Typewriter animation for featured thought
- 🌐 One-click Chinese/English toggle (top-right language button)
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
    zh: "你的中文內容。",
    en: "Your English content.",
    tag: "category",
    note_zh: "關於這則條目的中文筆記。",
    note_en: "A personal note about this entry."
  },
  // ...
];
```

Tags are generated automatically from whatever tags you use.

---

## Language Toggle

Click the **EN / 中** button in the top-right corner to switch languages. All content (thoughts, notes, and UI text) updates instantly.

---

## Project structure

```
thoughts-terminal/
└── index.html     ← everything is here
```

That's it. One file.

---

*Built with care. Runs anywhere.*