<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [streamShuffle](./transducers.streamshuffle.md)

## streamShuffle() function

Transducer. Creates internal sliding window of `n` values and performs `maxSwaps` random shuffle operations for each new value and yields values in shuffled order. By default `maxSwaps` is the same as the chosen chunk size.

```
[...streamShuffle(5, range(10))]
// [ 3, 2, 5, 0, 8, 7, 1, 6, 4, 9 ]

```

<b>Signature:</b>

```typescript
export declare function streamShuffle<T>(n: number, maxSwaps?: number): Transducer<T, T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  n | <code>number</code> | sliding window size |
|  maxSwaps | <code>number</code> | number of swaps per input |

<b>Returns:</b>

`Transducer<T, T>`
