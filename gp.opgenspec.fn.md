<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/gp](./gp.md) &gt; [OpGenSpec](./gp.opgenspec.md) &gt; [fn](./gp.opgenspec.fn.md)

## OpGenSpec.fn property

Function producing/selecting an operator value. If probabilistic, the given PRNG MUST be used for repeatable results. The function is called with all argument genes/expressions to allow inform the operator selection.

<b>Signature:</b>

```typescript
fn: Fn2<IRandom, NODE[], OP>;
```
