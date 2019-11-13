<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [mapcat](./transducers.mapcat.md)

## mapcat() function

Transducer. Similar to `map`<!-- -->, but expects the given mapping function `fn` to return an iterable result (or `null`<!-- -->) and then emits each value of the result individually downstream. `null` or `undefined` result values will be skipped / omitted.

<b>Signature:</b>

```typescript
export declare function mapcat<A, B>(fn: Fn<A, Iterable<B> | null | undefined>): Transducer<A, B>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  fn | <code>Fn&lt;A, Iterable&lt;B&gt; &#124; null &#124; undefined&gt;</code> | mapping function |

<b>Returns:</b>

`Transducer<A, B>`

## Example


```
[...mapcat((x) => [x, x], [1, 2, 3])]
// [ 1, 1, 2, 2, 3, 3 ]

[...mapcat((x) => x > 2 ? [x, x, x] : null, [1, 2, 3])]
// [ 3, 3, 3 ]

```
