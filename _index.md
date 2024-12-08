---
bookCollapseSection: true  
weight: 9  
draft: false  
title: Reformatter  
---

**Reformatter methods** enable the conversion of a `quadrille` into various formats, such as [BigInt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BigInt), [images](https://p5js.org/reference/#/p5.Image), and array-based data structures. These methods ensure seamless transitions and promote interoperability between `quadrille` instances and other data representations, making it easier to integrate quadrilles into different workflows.  

## Method Overview  

- **[toArray()]({{< relref "to_array" >}}):** Converts the `quadrille` into a two-dimensional array, preserving its cell structure and content.  
- **[toBigInt()]({{< relref "to_bigint" >}}):** Converts the `quadrille` into a `BigInt`, encoding its non-empty cells as bits.  
- **[toImage()]({{< relref "to_image" >}}):** Generates a [p5.Image](https://p5js.org/reference/#/p5.Image) representation of the `quadrille`, rendering its content as pixels.  
- **[toFEN()]({{< relref "to_fen" >}})**: Encodes the quadrille into a FEN (Forsyth-Edwards Notation) string, often used for representing board states in games like chess.


These reformatter methods provide versatile tools for exporting and working with `quadrille` data in alternative formats. Whether you need binary encoding, image rendering, or array-based representations, these methods ensure smooth interoperability and flexibility.