# West Valley Fastpitch — Brand Guide Website

The official digital home of the **West Valley Fastpitch** visual identity — a
polished, responsive one-page brand site that serves as the source of truth for
the league's logos, colors, typography, photography, voice, and downloadable
assets.

> 1974 roots. West Valley heart. Built for today's players.

It is the digital extension of the **WVFP Rebrand Guide**, built for board
members, coaches, vendors, printers, sponsors, and partners who need approved
brand assets.

## Sections

- **Hero** — the league at a glance
- **Foundation** — brand pillars (unify, claim the legacy, raise the standard)
- **Logo** — primary circle badge, secondary marks, usage rules
- **Color** — the seven official colors with click-to-copy hex values
- **Type** — the three-job system (Roboto Slab · EB Garamond · Lato)
- **Photography** — documentary direction and style
- **Voice** — tone and approved core phrases
- **Applications** — where the brand shows up
- **Assets** — downloadable logos, color values, fonts, and templates

## Running locally

It's a static site — no build step. Open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Structure

```
index.html                     # all page content
assets/
  css/styles.css               # design system + layout
  js/main.js                   # nav, scrollspy, copy-to-clipboard, reveals
  img/logos/                   # web-optimized transparent PNG marks
  img/photos/                  # documentary + application photography
  img/favicon-*.png, og-image.jpg
  downloads/                   # full-resolution logo files for download
```

## Brand tokens

| Color          | Hex       | Role                 |
| -------------- | --------- | -------------------- |
| Softball Gold  | `#F3C12C` | Accent               |
| Primary Red    | `#B61816` | Primary signal       |
| Deep Red       | `#821415` | Secondary accent     |
| Primary Cream  | `#FFF7E8` | Default background    |
| Heritage Cream | `#E3D2AE` | Warm/nostalgic bg     |
| Dark Brown     | `#4A3426` | Secondary accent/text |
| Dusty Teal     | `#2E6B6A` | Secondary accent     |

**Type:** Roboto Slab (display) · EB Garamond (editorial) · Lato (utility),
all loaded from Google Fonts.

## Adding the official production files

The logo images shipped here are the marks from the rebrand guide, exported as
high-resolution transparent PNGs. Before wide rollout, drop the true vector
masters and export variants into `assets/downloads/` and wire the buttons in the
**Assets** section:

- [ ] Vector masters: `AI`, `SVG`, `EPS`, `PDF`
- [ ] Logo variants: full-color, one-color, reversed, black, white
- [ ] Confirm exact hex / CMYK / Pantone from the vector source
- [ ] Template files: field banner, social graphics, flyer, sponsorship packet
- [ ] Link the shared photo library for coaches and media

Placeholders and notes are already marked in the UI so nothing ships as a fake
final asset.
