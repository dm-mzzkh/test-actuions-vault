---
title: Media & Embeds
description: Embedding images and other notes.
tags:
  - feature
  - media
---

## Images

Embed an image stored in the vault with Obsidian's `![[file.png]]` syntax:

![[quartz-demo.png]]

You can also use standard Markdown with a relative path or a remote URL
(this page lives in `features/`, so it steps up one level to `attachments/`):

`![alt text](../attachments/quartz-demo.png)` →

![alt text](../attachments/quartz-demo.png)

> [!tip] Where to keep images
> This vault stores them in `content/attachments/`. Quartz copies them into the
> built site automatically, so the links keep working.

## Embedding (transcluding) notes

`![[note]]` pulls another note's content inline, and `![[note#Heading]]` pulls a
single section. Here's the callouts page's intro, transcluded:

![[callouts#Foldable callouts]]

Embeds are live: edit the source note and every place that transcludes it
updates on the next build.

See [[links]] for the non-embedding `[[wikilink]]` version.
