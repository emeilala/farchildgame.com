# farchildgame.com

The devlog site for FarChild. GitHub Pages builds it automatically with Jekyll every time a file changes here.

**This repository is public.** Everyone can read every file in it, including old versions. Don't put drafts, notes or anything secret here.

## Changing the season

- Site-wide (landing page, letters list): edit `season:` in `_config.yml`.
- One letter: set `season:` at the top of that letter's file.

The choices are `spring`, `summer`, `autumn` and `winter`. The colours for each live at the top of `assets/css/site.css`.

## Publishing a letter

1. Write the letter somewhere private first.
2. Here on GitHub, choose **Add file → Create new file**.
3. Name it `_posts/YYYY-MM-DD-short-name.md`, for example `_posts/2026-12-21-the-first-letter.md`. The date in the name is the publish date.
4. Start the file with this block, then write the letter below it in Markdown:

```
---
layout: letter
title: The book that runs her week
subtitle: Delivered by Toffee. Three weeks late and slightly damp.
number: 1
season: winter
---
```

5. Click **Commit changes**. The site and the RSS feed update within a minute or two.

`_drafts/first-letter.md` shows the Markdown that gets special styling: `---` for a leaf divider, `>` for the mood quote, and `{: .callout}` under a paragraph for a coloured box.

## Images

Upload images into `assets/img/`, then use them in a letter with:

```
![What the image shows](/assets/img/your-image.png)
```

## Files

| Path | What it is |
|---|---|
| `_config.yml` | Site name, email, default season |
| `_layouts/default.html` | Frame, header and footer around every page |
| `_layouts/letter.html` | The layout for a letter |
| `_includes/` | Small reusable pieces: leaves, garland, follow box |
| `assets/css/site.css` | All the styling |
| `index.html` | The landing page (currently "coming soon") |
| `letters.html` | The list of letters, at /letters/ |
| `privacy.md` | The privacy note |
| `CNAME` | Tells GitHub the site lives at farchildgame.com |
