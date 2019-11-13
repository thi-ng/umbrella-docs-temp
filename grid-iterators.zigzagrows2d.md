<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/grid-iterators](./grid-iterators.md) &gt; [zigzagRows2d](./grid-iterators.zigzagrows2d.md)

## zigzagRows2d() function

Yields sequence of 2D grid coordinates in zigzag row order starting from \[0,0\], given `cols` and `rows`<!-- -->.

Ported &amp; modified from original Java code by Christopher Kulla. [https://sourceforge.net/p/sunflow/code/HEAD/tree/trunk/src/org/sunflow/core/bucket/SpiralBucketOrder.java](https://sourceforge.net/p/sunflow/code/HEAD/tree/trunk/src/org/sunflow/core/bucket/SpiralBucketOrder.java)

<b>Signature:</b>

```typescript
export declare function zigzagRows2d(cols: number, rows?: number): Generator<number[], void, unknown>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  cols | <code>number</code> |  |
|  rows | <code>number</code> |  |

<b>Returns:</b>

`Generator<number[], void, unknown>`
