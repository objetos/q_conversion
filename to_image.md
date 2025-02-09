---
weight: 3
draft: false
title: toImage(args)
---

Returns a [p5.Image](https://p5js.org/reference/#/p5.Image) representation of this quadrille.

## Syntax

> `toImage(filename, [{[values], [tileDisplay], [imageDisplay], [colorDisplay], [stringDisplay], [numberDisplay], [arrayDisplay], [objectDisplay], [cellLength], [outlineWeight], [outline], [textColor], [textZoom]}])`

## Parameters

| Param         | Description                                                                                               |
|---------------|-----------------------------------------------------------------------------------------------------------|
| `filename`    | String: image name, png and jpg extensions are supported                                                  |
| `tileDisplay` | Function: empty cell drawing custom procedure default is [Quadrille.tileDisplay]({{< ref "display_fns" >}})[^1].  Use `0`, `null` or `undefined` to discard all edges |
| `imageDisplay` | Function: image filled cell drawing custom procedure default is [Quadrille.imageDisplay]({{< ref "display_fns" >}})    |
| `colorDisplay` | Function: color filled cell drawing custom procedure default is [Quadrille.colorDisplay]({{< ref "display_fns" >}})    |
| `stringDisplay` | Function: string filled cell drawing custom procedure default is [Quadrille.stringDisplay]({{< ref "display_fns" >}}) |
| `numberDisplay` | Function: number filled cell drawing custom procedure default is [Quadrille.numberDisplay]({{< ref "display_fns" >}}) |
| `arrayDisplay` | Function: array filled cell drawing custom procedure                                                      |
| `objectDisplay` | Function: object filled cell drawing custom procedure                                                     |
| `values`      | [Iterable](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of): cells to be exported. All cells are exported if this parameter is `undefined` |
| `cellLength`  | Number: edge length in pixels default is [Quadrille.cellLength]({{< ref "cell_length" >}})               |
| `outlineWeight` | Number: edge weight default is [Quadrille.outlineWeight]({{< ref "outline_weight" >}}).                  |
| `outline`       | [p5.Color](https://p5js.org/reference/#/p5.Color) representation: edge color default is [Quadrille.outline]({{< ref "outline" >}}) |
| `textColor`     | [p5.Color](https://p5js.org/reference/#/p5.Color) representation: text color default is [Quadrille.textColor]({{< ref "text_color" >}}) |
| `textZoom`      | Number:: text zoom level default is [Quadrille.textZoom]({{< ref "text_zoom" >}})                        |

[^1]: This function allows to implementing other [regular tilings](https://en.wikipedia.org/wiki/Euclidean_tilings_by_convex_regular_polygons#Regular_tilings) different than the default [square tiling](https://en.wikipedia.org/wiki/Square_tiling).