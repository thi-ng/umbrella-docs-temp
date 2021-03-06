<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [take](./transducers.take.md)

## take() function

Transducer which only yields the first `n` values and then terminates transformation (by emitting a [reduced](./transducers.reduced.md) value).

<b>Signature:</b>

```typescript
export declare function take<T>(n: number): Transducer<T, T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  n | <code>number</code> |  |

<b>Returns:</b>

`Transducer<T, T>`

## Example


```ts
[...iterator(comp(take(5), map((x) => x * 10)), range(10))]
// [ 0, 10, 20, 30, 40 ]

```

