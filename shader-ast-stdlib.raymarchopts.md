<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-stdlib](./shader-ast-stdlib.md) &gt; [RaymarchOpts](./shader-ast-stdlib.raymarchopts.md)

## RaymarchOpts interface

<b>Signature:</b>

```typescript
export interface RaymarchOpts 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [bias](./shader-ast-stdlib.raymarchopts.bias.md) | <code>number</code> | March step distance falloff / decay factor. Default: 0.7 |
|  [eps](./shader-ast-stdlib.raymarchopts.eps.md) | <code>number</code> | Surface tolerance, i.e. search stops once distance returned from <code>scene</code> function is less than this value. Default: 0.01 |
|  [far](./shader-ast-stdlib.raymarchopts.far.md) | <code>number</code> | Far clipping plane: Default: 10 |
|  [name](./shader-ast-stdlib.raymarchopts.name.md) | <code>string</code> | Name of generated function. Default: "raymarch" |
|  [near](./shader-ast-stdlib.raymarchopts.near.md) | <code>number</code> | Near clipping plane. Default: 0.1 |
|  [steps](./shader-ast-stdlib.raymarchopts.steps.md) | <code>number</code> | Max. iteration steps. Default: 100 |

