# Fintech Guild

Website for [fintechguild.com](https://fintechguild.com) — a private community of product and strategy experts in the Fintech and DeFi space.

## Pages

| File | URL |
|------|-----|
| `index.html` | `/` — Home |
| `admission/index.html` | `/admission/` — Admission criteria |
| `events/index.html` | `/events/` — Past and upcoming events |
| `events/<slug>/index.html` | `/events/<slug>/` — Event detail pages |

Pages are structured as `<name>/index.html` so GitHub Pages serves clean URLs (`/events/`) without a `.html` extension. All internal links use root-relative paths (`/events/`, `/styles.css`, `/logo.png`), so pages work the same regardless of nesting depth.

The old flat paths (`events.html`, `admission.html`, `events/agentic-payments.html`, etc.) still exist as thin redirect stubs (`<meta http-equiv="refresh">` + `rel="canonical"`) so any old bookmarks or external links keep working — don't delete them.

## Stack

Static HTML/CSS. No build step, no dependencies. `.nojekyll` disables GitHub Pages' Jekyll processing so files are served as-is.

- **Fonts** — Cormorant Garamond (serif) + DM Mono (monospace) via Google Fonts
- **Analytics** — Google Analytics (gtag)
- **Hosting** — GitHub Pages (`CNAME` → `fintechguild.com`)
- **Events** — [Luma](https://lu.ma)

## Running locally

```bash
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080).

## Making changes

1. Edit the relevant HTML file and `styles.css`. New pages should follow the `<name>/index.html` pattern and use root-relative links (`/foo/`, not `foo.html` or `../foo.html`)
2. Create a branch and open a PR against `main`
3. GitHub Pages deploys automatically on merge to `main`

## Contact

[info@fintechguild.com](mailto:info@fintechguild.com)
