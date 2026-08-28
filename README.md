# Photos

`index.html` looks for these five files. Filenames must match exactly —
drop the images in and the page picks them up, no code changes needed.

| File | Used in | Best shape |
|------|---------|-----------|
| `salon-interior.jpg` | About / Our Story — main image | portrait or square, ~1200px wide |
| `styling-curls.jpg`  | About / Our Story — small offset image | portrait, ~800px wide |
| `bridal-glam.jpg`    | Gallery — large tall tile | portrait, ~1000px wide |
| `blow-dry.jpg`       | Gallery — standard tile | portrait or square, ~900px wide |
| `scalp-ritual.jpg`   | Gallery — standard tile | portrait or square, ~900px wide |

Every slot is `object-fit: cover`, so a photo is centre-cropped to the tile —
keep the subject near the middle. Export as JPEG around quality 75–80; each
file under ~300 KB keeps the page fast.

Any tile whose file is missing falls back to the blush gradient placeholder,
so the page never shows a broken image.

The remaining gallery tiles are still placeholders. To fill one, copy the
pattern from a tile that already has a photo: add an `<img>` as the first
child and add `has-photo` to the `<figure>` class list.
