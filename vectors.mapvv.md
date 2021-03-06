<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/vectors](./vectors.md) &gt; [mapVV](./vectors.mapvv.md)

## mapVV variable

Vec2/3/4 view based buffer transformation for [VecOpVV](./vectors.vecopvv.md) type ops and supporting arbitrary component and element layouts of all input and output buffers.

<b>Signature:</b>

```typescript
mapVV: (op: import("@thi.ng/api").Fn3<import("./api").Vec | null, import("@thi.ng/api").ArrayLikeIterable<number>, import("@thi.ng/api").ArrayLikeIterable<number>, import("./api").Vec>, out: IVector<any>, a: IVector<any>, b: IVector<any>, num: number, so?: number, sa?: number, sb?: number) => import("./api").Vec
```

## Remarks

The given pre-initialized vectors MUST be separate instances, are used as sliding cursors / views of their respective backing buffers and will be modified as part of the transformation process (though the input buffers themselves are treated as immutable, unless `out` is configured to use one of the input buffers).

In each iteration `op` is called via `op(out, a, b)`<!-- -->, followed by cursor updates to process the next vector view. No bounds checking is performed.

This function returns `out`<!-- -->'s backing buffer.

## Example


```ts
// each input buffer contains 2 2D vectors, but using
// different strided data layouts
mapVV(
  // transformation function
  add,
  // init output buffer view
  new Vec2(),
  // wrap 1st input buffer & configure offset & component stride
  new Vec2([1,0,2,0,0,0,0,0,3,0,4,0,0,0,0,0], 0, 2),
  // wrap 2nd input buffer
  new Vec2([0,10,0,0,20,0,0,30,0,0,40], 1, 3),
  2, // num vectors
  2, // output element stride
  8, // input #1 element stride
  6  // input #2 element stride
);
// [ 11, 22, 33, 44 ]

```
Alternatively, `Vec2/3/4.iterator()` combined with transducers can be used to achieve the same (and more flexible) transformations, but will incur more intermediate object allocations. `mapV*()` functions only use (and mutate) the provided vector instances and do not allocate any further objects.

```ts
// output buffer
const out = new Array(4);

tx.run(
  tx.map(([o, a, b]) => add(o, a, b)),
  tx.zip(
     Vec2.iterator(out, 2),
     Vec2.iterator([1,0,2,0,0,0,0,0,3,0,4,0,0,0,0,0], 2, 0, 2, 8),
     Vec2.iterator([0,10,0,0,20,0,0,30,0,0,40], 2, 1, 3, 6),
  )
);

out
// [ 11, 22, 33, 44 ]

```

