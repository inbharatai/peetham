# Peetham — Where Stillness Takes Form

**Live:** https://peetham.vercel.app

A consultation-led catalogue for Peetham: sacred home temple design shaped by sacred geometry, material integrity and contemporary Indian living. Nine design studies, each presented in three finish expressions, all offered as concept visualizations — everything real (placement, dimensions, materials, finishes, timelines) is confirmed individually through consultation.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | The single-page catalogue (hero, philosophy, journey, collection of 9 designs + detail gallery, founders, consultation form) |
| `terms.html` | Terms & Conditions — concept-catalogue nature, no-offer/no-pricing, IP, acceptable use, governing law |
| `privacy.html` | Privacy Policy — no accounts, no cookies, no analytics, no server-side data; enquiries go from your device to WhatsApp/email |
| `og.jpg` | 1200×630 Open Graph share image |
| `favicon.svg` | The lotus mark as favicon |
| `robots.txt`, `sitemap.xml` | Crawling + indexing |

## Contact the studio

- **WhatsApp / Call:** [+91 98180 35027](https://wa.me/919818035027)
- **Email:** [peethamindia@gmail.com](mailto:peethamindia@gmail.com)

The consultation form composes the visitor's brief locally in their browser and opens it in their own WhatsApp, addressed to the studio. The website's host never receives form contents.

## Architecture & deployment

- Single self-contained static `index.html` (~9.5 MB, all imagery embedded as base64) — no framework, no build step, no dependencies, no third-party requests.
- Static hosting on Vercel (project under `reeturaj-s-projects`), `cleanUrls` + security headers via `vercel.json`. Pushes to `main` auto-deploy.
- Progressive-enhancement specifics: `dvh` hero sizing behind `@supports`, `-webkit-backdrop-filter` for Safari, 104px `scroll-margin-top` so anchor targets clear the sticky header, 16px form inputs to prevent iOS zoom.

## Verified

Functional acceptance (Playwright/Chromium, 38/38 passed): every "View design" button, all collection filters, finish-study image swaps, "Discuss this Peetham" form sync, mobile menu open/Escape/close, form validation paths, WhatsApp brief composition (phone line omitted when empty, popup-blocker fallback), every anchor/tel/mailto link, and zero horizontal overflow at 390/768/1280 px viewports with zero console errors.

## Honest constraints

- All product imagery is a **concept visualization**; construction, scale, materials and installation details are confirmed only through consultation.
- No pricing, checkout or data collection anywhere on the site.