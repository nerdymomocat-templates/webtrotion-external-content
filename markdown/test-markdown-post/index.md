# Markdown Integration Surface

> [!NOTE]
> This tests GitHub callouts, footnotes [^fn1], citations [@smith2020], media, HTML passthrough, tasks, and tables.

## Headings and Lists
- Bullet item one
- [ ] Task unchecked
- [x] Task checked
1. Ordered one
2. Ordered two

### Blockquote
> Nested text with a [link](https://example.com) and a footnote marker [^fn2].

## Code Fence
```js
console.log("hello world");
```

## Table (alignment ignored)

| Feature         | Status  | Notes              |
| --------------- | ------- | ------------------ |
| Callouts        | ✅      | [!WARNING] inside cells stays literal |
| Tasks           | ✅      | Task list items map to ToDo            |
| Footnotes       | ✅      | GFM footnotes collected                |

## Media

- Inline image: here ![hello](./media/post-hero.svg)
- Video link auto-upgraded: [Launch video](./media/sqmedia.mp4)

## Raw HTML passthrough
<div class="custom-html-block">
  <p>Inline HTML with <strong>bold</strong> and a relative asset:</p>
  <img src="./media/post-hero.svg" alt="Hero via HTML" />
</div>
<!-- This comment should be hidden -->

## Footnotes & Citations

Regular paragraph with citation [@smith2020] and another footnote [^fn3].

[^fn1]: Footnote one from callout.
[^fn2]: Footnote from inside a quote.
[^fn3]: Footnote from the closing section.
