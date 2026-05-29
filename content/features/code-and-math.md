---
title: Code & Math
description: Syntax-highlighted code blocks and LaTeX math via KaTeX.
tags:
  - feature
  - code
  - math
---

## Code blocks

Fenced code blocks are syntax-highlighted (light & dark themes switch with the
site theme). Just tag the fence with a language:

```python
def fib(n: int) -> int:
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    return a

print([fib(i) for i in range(10)])
```

```typescript
type Note = { title: string; tags: string[] }

const publish = (n: Note): string =>
  `Publishing "${n.title}" with tags: ${n.tags.join(", ")}`
```

```bash
# Build the site locally
npx quartz build --serve
```

You can highlight specific lines and add a title:

```js {2-3} title="greet.js"
function greet(name) {
  const msg = `Hello, ${name}!` // highlighted
  return msg                    // highlighted
}
```

Inline `code` works mid-sentence too.

## Math with LaTeX

Inline math: the golden ratio is $\varphi = \frac{1 + \sqrt{5}}{2}$.

Block math renders centered:

$$
\int_{-\infty}^{\infty} e^{-x^2}\,dx = \sqrt{\pi}
$$

A matrix, because we can:

$$
A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}, \quad \det(A) = ad - bc
$$

Next up: [[diagrams]] for Mermaid charts.
