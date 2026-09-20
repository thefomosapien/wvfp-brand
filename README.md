# West Valley Fast Pitch — Brand Guide Website

The official digital home of the **West Valley Fast Pitch** visual identity — a
polished, responsive one-page brand site that serves as the source of truth for
the league's logos, colors, typography, photography, voice, and downloadable
assets.

> 1974 roots. West Valley heart. Built for today's players.

It is the digital extension of the **WVFP Rebrand Guide**, built for board
members, coaches, vendors, printers, sponsors, and partners who need approved
brand assets.

## Naming (writing the league's name)

Keep prose consistent — the site's Voice section documents this in full:

- **West Valley Fast Pitch, Inc.** — legal name (contracts, filings, banking, insurance, tax).
- **West Valley Fast Pitch** — standard written name; use in all normal prose and copy, with "Fast Pitch" as **two words**.
- **WEST VALLEY FASTPITCH** / **FASTPITCH** — one-word branded display treatment only (logos, wordmarks, merch, signage, headlines). It never replaces the written name.
- **WVFP** — approved abbreviation once the league is identified or context is clear.

Avoid sentence-case "West Valley Fastpitch" in running text — it reads like an
alternate spelling rather than a purposeful brand treatment.

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
  img/logos/                   # web-optimized display PNGs used on the page
  img/photos/                  # documentary + application photography
  img/favicon.svg, favicon-*.png, og-image.png
  brand-logos/                 # the official, downloadable logo files
    primary-badge/             # circle badge — CORE (no date) + 1974 (dated)
    arched-wordmark/           # arched varsity wordmark
    pill-lockup/               # horizontal pill lockup
    wvfp-logo-pack.zip         # everything, zipped, for "download all"
```

### Logo file naming

There are four marks — **core** (circle badge, no date), **1974** (circle
badge with the date), **word** (arched wordmark), and **pill** (pill lockup).
Each comes in three color treatments (color / black / white) and five formats
(AI · EPS · JPG · PNG · SVG):

```
primary-badge/wvfp-core-color.{ai,eps,jpg,png,svg}    # no date, full color
primary-badge/wvfp-core-black.*                         # no date, one-color black
primary-badge/wvfp-core-white.*                         # no date, white / reversed
primary-badge/wvfp-1974-color.*  wvfp-1974-black.*  wvfp-1974-white.*   # dated
arched-wordmark/wvfp-word-color.*  -black.*  -white.*
pill-lockup/wvfp-pill-color.*  -black.*  -white.*
```

- **PNG** — everyday use, transparent (docs, slides, web, email)
- **SVG** — sharpest at any size (web, large signage)
- **JPG** — a flat image for tools that require one
- **AI / EPS** — editable source files for designers

Use **full-color** on light/cream backgrounds, **white** on red, brown, dark,
or photo backgrounds, and **black** wherever a single-color mark is needed.
(White PNGs are exported transparent from the master vector so they place
cleanly on any background.)

The raw export files the league provided were reviewed and consolidated into
the structure above: exact duplicates and non-useful exports (e.g. white logos
baked onto a solid black box) were removed, and everything else was renamed and
grouped by mark.

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

## Official logo files

The official logo files live in `assets/brand-logos/` and are wired into the
**Assets** section for download (per-mark, or the full `wvfp-logo-pack.zip`). To
add or update a mark, replace the matching files in its folder — keep the names
the same and the download buttons keep working.

Still nice to have later:

- [ ] Confirm exact hex / CMYK / Pantone from the vector source
- [ ] Template files: field banner, social graphics, flyer, sponsorship packet
- [ ] Link a shared photo library for coaches and media
