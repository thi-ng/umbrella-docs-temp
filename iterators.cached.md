<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/iterators](./iterators.md) &gt; [cached](./iterators.cached.md)

## cached variable

<b>Signature:</b>

```typescript
cached: <T>(input: Iterable<T>) => () => {
    [Symbol.iterator](): IterableIterator<T>;
    next(): IteratorResult<T, any>;
}
```
