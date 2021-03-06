<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [extendSides](./transducers.extendsides.md)

## extendSides() function

Yields iterator of given iterable which repeats the first and/or last value(s) `numLeft`<!-- -->/`numRight` times (default: 1).

<b>Signature:</b>

```typescript
export declare function extendSides<T>(src: Iterable<T>, numLeft?: number, numRight?: number): IterableIterator<T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  src | <code>Iterable&lt;T&gt;</code> |  |
|  numLeft | <code>number</code> |  |
|  numRight | <code>number</code> |  |

<b>Returns:</b>

`IterableIterator<T>`

## Remarks

By default both sides are repeated, but can be adjusted by setting either of them to zero. `numRight` defaults to same value as `numLeft`<!-- -->.

## Example


```ts
[...extendSides([1, 2, 3])]
// [ 1,  1, 2, 3,  3]

[...extendSides([1, 2, 3], 3)]
// [ 1, 1, 1,  1, 2, 3,  3, 3, 3 ]

[...extendSides([1, 2, 3], 0, 3)]
// [ 1, 2, 3,  3, 3, 3 ]

```
- [padSides](./transducers.padsides.md) - [wrapSides()](./transducers.wrapsides.md)

