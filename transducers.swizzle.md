<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [swizzle](./transducers.swizzle.md)

## swizzle() function

Transducer which performs value reordering on inputs using provided property order. Accepts arrays or objects as input, but always yields arrays.

<b>Signature:</b>

```typescript
export declare function swizzle<T>(order: PropertyKey[]): Transducer<T, any[]>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  order | <code>PropertyKey[]</code> | key order |

<b>Returns:</b>

`Transducer<T, any[]>`

## Example


```ts
[...swizzle([3,0,2,1], [[1,2,3,4], [10,20,30,40]])]
// [ [ 4, 1, 3, 2 ], [ 40, 10, 30, 20 ] ]

[...swizzle([0,0,1,1], [[1,2,3,4], [10,20,30,40]])]
// [ [ 1, 1, 2, 2 ], [ 10, 10, 20, 20 ] ]

[...swizzle(["z","x"], [{x: 1, y: 2, z: 3}])]
// [ [ 3, 1 ] ]

```
[swizzle](./arrays.swizzle.md)

