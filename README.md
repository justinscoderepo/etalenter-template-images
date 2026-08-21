# eTalenter template images

AI-generated imagery for the eTalenter event category templates, served over GitHub Pages.

| Folder | Count | What it is |
|---|---|---|
| `categories/` | 12 | One landscape image per template category |
| `groups/` | 10 | One per age band, shared across all templates |
| `items/` | 509 | One per competition item, shared where items mean the same thing |

All images are 1200px-wide WebP, flat vector illustration on white.

Item images are keyed by *meaning*, not by title: the six language variants of Prasangam all
resolve to `items/elocution.webp`, because they are one photograph of someone giving a speech.
Age groups collapse the 189 distinct group names down to ten real bands.

Referenced from `etaletnerStaticDb` as the `ImageUrl` on each category, age group, competition
item and competition row.

## `_old` files

Each image has a `<key>_old.webp` alongside it holding the earlier photographic version, kept for
reference. Nothing reads them today; the URL is derivable if a future page wants photographs:

```js
const photoUrl = item.ImageUrl.replace('.webp', '_old.webp');
```
