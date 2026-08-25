# Roca Tax Website

Roca Tax has permanently closed. This repository now serves a single static
closure notice at [roca.tax](https://roca.tax/), in English and Spanish.

All service, about, contact, and blog pages have been removed, along with every
scheduling link, email address, and phone number.

## Structure

```
roca-tax-website/
├── content/
│   ├── _index.md           # Closure notice (English)
│   └── es/_index.md        # Closure notice (Spanish)
├── themes/roca-tax-theme/  # Minimal theme: index, 404, base layout, CSS
├── config.toml             # Hugo configuration
└── public/                 # Build output
```

## Building

Requires [Hugo](https://gohugo.io/).

```bash
hugo server      # preview at http://localhost:1313
hugo --minify    # build into public/
```

## Notes

- `noindex` is set site-wide, and sitemap/RSS output is disabled, so search
  engines drop the old pages.
- The 404 template shows the same closure notice in both languages, so inbound
  links to removed pages (`/en/contact/`, `/es/services/`, blog posts, etc.)
  land on the message rather than a broken page.
