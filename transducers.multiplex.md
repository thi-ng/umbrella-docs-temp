<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [multiplex](./transducers.multiplex.md)

## multiplex() function

Yields a new transducer which applies given transducers in parallel (using [juxt()](./compose.juxt.md) &amp; [step](./transducers.step.md)<!-- -->) and produces tuples of results.

<b>Signature:</b>

```typescript
export declare function multiplex<T, A>(a: TxLike<T, A>): Transducer<T, [A]>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  a | <code>TxLike&lt;T, A&gt;</code> |  |

<b>Returns:</b>

`Transducer<T, [A]>`

## Remarks

Use the [noop](./transducers.noop.md) transducer for processing lanes which should retain the original input values.

## Example


```ts
[...iterator(
  multiplex(
    map(x => x.charAt(0)),
    map(x => x.toUpperCase()),
    map(x => x.length)
  ),
  ["Alice", "Bob", "Charlie", "Andy"]
)]
// [ [ "A", "ALICE", 5 ], [ "B", "BOB", 3 ], [ "C", "CHARLIE", 7 ] ]

```

