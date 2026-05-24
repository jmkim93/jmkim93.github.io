# Jungmin Kim Website

Personal website built with [Hugo](https://gohugo.io/) on top of the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme and deployed through GitHub Pages.

## Local development

```bash
hugo server
```

For a production build:

```bash
hugo
```

## Repo structure

- `config.yml`: site configuration, menu, homepage profile, and global theme params.
- `content/`: page content and publication entries.
- `layouts/`: site-specific Hugo template overrides only.
- `assets/css/extended/site.css`: all site-specific visual overrides layered on top of PaperMod.
- `static/`: files copied directly to the built site such as images, PDFs, and favicons.
- `themes/PaperMod/`: upstream theme source.

## Maintenance notes

- Prefer editing `assets/css/extended/site.css` for styling changes instead of copying PaperMod CSS files into `assets/css/common/`.
- Prefer the smallest possible Hugo override in `layouts/`. If an upstream PaperMod template already works, inherit it instead of copying it.
- Do not commit `public/`, `resources/`, or `.DS_Store` files.

## License

This repository is licensed under the [MIT License](LICENSE.md).
