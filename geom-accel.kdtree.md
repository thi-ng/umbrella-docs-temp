<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-accel](./geom-accel.md) &gt; [KdTree](./geom-accel.kdtree.md)

## KdTree class

[https://en.wikipedia.org/wiki/K-d\_tree](https://en.wikipedia.org/wiki/K-d_tree)

Partially based on: [https://github.com/ubilabs/kd-tree-javascript](https://github.com/ubilabs/kd-tree-javascript)

<b>Signature:</b>

```typescript
export declare class KdTree<K extends ReadonlyVec, V> implements ICopy<KdTree<K, V>>, ISpatialAccel<K, V> 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(dim, pairs)](./geom-accel.kdtree._constructor_.md) |  | Constructs a new instance of the <code>KdTree</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [\_length](./geom-accel.kdtree._length.md) |  | <code>number</code> |  |
|  [dim](./geom-accel.kdtree.dim.md) |  | <code>number</code> |  |
|  [length](./geom-accel.kdtree.length.md) |  | <code>number</code> |  |
|  [root](./geom-accel.kdtree.root.md) |  | <code>KdNode&lt;K, V&gt; &#124; null</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [\[Symbol.iterator\]()](./geom-accel.kdtree._symbol.iterator_.md) |  |  |
|  [add(p, v, eps)](./geom-accel.kdtree.add.md) |  |  |
|  [addAll(pts, eps)](./geom-accel.kdtree.addall.md) |  |  |
|  [addKey(k, eps)](./geom-accel.kdtree.addkey.md) |  |  |
|  [addKeys(ks, eps)](./geom-accel.kdtree.addkeys.md) |  |  |
|  [balanceRatio()](./geom-accel.kdtree.balanceratio.md) |  |  |
|  [buildSelection(q, maxNum, maxDist)](./geom-accel.kdtree.buildselection.md) |  |  |
|  [buildTree(points, depth, parent)](./geom-accel.kdtree.buildtree.md) |  |  |
|  [copy()](./geom-accel.kdtree.copy.md) |  |  |
|  [doSelect(q, f, maxNum, maxDist)](./geom-accel.kdtree.doselect.md) |  |  |
|  [has(k, eps)](./geom-accel.kdtree.has.md) |  |  |
|  [keys()](./geom-accel.kdtree.keys.md) |  |  |
|  [remove(p)](./geom-accel.kdtree.remove.md) |  |  |
|  [select(q, maxNum, maxDist)](./geom-accel.kdtree.select.md) |  |  |
|  [selectKeys(q, maxNum, maxDist)](./geom-accel.kdtree.selectkeys.md) |  |  |
|  [selectVals(q, maxNum, maxDist)](./geom-accel.kdtree.selectvals.md) |  |  |

