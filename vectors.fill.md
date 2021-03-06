<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/vectors](./vectors.md) &gt; [fill](./vectors.fill.md)

## fill variable

Fills Vec2/3/4 view based buffer, supporting arbitrary component and element layouts of both the input and output buffers. The `out` vector is used as write cursor over the underlying buffer and will be filled with the components of vector `v`<!-- -->.

<b>Signature:</b>

```typescript
fill: (out: IVector<any>, v: IVector<any>, num: number, so?: number) => import("./api").Vec
```

## Example


```ts
fill(
  new Vec2(new Float32Array(12)),
  new Vec2([1, 2]),
  3, // num elements
  4  // stride
)
// Float32Array [1, 2, 0, 0, 1, 2, 0, 0, 1, 2, 0, 0]

```

