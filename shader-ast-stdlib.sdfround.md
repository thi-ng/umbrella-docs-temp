<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-stdlib](./shader-ast-stdlib.md) &gt; [sdfRound](./shader-ast-stdlib.sdfround.md)

## sdfRound variable

Inline function. Essentially an isoline offset to create:

- `r > 0`<!-- -->: rounded/thicker shapes - `r < 0`<!-- -->: sharper/thinner shapes

<b>Signature:</b>

```typescript
sdfRound: (d: FloatTerm, r: FloatTerm) => import("@thi.ng/shader-ast").Op2<"float">
```
