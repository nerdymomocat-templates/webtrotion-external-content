## External Content Sample

You can copy these folders into a public GitHub repo and point a Notion post’s **External URL** at one of the files to test the new remote-content flow.

Structure:

```
examples/external-content-sample/
├── markdown/
│   └── test-markdown-post/
│       ├── index.md
│       └── media/
│           └── post-hero.svg
├── mdx/
│   └── test-mdx-post/
│       ├── index.mdx
│       ├── components/
│       │   └── FancyBadge.astro
│       └── media/
│           └── diagram.svg
└── html/
    └── test-html-post/
        ├── index.html
        └── media/
            └── wireframe.svg
└── custom-components/
    └── SpotlightCard.astro
```

### Usage

1. Copy any of the sample folders into a public GitHub repository.
2. Point a Notion entry’s **External URL** at one of the files (e.g. `https://github.com/you/repo/tree/main/markdown/test-markdown-post/index.md`).
3. Add the repo prefix to `constants-config.json5 -> external-content.url-prefixes`.
4. Run `npm run build-local`; the site will download and render the remote content.

> **Note:** MDX and custom-component imports are provided for testing future enhancements. Today’s build renders Markdown/HTML; once MDX + remote component support ships, these examples will exercise that code path.
