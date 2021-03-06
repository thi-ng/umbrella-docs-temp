<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/math](./math.md) &gt; [solveQuadratic](./math.solvequadratic.md)

## solveQuadratic variable

Computes solutions for quadratic equation: `ax^2 + bx + c = 0`<!-- -->. Returns array of real solutions. Note: `a` MUST NOT be zero. If the quadratic term is missing, use [solveLinear](./math.solvelinear.md) instead.

- [https://en.wikipedia.org/wiki/Quadratic\_function](https://en.wikipedia.org/wiki/Quadratic_function) - [https://en.wikipedia.org/wiki/Quadratic\_equation](https://en.wikipedia.org/wiki/Quadratic_equation)

<b>Signature:</b>

```typescript
solveQuadratic: (a: number, b: number, c: number, eps?: number) => number[]
```
