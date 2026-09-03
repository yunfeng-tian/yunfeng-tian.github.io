# LicenseDesktop Website

Bilingual marketing site for [LicenseDesktop — Offline License Management System](https://chengyoung.com): English at the site root and Simplified Chinese under `/zh/`, hosted on GitHub Pages.

> Static marketing site for [chengyoung.com](https://chengyoung.com) — English (root) + Simplified Chinese (`/zh/`). Deployed on GitHub Pages.

## Pages

| File | Purpose |
|---|---|
| `index.html` | Product intro, features, screenshots, SEO (JSON-LD structured data) |
| `pricing.html` | USD pricing (Basic $49 / Professional $99 / Enterprise $149, M12) with real Creem checkout links |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms of Service / software license terms |
| `changelog.html` | Release notes / update history (`[1.0.0]` first release) |
| `download.html` | Windows download (GitHub Releases; "coming soon" until first public release) |
| `faq.html` | Frequently asked questions |
| `contact.html` | Contact (email support) |
| `assets/site.css` | Shared styles (zero-dependency) |
| `assets/favicon.svg` | Site favicon |
| `CNAME` | Custom domain `chengyoung.com` |
| `robots.txt` / `sitemap.xml` | SEO |
| `404.html` | Not-found page |
| `zh/` | Simplified Chinese mirror — `index / pricing / download / privacy / terms / faq / contact / changelog` |

## Status

- Creem checkout links: **live** — the three plan buttons in `pricing.html` point to real product
  checkout URLs on `creem.io` (Basic / Professional / Enterprise).
- Download buttons: **coming soon** until the first public release (0.9/1.0). When releasing, point
  the two buttons to the real GitHub Releases URL and fill `resources/update.config.json`
  `manual_download_url` with the same download location.
- Product screenshots: **in place** (`main.png`, `licenses.png`, `purchase.png`).
- Chinese site: **live** at `/zh/` — all 7 pages in Simplified Chinese, with `hreflang` alternates and a language switcher (中文 / English) in the nav on every page.

## Deploy steps

1. Push all files in this directory to the **repo root** of `yunfeng-tian/yunfeng-tian.github.io` (the user-homepage repo).
2. Keep `CNAME` (= `chengyoung.com`) at the repo root so GitHub Pages serves the custom domain.
3. Repo → Settings → Pages: **Source** = Deploy from a branch (`main` / root); set **Custom domain** = `chengyoung.com` and enable **Enforce HTTPS**.
4. DNS: point `chengyoung.com` at the GitHub Pages Anycast IPs (`185.199.108.153` … `185.199.111.153`), then confirm the site resolves over HTTPS.
5. `chengyoung.com` is hosted on GitHub Pages.
