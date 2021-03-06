<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-closest-point](./geom-closest-point.md) &gt; [closestT](./geom-closest-point.closestt.md)

## closestT variable

Computes the parametric distance `t` of point `p` projected onto line `a` -<!-- -->&gt; `b`<!-- -->, relative to `a`<!-- -->. I.e. the projection of `p` can then be computed like so:

<b>Signature:</b>

```typescript
closestT: (p: import("@thi.ng/api").ArrayLikeIterable<number>, a: import("@thi.ng/api").ArrayLikeIterable<number>, b: import("@thi.ng/api").ArrayLikeIterable<number>) => number | undefined
```

## Example


```ts
mixN([], a, b, closestT(p, a, b))

```
If the return value is outside the closed \[0,1\] interval, the projected point lies outside the line segment. Returns `undefined` if `a` and `b` are coincident.

- [closestPointLine](./geom-closest-point.closestpointline.md) - [closestPointSegment](./geom-closest-point.closestpointsegment.md)

