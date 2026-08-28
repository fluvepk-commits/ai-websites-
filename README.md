# Bloom & Blush Salon — website

A single-page salon website: `index.html` holds the markup, styles and
scripts in one file, with no external requests, so it runs by opening it in
a browser and deploys by copying it to any host.

## Files

| Path | What it is |
|------|-----------|
| `index.html` | The entire site — HTML, CSS and JS |
| `images/` | Photos the page loads (see `images/README.md`) |

## Sections

Sticky header · hero · services · about with stat counters · filterable
gallery · pricing · testimonial carousel · location and contact · footer.

## Adding photos

The page has nine photo slots. Each one loads a file from `images/`; any
file that is missing falls back to a blush gradient placeholder, so the
page never shows a broken image. `images/README.md` lists the exact
filenames and the tile each one fills.

## Rebranding

Client-specific spots are marked with `[SWAP]` comments in `index.html`:
colours and fonts (the `:root` variables), logo, photos, copy, and contact
details.
