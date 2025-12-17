# NanoBot Showcase Website (Static Landing Page)

A single-page, dark, futuristic landing site to showcase **NanoBot** – a tiny, friendly AI assistant that is **completely free**.  
Built with plain **HTML**, **CSS**, and a little **JavaScript** (no frameworks).

## Files

- `index.html` – Main single-page layout with:
  - Sticky header + navigation
  - Hero section
  - About section
  - Features (what NanoBot does)
  - How it works
  - Friendly & safe highlight strip
  - FAQ
  - Contact / call to action
  - Footer
- `styles.css` – Dark futuristic theme, layout, and responsive design.
- `main.js` – Small enhancements:
  - Smooth scrolling for in-page navigation links
  - Reveal-on-scroll animation for sections/cards
  - Dynamic current year in the footer

## How to run locally

1. Make sure all three files are in the same folder.
2. Open `index.html` directly in your browser:
   - On Windows: right-click `index.html` → **Open with** → your browser, or
   - Drag `index.html` into a browser window.

No build step or dependencies are required.

## Customizing the content

Open `index.html` in a code editor and adjust:

- **Hero section**  
  Search for the `<section id="hero">` block and update:
  - Main heading (`Meet NanoBot – your tiny AI that does big things.`)
  - Subtitle text
  - Button labels (e.g. “Start with NanoBot”, “See what it can do”)

- **About section**  
  In `<section id="about">`, edit the paragraphs/cards to reflect:
  - Who you are
  - Your mission
  - How you think about friendly / free AI

- **Features section**  
  In `<section id="features">`, there are multiple `.feature-card` blocks.  
  Update titles and descriptions to match what your nano-bot actually does
  (e.g. WhatsApp automation, FAQs, lead capture, etc.).

- **How it works**  
  In `<section id="how-it-works">`, you can rename the three steps or tweak
  the descriptions to better describe your real flow.

- **FAQ**  
  In `<section id="faq">`, each question is a `<details>` with a `<summary>`.  
  Replace the questions/answers with ones your users are likely to have.

- **Contact section**  
  In `<section id="contact">`, update:
  - The `mailto:` link with your real email
  - The WhatsApp link placeholder with your actual bot or chat URL
  - The main CTA button `href="#"` to point to your landing page / bot link

## Customizing the look

Most key colors and radii live at the top of `styles.css` in the `:root` block:

```css
:root {
  --bg-main: #040615;
  --accent: #3cf2ff;
  --accent-strong: #6f7dff;
  --text-main: #f6f7ff;
  --text-muted: #9ca4d2;
  --radius-lg: 18px;
  --radius-pill: 999px;
}
```

- Change `--accent` / `--accent-strong` for different neon colors.
- Adjust `--bg-main` / `--bg-alt` if you want a different dark base.
- Font families are defined on `body` and in headings (`Space Grotesk` + `Inter` via Google Fonts).

## Deploying the site

Because this is a static site, you can host it almost anywhere:

- **GitHub Pages**
  - Create a repository, commit `index.html`, `styles.css`, and `main.js`.
  - Enable GitHub Pages for the repo (from the `Settings` → `Pages`).
  - Your site will be available at a GitHub Pages URL you can share.

- **Netlify / Vercel**
  - Create a new project and point it at your repo, or drag-and-drop the folder.
  - No build step is needed; just serve `index.html` as-is.

- **Any static hosting**
  - Upload the three files to a web server (or your existing site’s public folder).

Once deployed, point your WhatsApp bot or any “Try NanoBot” link to this
landing page so people can see what it is and what it does.


