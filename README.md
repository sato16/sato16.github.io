# Fumiaki Sato Academic Website

Jekyll / Minimal Mistakes site source for a bilingual academic homepage.

## Structure

- `_pages/`: fixed pages for English and Japanese content.
- `_posts/`: language-tagged update posts.
- `_includes/`: local overrides and shared Liquid fragments.
- `_layouts/`: local layout overrides.
- `_sass/custom.scss`: site-specific CSS.
- `_data/`: publication, presentation, and navigation data safe for public builds.
- `assets/`: public images and stylesheets.
- `scripts/`: private helper scripts, excluded from generated sites.
- `private_data/`: raw or local-only material, excluded from generated sites and public copies.

## Build

```bash
bundle exec jekyll build --destination ../test/private_site
```

For public repository preparation, copy only the public-safe site files and exclude `private_data/`, `scripts/`, raw JSONL files, generated caches, and Git history.
