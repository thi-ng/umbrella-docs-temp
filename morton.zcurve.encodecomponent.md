<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/morton](./morton.md) &gt; [ZCurve](./morton.zcurve.md) &gt; [encodeComponent](./morton.zcurve.encodecomponent.md)

## ZCurve.encodeComponent() method

Encodes a single nD point component as partial Z index.

<b>Signature:</b>

```typescript
static encodeComponent(x: number, bits: number, dims: number, offset: number, out?: bigint): bigint;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  x | <code>number</code> | component value |
|  bits | <code>number</code> | bits per component |
|  dims | <code>number</code> | number of dimensions |
|  offset | <code>number</code> | bit offset (for curr dimension) |
|  out | <code>bigint</code> | existing partial Z result |

<b>Returns:</b>

`bigint`

