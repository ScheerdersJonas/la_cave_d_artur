# La Cave d'Artur

**Live site:** https://ScheerdersJonas.github.io/la_cave_d_artur/

A Jekyll-based GitHub Pages site built for wine tasting events hosted by La Cave d'Artur.

## What it does

Guests scan a single QR code and land on a mobile-friendly page where they can browse the wines being served that evening, organized by category:

- **White Wines**
- **Red Wines**
- **Bubbles**

Each wine has its own detail page with producer, region, grape variety, and tasting notes.

## Structure

```
index.html              # Landing page — category overview
print-qr.html           # Printable QR code page
assets/qr-code.png      # Static QR code image (points to the landing page)
wines/
  white/                # White wine pages
  red/                  # Red wine pages
  bubbles/              # Sparkling wine pages
_layouts/               # Jekyll HTML layouts
assets/css/style.css    # Site styles
_config.yml             # Jekyll configuration
```

## Adding or editing a wine

Each wine is a Markdown file under `wines/<category>/`. Open the file, edit the front matter (producer, region, grape, year) and add tasting notes below the `---`. Push to `main` and GitHub Pages rebuilds automatically within a minute.

## QR code

The QR code is pre-generated as a static PNG at `assets/qr-code.png`. Print it directly or navigate to `/print-qr` on the live site for a print-optimized page.

