---
title: Tags & Metadata
description: How frontmatter and tags drive titles, descriptions, and tag pages.
tags:
  - feature
  - metadata
  - demo
---

## What is frontmatter?

Frontmatter is the little YAML block at the very top of a note, between two
`---` lines. Quartz reads it to set the page **title**, **description** (used for
SEO and link previews), **tags**, and **aliases**. This page's frontmatter looks
like:

```yaml
---
title: Tags & Metadata
description: How frontmatter and tags drive titles, descriptions, and tag pages.
tags:
  - feature
  - metadata
  - demo
aliases:
  - metadata
---
```

If you omit `title`, Quartz falls back to the first `# Heading` or the file name.

## Tags

You can declare tags in frontmatter (above) **or** inline anywhere in the body,
like #example and #digital-garden. Click any tag to open its auto-generated tag
page listing every note that uses it.

A few tags used across this vault:

- #demo — the overview pages
- #feature — each feature tour page
- #markdown — Markdown-syntax pages

## Why it matters

Good metadata gives you:

1. Clean titles and link previews
2. Working tag pages and search
3. Better backlinks and graph clustering — see [[links]]

Back to the [[features/index|feature tour]] or the [[index|home page]].
