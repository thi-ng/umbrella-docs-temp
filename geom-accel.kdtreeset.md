<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-accel](./geom-accel.md) &gt; [KdTreeSet](./geom-accel.kdtreeset.md)

## KdTreeSet class

<b>Signature:</b>

```typescript
export declare class KdTreeSet<K extends ReadonlyVec> implements ICopy<KdTreeSet<K>>, IEmpty<KdTreeSet<K>>, IRegionQuery<K, K, number>, ISpatialSet<K> 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(dim, keys)](./geom-accel.kdtreeset._constructor_.md) |  | Constructs a new instance of the <code>KdTreeSet</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [height](./geom-accel.kdtreeset.height.md) |  | <code>number</code> |  |
|  [ratio](./geom-accel.kdtreeset.ratio.md) |  | <code>number</code> |  |
|  [size](./geom-accel.kdtreeset.size.md) |  | <code>number</code> |  |
|  [tree](./geom-accel.kdtreeset.tree.md) |  | <code>KdTreeMap&lt;K, K&gt;</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [\[Symbol.iterator\]()](./geom-accel.kdtreeset._symbol.iterator_.md) |  |  |
|  [add(key, eps)](./geom-accel.kdtreeset.add.md) |  |  |
|  [clear()](./geom-accel.kdtreeset.clear.md) |  |  |
|  [copy()](./geom-accel.kdtreeset.copy.md) |  |  |
|  [empty()](./geom-accel.kdtreeset.empty.md) |  |  |
|  [get(key, eps)](./geom-accel.kdtreeset.get.md) |  |  |
|  [has(key, eps)](./geom-accel.kdtreeset.has.md) |  |  |
|  [into(ks, eps)](./geom-accel.kdtreeset.into.md) |  |  |
|  [keys()](./geom-accel.kdtreeset.keys.md) |  |  |
|  [query(q, maxDist, limit, acc)](./geom-accel.kdtreeset.query.md) |  |  |
|  [queryKeys(q, maxDist, limit, acc)](./geom-accel.kdtreeset.querykeys.md) |  |  |
|  [queryValues(q, maxDist, limit, acc)](./geom-accel.kdtreeset.queryvalues.md) |  |  |
|  [remove(key)](./geom-accel.kdtreeset.remove.md) |  |  |
|  [values()](./geom-accel.kdtreeset.values.md) |  |  |

