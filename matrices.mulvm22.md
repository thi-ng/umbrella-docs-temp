<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/matrices](./matrices.md) &gt; [mulVM22](./matrices.mulvm22.md)

## mulVM22 variable

Same as:

<b>Signature:</b>

```typescript
mulVM22: (out: Vec | null, v: import("@thi.ng/api").ArrayLikeIterable<number>, m: import("@thi.ng/api").ArrayLikeIterable<number>) => Vec
```

## Example


```ts
out[0] = dot(v, column(m, 0))
out[1] = dot(v, column(m, 1))

```

