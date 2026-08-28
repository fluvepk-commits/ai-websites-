# Photos

`index.html` looks for these files by exact name. Drop them in and the page
picks them up — no code changes needed.

## Our Story (About section)

| File | Slot | Best shape |
|------|------|-----------|
| `salon-interior.jpg` | Main image | portrait, ~1200px wide |
| `styling-curls.jpg`  | Small offset image | portrait, ~800px wide |

## Our Work (Gallery)

| File | Tile | Category |
|------|------|----------|
| `bridal-glam.jpg`       | Large tall tile | Bridal |
| `blow-dry.jpg`          | Standard | Hair |
| `nail-art.jpg`          | Standard | Nails |
| `bridal-rose.jpg`       | Standard | Makeup |
| `scalp-ritual.jpg`      | Standard | Hair |
| `bridal-emerald.jpg`    | Standard | Makeup |
| `bridal-reception.jpg`  | Standard | Bridal |

## Hero

| File | Slot |
|------|------|
| `../video/hero.mp4`     | Hero background clip (muted, looping) |
| `hero-poster.jpg`       | Still shown until the clip's first frame is ready |

A portrait (9:16) clip sits in a right-hand panel on desktop and goes
full-bleed on narrower screens. Swapping in a landscape clip? Widen
`.hero-video` to `width:100%` and drop the mask.

All gallery photos want a portrait or square crop, ~900–1200px wide.

All the files above are in place and every gallery tile now carries a real
photo.

## Export settings

JPEG, quality 75–80, each file under ~300 KB keeps the page fast.

Every slot is `object-fit: cover`, so the photo is centre-cropped to the
tile — keep the subject near the middle. Where a subject sits high in the
frame, the `<img>` carries an inline `object-position` to pull the crop up;
adjust that percentage if a replacement photo frames differently. Crop out phone status bars and
screen-recording chrome before saving; the tile will not hide them.

Any file that is missing falls back to the blush gradient placeholder, so
the page never shows a broken image.

## Adding another gallery tile

Copy any existing `<figure class="tile ...">` block, point its `<img>` at the
new file, and set `data-cat` to one of: hair, bridal, makeup, nails. Adding a
new category also needs a matching `<button class="filter">` in the filter
row — a filter with no tiles behind it shows an empty grid.
