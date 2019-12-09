<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/gp](./gp.md) &gt; [GPOpts](./gp.gpopts.md)

## GPOpts interface

<b>Signature:</b>

```typescript
export interface GPOpts<OP, T, ARGS> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [ops](./gp.gpopts.ops.md) | <code>OpGenSpec&lt;ARGS, OP&gt;[]</code> | Operator node generators. |
|  [probMutate](./gp.gpopts.probmutate.md) | <code>number</code> | Per-gene mutation probability. MUST be &lt; 1 for [ASTOpts](./gp.astopts.md) to avoid infinite tree expansion. |
|  [rnd](./gp.gpopts.rnd.md) | <code>IRandom</code> | Possibly seeded PRNG instance to be used for AST generation / editing. |
|  [terminal](./gp.gpopts.terminal.md) | <code>Fn&lt;IRandom, T&gt;</code> | Terminal node generator. If probabilistic, the given PRNG MUST be used for repeatable results. |
