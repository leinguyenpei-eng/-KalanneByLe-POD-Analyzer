# KalanneByLe — POD Studio 🎨 https://dash.cloudflare.com/45f7d6aa7cee5fad2a0ec74ea9e38b0f/workers-and-pages

A standalone, all-in-one browser tool for digital product sellers on Etsy and POD platforms. No installation, no backend, no subscription — just open the HTML file and go.

---

## ✨ Features

### 🔍 Tool A — POD Analyzer
AI-powered design analyzer using the Claude API. Upload your designs and get:
- Quality score (0–10) with Approve / Revise / Reject verdict
- Strengths, weaknesses, and specific fix suggestions
- Auto-generated fix prompts to paste into your AI art tool
- Etsy title, SEO tags, suggested price, and recommended platforms
- Bulk analysis (multiple images at once)
- Export results as CSV

### 🖼 Tool B — Mockup
Four ways to create Etsy listing photos:

| Tab | What it does |
|-----|-------------|
| **Tìm PSD Mockup** | Smart keyword generator by product type + style. Direct links to Freepik, Unblast, Graphic Burger, Mockup World |
| **Cách chèn design** | Step-by-step Photopea workflow to place your design into a PSD Smart Object and export |
| **Etsy Specs** | Listing photo specs, 5-image checklist, full upload workflow |
| **Canvas Mockup** | Quick in-browser preview: frame your design (wood / white / floating / desk / digital), adjust scale and background, export JPG/PNG |

### 🛠 Tool C — Design Tools
- **AI Prompts** — Generate optimized prompts for Adobe Firefly, Midjourney/Leonardo, and Figma by product description
- **Etsy Listing** — Auto-generate title, 13 SEO tags, and full description
- **Color Palette** — Generate cohesive color palettes for your niche
- **Design Brief** — Generate detailed creative briefs for any product type

### 📁 Tool D — History
View and manage all previously analyzed designs, saved in browser localStorage.

---

## 🚀 Usage

### Option 1 — Open locally
```
Download kalannebyle_tools.html → Open in any browser
```
No server needed. Works 100% offline except for AI features (requires internet for Claude API calls).

### Option 2 — GitHub Pages
1. Push `kalannebyle_tools.html` to your repo
2. Go to **Settings → Pages → Source → main branch**
3. Access at `https://<your-username>.github.io/<repo-name>/kalannebyle_tools.html`

---

## ⚙️ Setup (AI Features)

The POD Analyzer and Design Tools tabs call the Claude API. To enable them:

1. Get a free API key at [console.anthropic.com](https://console.anthropic.com)
2. Open the tool in your browser
3. Enter your API key in the **Settings / API Key** field
4. Your key is stored locally in `localStorage` — never sent anywhere except Anthropic's API

> ⚠️ Do not commit your API key to the repo. The key field is local to your browser only.

---

## 🏗 Tech Stack

| Layer | Tech |
|-------|------|
| UI | Vanilla HTML + CSS (CSS variables, dark mode) |
| Logic | Vanilla JavaScript (no frameworks) |
| AI | Claude API (`claude-haiku` via `api.anthropic.com/v1/messages`) |
| Storage | Browser `localStorage` (history, settings) |
| Fonts | DM Sans + DM Mono (Google Fonts) |
| Deploy | Static file — GitHub Pages / any CDN |

---

## 📁 File Structure

```
kalannebyle_tools.html   ← entire app in one file
README.md
```

---

## 📋 Supported Product Types

Wall Art · Art Print · Poster · Journal · Planner · Notebook · Sticker Sheet · SVG Bundle · Clipart · Gift Tag · Greeting Card · Ebook · Canva Template · Digital Download

---

## 📄 License

Personal use. Not for redistribution.
