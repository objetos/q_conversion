---
weight: 1
draft: false
title: toArray()
---

Returns a [row-major order](https://en.wikipedia.org/wiki/Row-_and_column-major_order) array of the quadrille cells (refer to [createQuadrille]({{< relref "create_quadrille" >}}) for all the possible cell contents). The resulting array has [width]({{< ref "width" >}}) `*` [height]({{< ref "height" >}}) entries, with empty cells as `null`.

## Syntax

> `toArray()`