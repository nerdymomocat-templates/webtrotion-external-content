---
title: Remote Markdown Demo
excerpt: A short sample post rendered entirely from a GitHub folder.
---

# Remote Markdown Demo

![Hand drawn shapes](./media/post-hero.svg)

This is a **Markdown-only** post that lives outside of Notion. When you set the Notion page’s External URL to the GitHub path for `index.md`, Webtrotion will download:

- this file,
- everything inside the sibling `./media/` folder,
- and render it through the normal `PostLayout`.

## Why this is useful

- Keep long-form writing, diagrams, or custom MDX components under version control.
- Still drive the front-matter (title, tags, slug, etc.) from Notion.
- Blend Notion-native articles with GitHub-authored ones in listings, RSS, and sitemap.

## Extras

You can add callouts, fenced code blocks, tables, or embeds—anything Markdown supports. Relative links such as [`./media/post-hero.svg`](./media/post-hero.svg) continue to work because the downloader mirrors the folder structure in `public/posts/<slug>/`.
