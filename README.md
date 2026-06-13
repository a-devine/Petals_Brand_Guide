# Petals &amp; Purpose — Brand Guide

The living brand guide for **Petals &amp; Purpose**, a small floral studio in Waukesha, Wisconsin.
Handcrafted, one-of-a-kind arrangements — with a portion of every sale supporting grassroots charities.

**Live site:** https://a-devine.github.io/Petals_Brand_Guide/

This is a clean, self-contained static site. There is no build step and no framework — just
HTML, CSS, and a few lines of vanilla JavaScript. Fonts load from Google Fonts; every logo and
specimen lives as a real file in `brand/`.

## Structure

```
.
├── index.html          # the brand guide (single page, ~46 KB)
├── .nojekyll           # tells GitHub Pages to serve files as-is
└── brand/              # downloadable assets
    ├── logo-primary.svg / .png            # full stacked lockup (master)
    ├── logo-primary-transparent.svg       # same master, named for the download link
    ├── logo-reverse.svg / .png            # light-on-dark version (Linen Cream)
    ├── logo-icon.svg / .png               # flower mark only (avatar / favicon)
    ├── logo-horizontal.svg / .png         # horizontal lockup (mark + wordmark)
    ├── favicon.png                        # 128px flower mark
    ├── palette.svg / .png                 # six-tone color reference
    ├── typography.svg / .png              # Cinzel · Cormorant · Inter specimen
    └── brand-guide.pdf                    # printable two-page summary
```

## Brand at a glance

**Fonts** (all free via Google Fonts): Cinzel (display), Cormorant Garamond Italic (kicker /
pull quotes), Inter (body / UI).

**Palette**

| Role | Name | Hex |
|------|------|-----|
| Primary | Petal Pink | `#DBA5A8` |
| Canvas | Linen Cream | `#FCF8EC` |
| Depth | Mauve Rose | `#C68A8E` |
| Ink | Warm Charcoal | `#3A2A2A` |
| Natural accent | Stem Sage | `#B5C2A5` |
| Rare accent | Antique Gold | `#C9A96E` |

## Deploying

This repo is served by GitHub Pages from the `main` branch root.

1. Commit `index.html`, `.nojekyll`, and the `brand/` folder to the repo root.
2. In **Settings → Pages**, confirm the source is `main` / root.
3. Wait a minute or two for the build, then load the live URL.

To preview locally, run any static server from the repo root, e.g. `python3 -m http.server`,
then open `http://localhost:8000`.

## Notes

- The **horizontal lockup** was composed to the brand-guide spec (real flower mark + Cinzel
  wordmark + Cormorant descriptor). Swap `brand/logo-horizontal.*` if a different master exists.
- The logo mark is Petal Pink — do not recolor outside the palette. Minimum sizes and clear-space
  rules are in the guide (§ 01) and the PDF.
