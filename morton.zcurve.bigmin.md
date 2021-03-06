<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/morton](./morton.md) &gt; [ZCurve](./morton.zcurve.md) &gt; [bigMin](./morton.zcurve.bigmin.md)

## ZCurve.bigMin() method

Computes the next valid Z index in bbox defined by `zmin` / `zmax` and greater than `zcurr`<!-- -->. Returns -1 if no further indices are in the box.

<b>Signature:</b>

```typescript
bigMin(zcurr: bigint, zmin: bigint, zmax: bigint): bigint;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  zcurr | <code>bigint</code> |  |
|  zmin | <code>bigint</code> |  |
|  zmax | <code>bigint</code> |  |

<b>Returns:</b>

`bigint`

## Remarks

Partially based on: [https://github.com/statgen/LDServer/blob/master/core/src/Morton.cpp\#L38](https://github.com/statgen/LDServer/blob/master/core/src/Morton.cpp#L38)

