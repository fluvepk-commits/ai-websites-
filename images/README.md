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

All gallery photos want a portrait or square crop, ~900–1200px wide.

## Export settings

JPEG, quality 75–80, each file under ~300 KB keeps the page fast.

Every slot is `object-fit: cover`, so the photo is centre-cropped to the
tile — keep the subject near the middle. Crop out phone status bars and
screen-recording chrome before saving; the tile will not hide them.

Any file that is missing falls back to the blush gradient placeholder, so
the page never shows a broken image.

## Filling the four remaining placeholder tiles

Copy the pattern from a tile that already has a photo: add an `<img>` as the
first child of the `<figure>` and add `has-photo` to its class list.
