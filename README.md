# hugo-theme-personal

Personal overlay theme for [pietrbr.github.io](https://pietrbr.github.io).
Designed to be stacked on top of [PaperMod](https://github.com/adityatelange/hugo-PaperMod):

```yaml
theme: ["personal", "PaperMod"]
```

Hugo resolves templates and assets in theme order, so this repo carries only
the files that differ from stock PaperMod (partials, CSS, citation meta tags).
Files with the same path as a PaperMod file override it entirely.

## Override inventory

Rebased onto current PaperMod (carry only the listed change):

- `_partials/author.html` — thin-space author delimiter
- `_partials/edit_post.html`, `_partials/post_canonical.html` — middot separator
- `layouts/single.html` — no description block under the title
- `layouts/taxonomy.html` — no page header on the tags page
- `layouts/baseof.html` — headerless hero page with floating theme toggle

Fully custom (no upstream counterpart): `theme_init`, `hero_toggle`,
`extend_head` (Scholar citation tags), `math`, `analytics`, `render-link`,
`404`, `assets/css/extended/refresh.css`.

Still old-generation full copies, pending rebase: `head.html`,
`header.html`, `footer.html`, `list.html`, `svg.html` (custom icons), and
the `assets/css/{core,common}` files (the design system).
