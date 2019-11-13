<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/math](./math.md) &gt; [solveCubic](./math.solvecubic.md)

## solveCubic variable

Computes solutions for quadratic equation: `ax^3 + bx^2 + c*x + d = 0`<!-- -->. Returns array of solutions, both real &amp; imaginary. Note: `a` MUST NOT be zero. If the cubic term is missing (i.e. zero), use `solveQuadratic` or `solveLinear` instead.

[https://en.wikipedia.org/wiki/Cubic\_function](https://en.wikipedia.org/wiki/Cubic_function)

<b>Signature:</b>

```typescript
solveCubic: (a: number, b: number, c: number, d: number, eps?: number) => number[]
```