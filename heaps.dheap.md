<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/heaps](./heaps.md) &gt; [DHeap](./heaps.dheap.md)

## DHeap class

Generic d-ary heap / priority queue with configurable arity (default = 4) and ordering via user-supplied comparator.

<b>Signature:</b>

```typescript
export declare class DHeap<T> extends Heap<T> implements ICopy<DHeap<T>>, IEmpty<DHeap<T>>, IStack<T, T, DHeap<T>> 
```

## Remarks

By default, implements min-heap ordering and uses [compare](./compare.compare.md)<!-- -->. The arity `d` must be &gt;<!-- -->= 2 (default: 4). If `d=2`<!-- -->, the default binary [Heap](./heaps.heap.md) implementation will be faster.

[https://en.wikipedia.org/wiki/D-ary\_heap](https://en.wikipedia.org/wiki/D-ary_heap)

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(values, opts)](./heaps.dheap._constructor_.md) |  | Constructs a new instance of the <code>DHeap</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [d](./heaps.dheap.d.md) |  | <code>number</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [childIndex(idx, d)](./heaps.dheap.childindex.md) | <code>static</code> | Returns index of 1st child or -1 if <code>idx &lt; 0</code>. |
|  [children(n)](./heaps.dheap.children.md) |  |  |
|  [copy()](./heaps.dheap.copy.md) |  |  |
|  [empty()](./heaps.dheap.empty.md) |  |  |
|  [heapify(vals)](./heaps.dheap.heapify.md) |  |  |
|  [leaves()](./heaps.dheap.leaves.md) |  |  |
|  [parent(n)](./heaps.dheap.parent.md) |  |  |
|  [parentIndex(idx, d)](./heaps.dheap.parentindex.md) | <code>static</code> | Returns index of parent node or -1 if <code>idx &lt; 1</code>. |
|  [percolateDown(i, vals)](./heaps.dheap.percolatedown.md) |  |  |
|  [percolateUp(i, vals)](./heaps.dheap.percolateup.md) |  |  |

