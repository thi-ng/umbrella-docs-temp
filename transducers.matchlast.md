<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [matchLast](./transducers.matchlast.md)

## matchLast() function

Transducer composition / syntax sugar for:

<b>Signature:</b>

```typescript
export declare function matchLast<T>(pred: Predicate<T>): Transducer<T, T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  pred | <code>Predicate&lt;T&gt;</code> | predicate function |

<b>Returns:</b>

`Transducer<T, T>`

## Example 1


```ts
comp(filter(pred), takeLast(1))

```
Yields none or only the last value which passed the predicate check. If `src` input is given, returns last match found (or `undefined`<!-- -->).

## Example 2


```ts
matchLast((x) => x >= 5, [3, 1, 6, 5, 4, 2])
// 5

transduce(
  comp(
    matchLast((x) => x >= 5),
    map((x) => x * 10)
  ),
  last(),
  [3, 1, 4, 2, 6, 5]
)
// 50

```

