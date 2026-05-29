---
title: Links & Backlinks
description: Wikilinks, aliases, heading links, embeds, and automatic backlinks.
tags:
  - feature
  - linking
aliases:
  - wikilinks
---

The whole point of a digital garden is **connecting** notes. Quartz understands
Obsidian's `[[wikilink]]` syntax natively.

## Wikilinks

| You write | It links to |
| --- | --- |
| `[[callouts]]` | [[callouts]] |
| `[[callouts\|see the callouts page]]` | [[callouts\|see the callouts page]] |
| `[[formatting#Tables]]` | [[formatting#Tables]] (jumps to a heading) |
| `[[index]]` | [[index]] (the home page) |

> [!note] Link resolution
> This vault uses `markdownLinkResolution: shortest`, so `[[callouts]]` finds the
> note no matter which folder it lives in — you don't need the full path.

You can also use plain Markdown links, e.g.
[the Quartz docs](https://quartz.jzhao.xyz).

## Aliases

This note declares `aliases: [wikilinks]` in its frontmatter, so a link like
`[[wikilinks]]` also lands here — handy when a page is known by several names.

## Embeds / transclusion

Pull the content of another note straight into this one with `![[...]]`:

![[tags-and-metadata#What is frontmatter?]]

*(Everything above this line between the rules came from [[tags-and-metadata]].)*

## Backlinks

Scroll to the bottom of any page (or look in the right sidebar) to see
**Backlinks** — every note that links *to* this one, generated automatically.
This page is linked from [[index]] and [[features/index|the features index]], so
both show up as backlinks here.
