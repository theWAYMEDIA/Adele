# adeleduplessis.net

Personal site of Adele du Plessis — business card, photo album and posts.
Plain Hugo, no theme: four layouts and one stylesheet.

```bash
hugo server -D      # local preview
hugo --minify       # production build -> public/
```

Push to `main` deploys to GitHub Pages.

## Adding a post

Create a page bundle `content/posts/<slug>/index.md`, drop the photos beside it,
and list them in front matter:

```yaml
---
title: "Title"
date: 2026-10-26
cover: first-photo.jpg
gallery:
  - src: first-photo.jpg
    caption: "Optional caption"
---
Body text in Markdown.
```

Hugo resizes every photo to WebP thumbnails (480px) and lightbox images (1600px) at build time,
so upload originals as they are.

Content was migrated from the WordPress site on 2026-10-26; old URLs `/jean-and-i/` and `/home/` still resolve.
