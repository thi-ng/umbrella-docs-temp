<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-stdlib](./shader-ast-stdlib.md) &gt; [lambert](./shader-ast-stdlib.lambert.md)

## lambert variable

Inline function. Computes Lambert term, i.e. `max(dot(n, l), 0)`<!-- -->. Both vectors must be pre-normalized.

<b>Signature:</b>

```typescript
lambert: (n: Vec3Term, ldir: Vec3Term) => import("@thi.ng/shader-ast").FnCall<"float">
```
