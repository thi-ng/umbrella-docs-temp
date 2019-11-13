<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [matchFirst](./transducers.matchfirst.md)

## matchFirst() function

Transducer composition / syntax sugar for:

```ts
comp(filter(pred), take(1))

```
Yields none or only the first value which passed the predicate check and then causes early termination. If `src` input is given, returns first match found (or `undefined`<!-- -->). Also see `matchLast()`<!-- -->.

```ts
matchFirst((x) => x >= 5, [3, 1, 4, 2, 6, 5])
// 6

transduce(
  comp(
    matchFirst((x) => x >= 5),
    map((x) => x * 10)
  ),
  last(),
  [3, 1, 4, 2, 6, 5]
)
// 60

```

<b>Signature:</b>

```typescript
export declare function matchFirst<T>(pred: Predicate<T>): Transducer<T, T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  pred | <code>Predicate&lt;T&gt;</code> | predicate function |

<b>Returns:</b>

`Transducer<T, T>`
