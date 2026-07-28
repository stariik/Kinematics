<div align="center">

# KINEMATICS AGENCY

### `[ WE CREATE UNSKIPPABLE ]`

**A cinematic, motion-driven marketing site for a video production & branding studio.**

Premium video. Optimized budgets. End-to-end control.

[Home](./index.html) · [Portfolio](./portfolio.html) · [About](./aboutus.html)

---

</div>

## About

**Kinematics Agency** is the official website for a full-service production and branding studio that helps mid-sized businesses tell their stories through cinematic video, strong visual identity, and performance marketing.

The site is a fully hand-crafted, multi-page static web experience. It opens with an autoplaying background reel, introduces the studio's services, presents a curated portfolio of work, and closes with a dynamic, animated contact section. Every page is wired with scroll-triggered motion to reinforce the "we make things move" brand promise.

## What the Site Does

- **Hero Reel** — a silent, looping background video greets the visitor, overlaid with stretching typography that scales as the user scrolls.
- **Services Grid** — a six-card overview of the agency's offering (Brand Films, Ad Campaigns, End-to-End Production, Visual Branding, Performance Marketing, Business Intelligence Reporting).
- **Portfolio Page** — a curated case-study gallery of the studio's highest-impact work.
- **About Page** — the studio's philosophy, methodology, and the "Kinetic Shock Process".
- **Dynamic Contact Section** — an animated tagline cycles through words like *MOTION*, *EMOTIONAL DEPTH*, *CINEMATIC IDENTITY* while a Netlify-powered contact form handles inbound leads.
- **Off-Canvas Navigation** — a single menu system that behaves as click-to-toggle on mobile and hover-to-reveal on desktop.

## Techniques Used

### Front-End Stack
- **HTML5** — semantic structure across three pages (`index.html`, `portfolio.html`, `aboutus.html`).
- **CSS3** — three dedicated stylesheets (`style.css`, `portf.css`, `aboutss.css`), each scoped to a page. Uses Flexbox, CSS Grid, custom properties, media queries, and keyframe transitions.
- **Vanilla JavaScript** — no framework, no build step. One hand-written script per page (`script.js`, `portoofo.js`, `aboutsss.js`).
- **AOS (Animate On Scroll)** — scroll-triggered entrance animations (`fade-up`, staggered delays) applied declaratively via `data-aos` attributes.

### Motion & Interaction
- **Scroll-Driven Typography Stretch** — the hero headline `UNSKIPPABLE` scales vertically in response to scroll position, with a separate amplification factor for mobile viewports.
- **Scroll-Hide Header** — the top navigation slides away on scroll-down and returns on scroll-up, guarded against flicker while the menu is open.
- **Width-Stable Dynamic Text** — the cycling tagline pre-measures the widest term so the surrounding layout doesn't reflow on every swap.
- **Off-Canvas Menu with Dimmer** — click, hover, link-tap, and dimmer-click all close the menu through a single pair of `openMenu` / `closeMenu` handlers.
- **Autoplaying Muted Background Video** — `autoplay muted loop playsinline` for cross-browser (including iOS Safari) inline playback.

### Performance & UX
- **Passive scroll listeners** so animation work never blocks the scroll thread.
- **Responsive design** — mobile-first media queries, touch-safe interactions, and a dedicated mobile stretch factor.
- **Favicon + PWA manifest** — full icon set (`favicon.ico`, `favicon.svg`, `apple-touch-icon`, 192/512 app icons, `site.webmanifest`).
- **Netlify Forms** — contact form wired with `data-netlify="true"` and a honeypot field for spam protection.
- **Custom fonts** served locally from `/fonts` to preserve brand typography without extra network calls.

## Project Structure

```
Kinematics/
├── index.html            # Home — hero, services, about teaser, contact
├── portfolio.html        # Curated case-study gallery
├── aboutus.html          # Studio philosophy & methodology
│
├── style.css             # Styles for index.html
├── portf.css             # Styles for portfolio.html
├── aboutss.css           # Styles for aboutus.html
│
├── script.js             # Interactions for index.html
├── portoofo.js           # Interactions for portfolio.html
├── aboutsss.js           # Interactions for aboutus.html
│
├── logo/                 # Agency logo assets
├── photos/               # Imagery used across the site
├── videos/               # Hero reel & portfolio video assets
├── fonts/                # Self-hosted brand typefaces
│
├── favicon.ico           # Favicon + PWA icon set
├── favicon.svg
├── favicon-96x96.png
├── apple-touch-icon.png
├── web-app-manifest-192x192.png
└── web-app-manifest-512x512.png
```

## Running Locally

No build tools, no dependencies to install — it's static.

```bash
# clone
git clone https://github.com/stariik/Kinematics.git
cd Kinematics

# serve (pick one)
python -m http.server 8080
# or
npx serve .
```

Then open http://localhost:8080 in your browser.

> Opening `index.html` directly via `file://` also works, but a local server is recommended so relative paths (video, manifest, icons) resolve correctly.

## Deployment

The site is designed to drop straight onto **Netlify** — the contact form's `data-netlify` attribute is picked up automatically on deploy, no backend required. It will also deploy unchanged to GitHub Pages, Vercel, Cloudflare Pages, or any static host.

## Contact

- **Email** — info@kinematics.ge
- **Phone** — +995 551 22 03 44

<div align="center">

---

`© 2025 KINEMATICS AGENCY · ALL RIGHTS RESERVED`

</div>
