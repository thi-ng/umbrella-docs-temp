<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Last](./api.last.md)

## Last type

Extracts the last element from a tuple.

<b>Signature:</b>

```typescript
export declare type Last<T extends unknown[]> = {
    0: Last<Tail<T>>;
    1: Head<T>;
}[IsEmpty<Tail<T>>];
```