<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [movingMedian](./transducers.movingmedian.md)

## movingMedian() function

Transducer. Similar to [movingAverage()](./transducers.movingaverage.md)<!-- -->, but yields median of sliding window and supports non-numeric inputs.

<b>Signature:</b>

```typescript
export declare function movingMedian<A, B>(n: number, opts?: Partial<SortOpts<A, B>>): Transducer<A, A>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  n | <code>number</code> | window size |
|  opts | <code>Partial&lt;SortOpts&lt;A, B&gt;&gt;</code> |  |

<b>Returns:</b>

`Transducer<A, A>`

## Remarks

The optional `key` and `cmp` function options can be used to select / compute a sortable value and change sorting behavior.

