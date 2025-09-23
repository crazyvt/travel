# Travel Blog (Hugo)

A minimal Hugo site with hierarchical destinations:

- India → Kerala → Wayanad
- India → Kerala → Trivandrum
- India → Karnataka → Gokarna
- India → Kashmir → Srinagar

## Prerequisites
- Hugo Extended (recommended)
  - macOS: `brew install hugo`
  - Windows: `choco install hugo-extended`
  - Linux: use your package manager or download from releases

Verify install:
```bash
hugo version
```

## Get the code
- Zip: Share the `travel-blog` folder.
- Git: Initialize and push to a repo if desired.

## Run locally
```bash
cd travel-blog
hugo server --minify --navigateToChanged --buildDrafts
```
Open `http://localhost:1313`.

## Build for sharing/hosting
```bash
hugo --minify
```
Static files land in `public/`. Share or deploy that folder to any static host.

## Structure
- Content: `content/posts/india/...` with state `_index.md` and destination `index.md` files
- Templates: `layouts/_default/list.html` and `layouts/_default/single.html`
- Styles: `static/css/styles.css`
- Config: `hugo.toml`

## Adding more destinations
1. Create a state folder if needed, with `_index.md`.
2. Create a destination folder with `index.md` using front matter fields:
   - `title`, `location`, `description`, `tags`, optional `image`

## Notes
- No external theme; tiny footprint (<50 files, <10MB).
- Works on macOS, Windows, and Linux.
