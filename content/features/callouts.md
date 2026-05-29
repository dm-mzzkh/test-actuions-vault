---
title: Callouts
description: Obsidian-style callouts / admonitions in every flavor.
tags:
  - feature
  - markdown
---

Callouts (a.k.a. admonitions) use the `> [!type]` syntax. They're great for
warnings, tips, and asides.

> [!note] Note
> The default, neutral callout.

> [!tip] Tip
> Helpful advice goes here.

> [!info]
> An informational block — the title is optional and defaults to the type name.

> [!warning] Heads up
> Use this to flag something risky.

> [!danger] Danger
> For destructive or breaking actions.

> [!success] Done
> Also available as `[!check]` / `[!done]`.

> [!question] FAQ
> Also `[!help]` / `[!faq]`.

> [!quote] Quote
> "Notes are the residue of thought." — and they look great as callouts.

## Foldable callouts

Add `+` (open) or `-` (collapsed) after the type to make a callout foldable:

> [!example]- Click to expand
> This callout starts **collapsed**. Foldable callouts are perfect for spoilers,
> long examples, or optional detail.

## Nesting

> [!note] Outer
> Callouts can nest.
> > [!tip] Inner
> > And the inner one keeps its own styling.

See also: [[formatting]] for the rest of the text features.
