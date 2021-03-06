<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [mapIndexed](./transducers.mapindexed.md)

## mapIndexed() function

Transducer. Similar to [map()](./transducers.map.md)<!-- -->, but given `fn` takes two arguments: `index` and `value` to transform.

<b>Signature:</b>

```typescript
export declare function mapIndexed<A, B>(fn: Fn2<number, A, B>, offset?: number): Transducer<A, B>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  fn | <code>Fn2&lt;number, A, B&gt;</code> | transformation function |
|  offset | <code>number</code> | initial index |

<b>Returns:</b>

`Transducer<A, B>`

## Remarks

An optional start index `offset` can be provided (default 0).

## Example


```ts
transduce(
  mapIndexed((i, x) => ["id" + i, x * 10], 42),
  assocObj(),
  [1, 2, 3]
)
// { id42: 10, id43: 20, id44: 30 }

```

