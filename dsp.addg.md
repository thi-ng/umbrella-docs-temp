<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/dsp](./dsp.md) &gt; [addG](./dsp.addg.md)

## addG variable

Creates a new [IGen](./dsp.igen.md) using given `step` gen and `start (default: 0) value, producing: `<!-- -->y(t) = step(t) + y(t-1)<!-- -->\`<!-- -->.

<b>Signature:</b>

```typescript
addG: (step: IGen<number>, start?: number) => IGen<number>
```

## Remarks

Note this is different to , which merely sums given argument gens for each step, but doesn't for a reduction like this gen.

## Example


```ts
addg(constant(1), 10).take(5)
// [ 10, 11, 12, 13, 14 ]

```
