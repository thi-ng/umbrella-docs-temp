<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/dsp](./dsp.md) &gt; [madd](./dsp.madd.md)

## madd variable

Returns new multiply-add gen producing `y(t) = factor * y(t-1) + offset`<!-- -->. If `clamp` is given, the curve will be clamped at that value.

<b>Signature:</b>

```typescript
madd: (factor?: number | undefined, start?: number | undefined, offset?: number | undefined, clamp?: number | undefined) => MAdd
```
