---
title: Diagrams
description: Mermaid diagrams rendered directly from code fences.
tags:
  - feature
  - diagrams
---

Quartz renders [Mermaid](https://mermaid.js.org) diagrams from a ` ```mermaid `
code fence (enabled via the `mermaid: true` option on the Obsidian-flavored
Markdown plugin).

## Flowchart

```mermaid
flowchart TD
    A[Note in Obsidian] -->|git push| B(GitHub repo)
    B --> C{GitHub Actions}
    C -->|build| D[Quartz]
    D --> E[(GitHub Pages)]
    E --> F((Live site))
```

## Sequence diagram

```mermaid
sequenceDiagram
    participant You
    participant GitHub
    participant Pages
    You->>GitHub: git push
    GitHub->>GitHub: Run Quartz build
    GitHub->>Pages: Upload static site
    Pages-->>You: Published URL
```

## Class / entity diagram

```mermaid
classDiagram
    class Note {
      +string title
      +string[] tags
      +render() string
    }
    class Vault {
      +Note[] notes
    }
    Vault "1" o-- "many" Note
```

These render as real SVG diagrams in the browser — try toggling dark mode and
they'll re-theme. Back to the [[features/index|feature tour]].
