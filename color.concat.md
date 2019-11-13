<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/color](./color.md) &gt; [concat](./color.concat.md)

## concat variable

Concatenates given color matrices by pairwise multiplying them in left-right order. Returns combined result matrix to be used with `transform()`<!-- -->.

Note: Using `concat()` is the recommended way when applying multiple color transformations in sequence. Since the transforms are combined into a single matrix, it is faster than multiple, individual `transform()` calls and will also produce more correct results, since result color clamping is only applied once at the end (by default, unless disabled).

 transform

<b>Signature:</b>

```typescript
concat: (mat: [number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number], ...xs: [number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number][]) => [number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number, number]
```