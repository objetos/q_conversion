---
weight: 5
draft: false
---

# toImage

Returns a [p5.Image](https://p5js.org/reference/#/p5.Image) representation of this quadrille.

# Syntax

> `toImage(filename, [{[cells], [tileDisplay], [imageDisplay], [colorDisplay], [stringDisplay], [numberDisplay], [arrayDisplay], [objectDisplay], [cellLength], [outlineWeight], [outline], [textColor], [textZoom]}])`

# Parameters

| parameter     | description                                                                                               |
|---------------|-----------------------------------------------------------------------------------------------------------|
| filename      | String: image name, png and jpg extensions are supported                                                  |
| tileDisplay   | Function: empty cell drawing custom procedure default is [Quadrille.TILE]({{< ref "tile" >}})[^1].  Use `0`, `null` or `undefined` to discard all edges |
| imageDisplay  | Function: image filled cell drawing custom procedure default is [Quadrille.IMAGE]({{< ref "image" >}})    |
| colorDisplay  | Function: color filled cell drawing custom procedure default is [Quadrille.COLOR]({{< ref "color" >}})    |
| stringDisplay | Function: string filled cell drawing custom procedure default is [Quadrille.STRING]({{< ref "string" >}}) |
| numberDisplay | Function: number filled cell drawing custom procedure default is [Quadrille.NUMBER]({{< ref "number" >}}) |
| arrayDisplay  | Function: array filled cell drawing custom procedure                                                      |
| objectDisplay | Function: object filled cell drawing custom procedure                                                     |
| cells         | [Iterable](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of): cells to be exported. All cells are exported if this parameter is `undefined` |
| cellLength    | Number: edge length in pixels default is [Quadrille.CELL_LENGTH]({{< ref "cell_length" >}})               |
| outlineWeight | Number: edge weight default is [Quadrille.OUTLINE_WEIGHT]({{< ref "outline_weight" >}}).                  |
| outline       | [p5.Color](https://p5js.org/reference/#/p5.Color) representation: edge color default is [Quadrille.OUTLINE]({{< ref "outline" >}}) |
| textColor     | [p5.Color](https://p5js.org/reference/#/p5.Color) representation: text color default is [Quadrille.TEXT_COLOR]({{< ref "text_color" >}}) |
| textZoom      | Number:: text zoom level default is [Quadrille.TEXT_ZOOM]({{< ref "text_zoom" >}})                        |

[^1]: This function allows to implementing other [regular tilings](https://en.wikipedia.org/wiki/Euclidean_tilings_by_convex_regular_polygons#Regular_tilings) different than the default [square tiling](https://en.wikipedia.org/wiki/Square_tiling).