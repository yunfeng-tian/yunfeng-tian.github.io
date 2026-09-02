# LicenseDesktop Website

Bilingual marketing site for [LicenseDesktop — Offline License Management System](https://chengyoung.com): English at the site root and Simplified Chinese under `/zh/`, hosted on GitHub Pages.

> Status: minimal set for **Creem account review** (2026-08-31). Aligned with `docs/合规路径-1.0.md` + `docs/建站部署指南.md` + `docs/施工蓝图-50-建站与Creem过审.md`.

## Pages

| File | Purpose |
|---|---|
| `index.html` | Product intro, features, screenshots, SEO (JSON-LD structured data) |
| `pricing.html` | USD pricing (Basic $49 / Professional $99 / Enterprise $149, M12) with real Creem checkout links |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms of Service / software license terms |
| `download.html` | Windows download (GitHub Releases; "coming soon" until first public release) |
| `faq.html` | Frequently asked questions |
| `contact.html` | Contact (email support) |
| `assets/site.css` | Shared styles (zero-dependency) |
| `assets/favicon.svg` | Site favicon |
| `CNAME` | Custom domain `chengyoung.com` |
| `robots.txt` / `sitemap.xml` | SEO |
| `404.html` | Not-found page |
| `zh/` | Simplified Chinese mirror — `index / pricing / download / privacy / terms / faq / contact` |

## Status

- Creem checkout links: **live** — the three plan buttons in `pricing.html` point to real product
  checkout URLs on `creem.io` (Basic / Professional / Enterprise).
- Download buttons: **coming soon** until the first public release (0.9/1.0). When releasing, point
  the two buttons to the real GitHub Releases URL and fill `resources/update.config.json`
  `manual_download_url` with the same download location.
- Product screenshots: **in place** (`main.png`, `licenses.png`, `purchase.png`).
- Chinese site: **live** at `/zh/` — all 7 pages in Simplified Chinese, with `hreflang` alternates and a language switcher (中文 / English) in the nav on every page.

## Screenshots (how to take)

1. Run the app (LicenseDesktop), log in.
2. Use Windows screenshot: **Win + Shift + S** (or PrtScn) to capture the relevant window.
3. Save as PNG with the exact names above into `website/assets/img/screenshots/` and upload to the repo.
4. Suggested captures: main dashboard (workbench), license list / issue page, purchase / about page.

## Deploy steps

See `../docs/建站部署指南.md` §3-§5 (GitHub Pages + DNS + email). Upload all files to the **repo root of `yunfeng-tian/yunfeng-tian.github.io`** (user homepage repo, already created). `chengyoung.com` stays on GitHub Pages (overseas) with **no ICP filing**; if the project is later incorporated, a separate `chengyoung.cn` site would be created independently (see `../docs/官网优化方案-v1.1.md`).
