# StackMindrApp

Marketing + legal site for **StackMindr** — https://stackmindr.app

Static site, no build step. Served by GitHub Pages from this repo root.

```
index.html            landing page
privacy.html          privacy policy (linked from both app stores)
delete-account.html   account deletion instructions (required by Google Play)
apple-touch-icon.png  180x180 home-screen icon
og-image.png          1200x630 social share card
CNAME                 stackmindr.app
images/               screenshots referenced by index.html
```

## Updating screenshots

Drop a PNG into `images/` using the filename below. `index.html` picks it up on
next load — no code change needed.

| File | Screen |
|---|---|
| `today.png` | Today's stack (also the hero phone) |
| `schedule.png` | My schedule |
| `cycle-planner.png` | Calc → Cycle planner |
| `stock.png` | My pantry |
| `glossary.png` | Glossary |
| `labs.png` | Settings → Lab Work |
| `ai.png` | Stack advisor |
| `calc-recon.png` | Calc → Peptide Reconstitution |
| `injection-site.png` | Injection site rotation modal |

All screenshots are 620px wide, resized from 1290x2796 iPhone captures with
LANCZOS and saved optimized. Keep the whole set on one app version so the
carousel doesn't mix designs.

## Deploy

```
git add -A && git commit -m "Site refresh for v1.3.0" && git push
```

GitHub Pages redeploys in about a minute.
