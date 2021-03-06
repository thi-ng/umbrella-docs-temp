<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-accel](./geom-accel.md) &gt; [NdQuadtreeSet](./geom-accel.ndquadtreeset.md)

## NdQuadtreeSet class

<b>Signature:</b>

```typescript
export declare class NdQuadtreeSet<K extends ReadonlyVec> implements ICopy<NdQuadtreeSet<K>>, IEmpty<NdQuadtreeSet<K>>, IRegionQuery<K, K, number>, ISpatialSet<K> 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(pos, ext, keys)](./geom-accel.ndquadtreeset._constructor_.md) |  | Constructs a new instance of the <code>NdQuadtreeSet</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [\_size](./geom-accel.ndquadtreeset._size.md) |  | <code>number</code> |  |
|  [size](./geom-accel.ndquadtreeset.size.md) |  | <code>number</code> |  |
|  [tree](./geom-accel.ndquadtreeset.tree.md) |  | <code>NdQuadtreeMap&lt;K, K&gt;</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [\[Symbol.iterator\]()](./geom-accel.ndquadtreeset._symbol.iterator_.md) |  |  |
|  [add(key, eps)](./geom-accel.ndquadtreeset.add.md) |  |  |
|  [clear()](./geom-accel.ndquadtreeset.clear.md) |  |  |
|  [copy()](./geom-accel.ndquadtreeset.copy.md) |  |  |
|  [empty()](./geom-accel.ndquadtreeset.empty.md) |  |  |
|  [fromMinMax(min, max)](./geom-accel.ndquadtreeset.fromminmax.md) | <code>static</code> | Returns a new point-based <code>NdQuadtreeSet</code> for nD keys in given region defined by <code>min</code> / <code>max</code> coordinates. The dimensionality of the tree is implicitly defined by the provided coordinates. Only points within that region can be indexed. |
|  [get(key, eps)](./geom-accel.ndquadtreeset.get.md) |  |  |
|  [has(key, eps)](./geom-accel.ndquadtreeset.has.md) |  |  |
|  [into(keys, eps)](./geom-accel.ndquadtreeset.into.md) |  |  |
|  [keys()](./geom-accel.ndquadtreeset.keys.md) |  |  |
|  [query(q, maxDist, limit, acc)](./geom-accel.ndquadtreeset.query.md) |  |  |
|  [queryKeys(q, maxDist, limit, acc)](./geom-accel.ndquadtreeset.querykeys.md) |  |  |
|  [queryValues(q, maxDist, limit, acc)](./geom-accel.ndquadtreeset.queryvalues.md) |  |  |
|  [remove(key)](./geom-accel.ndquadtreeset.remove.md) |  |  |
|  [values()](./geom-accel.ndquadtreeset.values.md) |  |  |

