# Fintech Guild

Website for [fintechguild.com](https://fintechguild.com) — a private community of product and strategy experts in the Fintech and DeFi space.

## Pages

| File | URL |
|------|-----|
| `index.html` | `/` — Home |
| `events.html` | `/events` — Past and upcoming events |
| `book-club.html` | `/book-club` — Monthly reading group |

## Stack

Static HTML/CSS. No build step, no dependencies.

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

1. Edit the relevant HTML file and `styles.css`
2. Create a branch and open a PR against `main`
3. GitHub Pages deploys automatically on merge to `main`

## Contact

[info@fintechguild.com](mailto:info@fintechguild.com)
