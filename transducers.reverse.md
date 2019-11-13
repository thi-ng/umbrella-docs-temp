<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [reverse](./transducers.reverse.md)

## reverse() function

Yields iterator which consumes input and yield its values in reverse order. Important: Input MUST be finite.

```
[...tx.reverse("hello world")]
// [ "d", "l", "r", "o", "w", " ", "o", "l", "l", "e", "h" ]

```

<b>Signature:</b>

```typescript
export declare function reverse<T>(input: Iterable<T>): IterableIterator<T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  input | <code>Iterable&lt;T&gt;</code> |  |

<b>Returns:</b>

`IterableIterator<T>`
