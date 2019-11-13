<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/math](./math.md) &gt; [tangentCardinal](./math.tangentcardinal.md)

## tangentCardinal variable

Helper function for `mixCubicHermite()`<!-- -->. Computes cardinal tangents based on point neighbors of a point B (not given), i.e. `a` (predecessor) and `c` (successor) and their times (defaults to uniformly spaced). The optional `tension` parameter can be used to scale the tangent where 0.0 produces a Cardinal spline tangent and 1.0 a Catmull-Rom (opposite to the Wikipedia ref).

[https://en.wikipedia.org/wiki/Cubic\_Hermite\_spline\#Cardinal\_spline](https://en.wikipedia.org/wiki/Cubic_Hermite_spline#Cardinal_spline)

<b>Signature:</b>

```typescript
tangentCardinal: (prev: number, next: number, scale?: number, ta?: number, tc?: number) => number
```