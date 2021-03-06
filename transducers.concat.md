<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [concat](./transducers.concat.md)

## concat() function

Yields iterator producing concatenation of given iterables. Undefined &amp; null inputs are silently ignored, however any such values produced or contained in an input will remain.

<b>Signature:</b>

```typescript
export declare function concat<T>(...xs: Nullable<Iterable<T>>[]): IterableIterator<T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  xs | <code>Nullable&lt;Iterable&lt;T&gt;&gt;[]</code> |  |

<b>Returns:</b>

`IterableIterator<T>`

## Example


```ts
[...concat([1, 2, 3], null, [4, 5])]
// [ 1, 2, 3, 4, 5 ]

[...concat([1, 2, 3, undefined], null, [4, 5])]
// [ 1, 2, 3, undefined, 4, 5 ]

```

