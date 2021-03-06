<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/math](./math.md) &gt; [mixHermite](./math.mixhermite.md)

## mixHermite variable

Returns hermite interpolation of `a, b, c, d` at normalized position `t`<!-- -->, where `a` and `d` are used as predecessor/successor of `b` / `c` and only inform the tangent of the interpolation curve. The interpolated result is that of `b` and `c`<!-- -->.

Assumes all inputs are uniformly spaced. If that's not the case, use [mixCubicHermite](./math.mixcubichermite.md) with one of the tangent generators supporting non-uniform spacing of points.

See: [https://www.desmos.com/calculator/j4gf8g9vkr](https://www.desmos.com/calculator/j4gf8g9vkr)

Source: [https://www.musicdsp.org/en/latest/Other/93-hermite-interpollation.html](https://www.musicdsp.org/en/latest/Other/93-hermite-interpollation.html)

- [mixCubicHermite](./math.mixcubichermite.md) - [tangentCardinal](./math.tangentcardinal.md) - [tangentDiff3](./math.tangentdiff3.md)

<b>Signature:</b>

```typescript
mixHermite: (a: number, b: number, c: number, d: number, t: number) => number
```
