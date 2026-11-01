# Mug Media

**Brands, websites & bots, brewed fresh.**

Mug Media is an independent digital agency in India. This repository holds
its single-file static website — no build step, no backend, no database.

## What it does

- Fast, clear websites for small brands, creators and teams
- 11 services, each with a working demo on the page:
  Digital Marketing, Web Design, Social Media Management, Brand Management,
  AI Automations, QR to NFC, AI UGC Ads, Performance Ads,
  SEO + Google Business, Influencer Collaborations, WhatsApp Automation
- Live work, built by us:
  - [Rankaar 2026](https://rankaar-demo.vercel.app/) — Garba event site, Rotaract Club of Patan
  - [Mehak Mir](https://mehak-portfolio-tau.vercel.app/) — UGC creator portfolio
  - [Velaur Parfumes](https://atelier-veil-kappa.vercel.app/) — Designer-perfume shop site, Prayagraj

## Run it

Open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy it

Static only — deploy the repository root on Vercel, Netlify, or any static
host. No environment variables, no build command.

## Contact / Send a brief

The contact form on the page gives two options, both client-side:

1. **Send via Gmail** — opens Gmail compose to `support.mugmedia@gmail.com`
   with the brief filled in.
2. **Send via Instagram DM** — copies the brief, then opens the Mug Media
   Instagram profile so it can be pasted into a DM.

- Email: [support.mugmedia@gmail.com](mailto:support.mugmedia@gmail.com)
- Instagram: [@mugmedia.in](https://www.instagram.com/mugmedia.in?vrfl=YWw5NDl3MHhpNXRu&utm_source=qr)

Nothing from the form is stored on this page or in this repository.

## Structure

```
index.html            # the whole site, self-contained
                      # (logo + project screenshots are embedded in it)
README.md             # this file
```

Note: the logo and screenshots live inside `index.html` itself, so the
site works from that one file alone. Separate JPG copies are not in this
repo because the GitHub connector only pushes text files.

## Security notes

- No external scripts. Fonts load from Google Fonts only.
- No iframes, objects, or embeds.
- All external links use `rel="noopener noreferrer"`.
- A Content-Security-Policy meta tag blocks frames, objects and
  non-font external connections. Inline script/style is used for the
  on-page demos, so the policy allows `unsafe-inline` for those.
