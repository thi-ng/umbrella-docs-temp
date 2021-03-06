<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/vectors](./vectors.md) &gt; [mapV](./vectors.mapv.md)

## mapV variable

Like [mapVV](./vectors.mapvv.md)<!-- -->, but for [VecOpV](./vectors.vecopv.md) type ops and hence only using single input.

<b>Signature:</b>

```typescript
mapV: (op: import("@thi.ng/api").Fn2<import("./api").Vec | null, import("@thi.ng/api").ArrayLikeIterable<number>, import("./api").Vec>, out: IVector<any>, a: IVector<any>, num: number, so?: number, sa?: number) => import("./api").Vec
```

## Example


```ts
// 4x 2D vectors in SOA layout
// i.e. [x1, x2, x3, x4, y1, y2, y3, y4]
buf = [1, 3, 5, 7, 2, 4, 6, 8];

// use `swapXY` to swizzle each vector and use AOS for output
res = mapV(swapXY, new Vec2(), new Vec2(buf, 0, 4), 4, 2, 1);
// [ 2, 1, 4, 3, 6, 5, 8, 7 ]

// unpack result for demonstration purposes
[...Vec2.iterator(res, 4)].map(v => [...v]);
// [ [ 2, 1 ], [ 4, 3 ], [ 6, 5 ], [ 8, 7 ] ]

```

