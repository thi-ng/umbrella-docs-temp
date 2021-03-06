<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [interpolateLinear](./transducers.interpolatelinear.md)

## interpolateLinear() function

Pre-configured version of [interpolate()](./transducers.interpolate.md) for numeric values and using pairwise linear interpolation.

<b>Signature:</b>

```typescript
export declare function interpolateLinear(n: number): Transducer<number, number>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  n | <code>number</code> |  |

<b>Returns:</b>

`Transducer<number, number>`

## Remarks

The number of samples per interval is configurable. No values will be produced if there're less than 2 inputs.

See also: - [interpolate()](./transducers.interpolate.md) - [interpolateHermite()](./transducers.interpolatehermite.md)

