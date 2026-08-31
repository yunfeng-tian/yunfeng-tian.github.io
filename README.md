# LicenseDesktop Website

Minimal English marketing site for [LicenseDesktop — Offline License Management System](https://chengyoung.com), hosted on GitHub Pages.

> Status: minimal set for **Creem account review** (2026-08-31). Aligned with `docs/合规路径-1.0.md` + `docs/建站部署指南.md` + `docs/施工蓝图-50-建站与Creem过审.md`.

## Pages

| File | Purpose |
|---|---|
| `index.html` | Product intro, features, screenshots placeholder |
| `pricing.html` | USD pricing (Basic $49 / Professional $99 / Enterprise $149, M12) |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms of Service / software license terms |
| `download.html` | Windows download (links to GitHub Releases) |
| `assets/site.css` | Shared styles (zero-dependency) |
| `CNAME` | Custom domain `chengyoung.com` |
| `404.html` | Not-found page |

## Placeholders to replace before going live

- GitHub username resolved: `yunfeng-tian` — download links point to `yunfeng-tian/yunfeng-tian.github.io` releases.
- `https://checkout.creem.io/your-product` in `pricing.html` → real Creem checkout URL after review.
- `#screens` section in `index.html` → product screenshots.

## Deploy steps

See `../docs/建站部署指南.md` §3-§5 (GitHub Pages + DNS + email). Upload all files to the **repo root of `yunfeng-tian/yunfeng-tian.github.io`** (user homepage repo, already created). Keep the site on GitHub Pages (overseas) until the ICP filing is approved; keep the main domain on mainland servers after filing + show the ICP number in the footer.
