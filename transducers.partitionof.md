<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [partitionOf](./transducers.partitionof.md)

## partitionOf() function

Transducer. Yields cyclic sequence of user defined variable sized chunks. The last partition emitted is allowed to be incomplete.

<b>Signature:</b>

```typescript
export declare function partitionOf<T>(sizes: number[]): Transducer<T, T[]>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  sizes | <code>number[]</code> |  |

<b>Returns:</b>

`Transducer<T, T[]>`

## Example


```ts
[...partitionOf([3,2,4], range(20))]
// [ [ 0, 1, 2 ],
//   [ 3, 4 ],
//   [ 5, 6, 7, 8 ],
//   [ 9, 10, 11 ],
//   [ 12, 13 ],
//   [ 14, 15, 16, 17 ],
//   [ 18, 19 ] ]

```

