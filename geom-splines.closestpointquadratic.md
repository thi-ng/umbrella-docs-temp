<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-splines](./geom-splines.md) &gt; [closestPointQuadratic](./geom-splines.closestpointquadratic.md)

## closestPointQuadratic variable

Performs recursive search for closest point to `p` on quadratic curve defined by control points `a`<!-- -->,`b`<!-- -->,`c`<!-- -->. The `res` and `recur` params are used to control the recursion behavior. If `eps` is given, the search is terminated as soon as a point with a shorter \*squared\* distance than `eps` is found.

 thi.ng/math/minError

<b>Signature:</b>

```typescript
closestPointQuadratic: (p: import("@thi.ng/api").ArrayLikeIterable<number>, a: import("@thi.ng/api").ArrayLikeIterable<number>, b: import("@thi.ng/api").ArrayLikeIterable<number>, c: import("@thi.ng/api").ArrayLikeIterable<number>, out?: Vec, res?: number | undefined, iter?: number | undefined, eps?: number | undefined) => Vec
```