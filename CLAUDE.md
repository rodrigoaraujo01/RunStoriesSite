# RunStories Website

Marketing website for **Run Stories**, an iOS app that lets runners create beautiful Instagram Stories by overlaying workout data (routes, pace charts, splits, stats) onto their own photos.

**Live at:** https://runstories.app
**Hosting:** GitHub Pages
**Domain:** runstories.app (custom domain, configure via CNAME file)

## Tech Stack

- **Static site** — plain HTML, CSS, JS. No frameworks, no build step. Keep it simple.
- GitHub Pages compatible (no server-side rendering, no Node required)
- Must include a `CNAME` file containing `runstories.app`

## Pages

### Landing Page (`index.html`)
Single-page marketing site. Sections:

1. **Hero** — App name, tagline "Share Images from your Runs", App Store download button, hero screenshot/mockup
2. **Features** — Key selling points with visuals:
   - Create stunning Instagram Stories from your runs
   - Overlay route maps, pace charts, splits & stats on your photos
   - Works with Apple Health & Strava — no account required to start
   - Beautiful templates to get started in seconds
   - Full creative control: drag, resize, rotate any element
   - Export to Instagram Stories, Photos, or share anywhere
3. **How It Works** — 3-step flow: Pick a workout → Choose a photo → Customize & share
4. **Pricing** — Free (5 exports) / Pro ($1.99/mo or $9.99/yr, unlimited exports + all templates)
5. **Footer** — Links to privacy policy, support email, App Store badge

### Privacy Policy (`privacy-policy/index.html`)
The app references `https://runstories.app/privacy-policy`. Key points to cover:
- Health data (HealthKit) never leaves the device
- Strava data cached locally, never sent to third-party servers
- No analytics on health data
- Photos accessed only for background selection
- Subscription managed via Apple App Store

### Support (`support/index.html`)
Simple support/FAQ page with contact email.

## Design Direction

- **Dark-first** aesthetic (the app is dark-mode-first — runners share evening/early morning runs)
- Clean, modern, slightly editorial (Nike Run Club + VSCO vibes)
- Gradient accent: orange to pink (`#DC862F` → `#FF3770`)
- Blue accent: `#0088FF`
- Mobile-responsive (most visitors will come from Instagram/social)
- Smooth scroll animations, minimal and tasteful
- High contrast text for readability

## App Metadata

- **App Name:** Run Stories
- **Bundle ID:** com.rapptor.runstories
- **App Store Subtitle:** "Route & Stats on Your Photos"
- **Developer:** Rapptor (Rodrigo)
- **Category:** Health & Fitness
- **Pricing:** Free with In-App Purchases (Pro: $1.99/mo or $9.99/yr)
- **Supported Languages:** English, Portuguese (Brazil)

## App Store Link

Use placeholder `https://apps.apple.com/app/run-stories/idXXXXXXXXXX` — will be replaced with real ID once published. Use standard Apple App Store badge for the download button.

## Assets

- App icon files are in the sibling project at `../RunStories/RunStories/runstories.icon/Assets/`
- You'll need to create or source:
  - App Store badge (use official Apple "Download on the App Store" SVG)
  - Screenshot mockups (use placeholder frames for now)
  - Feature illustration icons

## SEO

- Title: "Run Stories — Share Images from your Runs"
- Meta description: "Create beautiful Instagram Stories from your running data. Overlay route maps, pace charts, splits & stats on your photos. Works with Apple Health & Strava."
- Keywords: run, running, strava, instagram stories, workout, route map, pace chart, fitness, gps, share run
- Open Graph and Twitter Card meta tags
- Structured data (SoftwareApplication schema)

## Important Notes

- The site must work perfectly as a GitHub Pages deployment (static files only)
- All paths must work with GitHub Pages routing (use relative paths or proper base URL)
- Include `CNAME` file with `runstories.app` in the repo root
- Ensure privacy-policy page is accessible at `/privacy-policy` (use directory with index.html)
- Keep total page weight light — aim for < 500KB initial load
- No cookies, no tracking scripts (consistent with the app's privacy stance)
