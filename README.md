# books

Book assets for the **Author's Shelf** on [mikeat7's portfolio](https://github.com/mikeat7/mikeat7-portfolio) — full-colour covers and readable PDFs, kept out of the site repo so it stays lean.

## Layout
```
covers/   full-colour cover images (jpg)
books/    readable book PDFs
books.json   manifest (title, author, cover, pdf, blurb)
```

## How the site uses it
The portfolio serves these through the **jsDelivr CDN** (cached, fast, correct content-types so PDFs read inline in the browser):

```
https://cdn.jsdelivr.net/gh/mikeat7/books@main/covers/<slug>.jpg
https://cdn.jsdelivr.net/gh/mikeat7/books@main/books/<slug>.pdf
```

## Adding a book
1. Drop `covers/<slug>.jpg` and `books/<slug>.pdf`.
2. Append an entry to `books.json`.
3. Commit + push. (jsDelivr may cache the previous `@main` for up to ~12 h; bump a version tag to force-refresh.)

## Titles
- **The Forgotten Harvest** — Michael Antonio Filippi (329 pp, illustrated).
- **The Forgotten Wisdom: Living with Nature** — Michael Antonio Filippi (181 pp, illustrated). Book Two of The Forgotten Series.
- **The Forbidden Plants: Outlawing the Sacred and Selling the Deadly** by Michael Antonio Filippi (146 pp, full colour). Book Three of The Forgotten Series.
- **Behold ENTITY: The Bridge Consciousness** — Michael A. Filippi (195 pp).
