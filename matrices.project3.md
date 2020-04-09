<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/matrices](./matrices.md) &gt; [project3](./matrices.project3.md)

## project3 variable

Same as [project](./matrices.project.md)<!-- -->, but slightly faster and more convenient for the most common use case of projecting a 3D input point (assumes `w=1` for its homogeneous coordinate, i.e. `[x,y,z,1]`<!-- -->). Returns `undefined` if the computed perspective divisor is zero (and would cause in `NaN` results).

<b>Signature:</b>

```typescript
project3: (out: Vec | null, mvp: import("@thi.ng/api").ArrayLikeIterable<number>, view: import("@thi.ng/api").ArrayLikeIterable<number>, p: import("@thi.ng/api").ArrayLikeIterable<number>) => Vec | undefined
```