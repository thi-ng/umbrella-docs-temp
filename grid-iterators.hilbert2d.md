<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/grid-iterators](./grid-iterators.md) &gt; [hilbert2d](./grid-iterators.hilbert2d.md)

## hilbert2d() function

Yields sequence of 2D grid coordinates along 2D Hilbert curve using given `cols` and `rows` (each max. 32768 (2^15)).

Ported &amp; modified from original Java code by Christopher Kulla. [https://sourceforge.net/p/sunflow/code/HEAD/tree/trunk/src/org/sunflow/core/bucket/HilbertBucketOrder.java](https://sourceforge.net/p/sunflow/code/HEAD/tree/trunk/src/org/sunflow/core/bucket/HilbertBucketOrder.java)

<b>Signature:</b>

```typescript
export declare function hilbert2d(cols: number, rows?: number): Generator<number[], void, unknown>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  cols | <code>number</code> |  |
|  rows | <code>number</code> |  |

<b>Returns:</b>

`Generator<number[], void, unknown>`

