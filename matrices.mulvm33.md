<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/matrices](./matrices.md) &gt; [mulVM33](./matrices.mulvm33.md)

## mulVM33 variable

Same as:

<b>Signature:</b>

```typescript
mulVM33: (out: Vec | null, v: import("@thi.ng/api").ArrayLikeIterable<number>, m: import("@thi.ng/api").ArrayLikeIterable<number>) => Vec
```

## Example


```ts
out[0] = dot(v, column(m, 0))
out[1] = dot(v, column(m, 1))
out[2] = dot(v, column(m, 2))

```

