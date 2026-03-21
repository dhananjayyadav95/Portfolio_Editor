# 🌐 Portfolio Editor Pro

> **A fully visual portfolio website builder — no coding, no tools, no hosting cost.**  
> Upload your photos, fill in your details, pick a color, and download a production-ready website in minutes.

<br/>

![Status](https://img.shields.io/badge/Status-Live-22C55E?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-3B82F6?style=flat-square)
![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-E11D48?style=flat-square)
![Single File](https://img.shields.io/badge/Single%20File-HTML%20Only-F59E0B?style=flat-square)
![Image Upload](https://img.shields.io/badge/Image%20Upload-Built%20In-7C3AED?style=flat-square)

---

## ✨ What is this?

**Portfolio Editor Pro** is a single HTML file that runs entirely in your browser. Open it, fill in your details, upload your photos, and click **Download**. You get a complete, polished portfolio website — fully animated, dark-mode-ready, and mobile-friendly — with zero code required.

No npm. No build step. No server. Just one file.

---

## 🚀 Live Demo

👉 **[Try the Editor Live](https://yourusername.github.io/portfolio-editor)**

> Replace the link above with your GitHub Pages URL after deploying.

---

## 📦 What's in this repo?

```
portfolio-editor/
├── index.html    ← The entire editor (open this in your browser)
└── README.md     ← You are here
```

One file. That's it.

---

## 🎬 How to use it — 5 steps

### Step 1 — Open the editor
Download `index.html` and double-click it. It works in Chrome, Firefox, Edge, and Safari with no installation.

### Step 2 — Fill in your 7 tabs

| Tab | What you edit |
|---|---|
| 👤 **Personal** | Name, title, bio, status badge, typing roles, fun facts, stats |
| 📸 **Photos** | Upload hero photo, about photo, and per-project images — drag & drop supported |
| 🎯 **Skills** | Skill names with progress bar percentages, tech badge cloud |
| 🏢 **Experience** | Jobs, dates, company, location, descriptions |
| 🚀 **Projects** | Project cards with title, description, tags, category, GitHub & live links |
| 📬 **Contact** | Email, LinkedIn, GitHub, Twitter, Calendly, Formspree form ID, SEO meta |
| 🎨 **Style** | 16 accent color swatches + custom hex, default dark/light mode, hero background style |

### Step 3 — Upload your photos
Go to the **Photos tab**. Click (or drag & drop) to upload:
- Your **hero photo** — shown as a circle in the banner
- Your **about photo** — shown in the About Me section
- A **cover image for each project** — shown on project cards and in modals

All images are embedded directly into the downloaded HTML — no separate image files needed.

### Step 4 — Preview in real time
The right panel shows a live browser preview that updates as you type. Toggle **☀ Light / 🌙 Dark** at the top to see both modes.

### Step 5 — Download and deploy
Click **Download index.html**. Then drag it onto [Netlify](https://netlify.com) or upload to GitHub Pages — you're live in under 2 minutes.

---

## 🛠️ Editor features

- **Live preview** — every keystroke updates the preview instantly
- **Image upload** — drag & drop or click to upload; images are base64-embedded in the output
- **Light / Dark preview toggle** — see exactly how your site looks in both modes before downloading
- **Save Progress** — saves everything (including images) to your browser so you can close and come back
- **Restore** — one-click to reload your last session
- **Copy HTML** — copies the complete generated HTML to clipboard
- **Download index.html** — generates and saves your portfolio as a single self-contained file

---

## 🌟 What the generated portfolio includes

- **Sticky navbar** — scroll-aware, mobile hamburger menu
- **Full-screen hero** — your photo, name, animated typing roles, status badge, and CTA buttons
- **About section** — photo, bio, fun facts, stats (years / projects / clients)
- **Skills** — animated progress bars triggered on scroll + tech badge cloud
- **Experience timeline** — clean two-column layout with dates, company, and descriptions
- **Projects grid** — filterable by category (Software / Hardware / AI / Design / Other), 3D tilt cards, modal popups with full project details
- **Contact form** — async submit via Formspree, no backend needed
- **Dark / Light mode toggle** — persisted via `localStorage`, zero flash on load
- **Scroll progress bar** — accent-colored bar at the top of the page
- **Back to top button** — appears after scrolling down
- **Loading spinner** — polished fade-in on first visit
- **Print CSS** — clean layout when printed as a CV (Ctrl+P)
- **SEO ready** — `<title>`, `<meta description>`, Open Graph, and Twitter card tags
- **Fully responsive** — works on all screen sizes

---

## 🌍 Deploying to GitHub Pages

1. [Create a GitHub account](https://github.com/signup) if you don't have one
2. Go to [github.com/new](https://github.com/new) → name it `portfolio-editor` → **Public**
3. Click **"uploading an existing file"**
4. Upload `index.html` (rename it from `portfolio-editor.html` if needed) and `README.md`
5. Go to **Settings → Pages → Branch: main → Save**
6. Wait ~2 minutes → visit `https://yourusername.github.io/portfolio-editor`

Your editor and portfolio are now live, shareable, and free forever.

---

## ⚡ Alternative: Netlify (fastest option — 60 seconds)

1. Go to [netlify.com](https://netlify.com) — no account needed
2. Drag your downloaded `index.html` onto the homepage drop zone
3. Done — you get a live URL instantly

---

## 🧩 Tech stack

### Editor (`index.html`)
- Pure HTML + CSS + vanilla JavaScript — no frameworks
- `FileReader` API for image upload → base64 encoding
- `localStorage` for save/restore
- `Blob` + `URL.createObjectURL` for download

### Generated Portfolio
| Technology | Purpose |
|---|---|
| [Tailwind CSS v3](https://tailwindcss.com) via CDN | All styling, dark mode, responsive layout |
| [Alpine.js v3.14](https://alpinejs.dev) via CDN | Reactivity — dark mode, modals, project filter, tilt, mobile menu |
| [Google Fonts](https://fonts.google.com) | Playfair Display (headings) + DM Sans (body) |
| `IntersectionObserver` | Scroll-triggered reveal animations and skill bar fills |
| Vanilla JS | Typing animation, scroll progress bar |
| [Formspree](https://formspree.io) | Contact form — free tier, no backend |

---

## 🔧 Customizing after download

The downloaded `index.html` is standalone and self-contained. If you want to tweak anything after downloading:

| What | How |
|---|---|
| **Accent color** | Find & replace your chosen hex (e.g. `#E11D48`) with any new color |
| **CV file** | Put your PDF in the same folder as `index.html`, then find `cv.pdf` and replace with your filename |
| **Formspree form** | Replace `YOUR_FORM_ID` with your ID from [formspree.io](https://formspree.io) |
| **Default dark/light mode** | Find `darkMode:'class'` in the Tailwind config — the `<html class="dark">` attribute controls the default |
| **Add more sections** | The HTML is clean and well-structured — add new `<section>` blocks following the existing pattern |

---

## 🤝 Contributing

Found a bug or want to add something? PRs are welcome.

1. Fork this repo
2. Edit `index.html` directly
3. Test by opening the file in a browser
4. Submit a pull request with a clear description of what changed and why

### Ideas for future contributions
- [ ] Testimonials editor tab
- [ ] JSON import/export for sharing editor state
- [ ] Mobile/desktop preview toggle
- [ ] More font choices
- [ ] CV PDF upload (embed and link in navbar)
- [ ] Multiple color scheme presets (not just accent color)

---

## 📄 License

MIT — free to use, fork, modify, and distribute for any purpose, including commercially.

---

## 🙏 Acknowledgements

Built on the shoulders of great open-source work — Tailwind CSS, Alpine.js, Google Fonts, and Formspree. Thanks to all their contributors.

---

<div align="center">
  <br/>
  <strong>Built for everyone who deserves a great portfolio but shouldn't need to learn to code to have one.</strong>
  <br/><br/>
  <a href="https://yourusername.github.io/portfolio-editor"><strong>Try it live →</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/yourusername/portfolio-editor/issues">Report a bug</a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/yourusername/portfolio-editor/pulls">Contribute</a>
  <br/><br/>
</div>
