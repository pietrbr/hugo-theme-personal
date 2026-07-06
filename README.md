# hugo-theme-personal

Personal overlay theme for [pietrbr.github.io](https://pietrbr.github.io).
Designed to be stacked on top of [PaperMod](https://github.com/adityatelange/hugo-PaperMod):

```yaml
theme: ["personal", "PaperMod"]
```

Hugo resolves templates and assets in theme order, so this repo carries only
the files that differ from stock PaperMod (partials, CSS, citation meta tags).
Files with the same path as a PaperMod file override it entirely.
