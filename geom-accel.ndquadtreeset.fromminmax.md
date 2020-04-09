<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-accel](./geom-accel.md) &gt; [NdQuadtreeSet](./geom-accel.ndquadtreeset.md) &gt; [fromMinMax](./geom-accel.ndquadtreeset.fromminmax.md)

## NdQuadtreeSet.fromMinMax() method

Returns a new point-based `NdQuadtreeSet` for nD keys in given region defined by `min` / `max` coordinates. The dimensionality of the tree is implicitly defined by the provided coordinates. Only points within that region can be indexed.

<b>Signature:</b>

```typescript
static fromMinMax<K extends ReadonlyVec>(min: ReadonlyVec, max: ReadonlyVec): NdQuadtreeSet<K>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  min | <code>ReadonlyVec</code> |  |
|  max | <code>ReadonlyVec</code> |  |

<b>Returns:</b>

`NdQuadtreeSet<K>`

## Remarks

Due to exponentially growing lookup tables, currently only supports up to 16 dimensions.
