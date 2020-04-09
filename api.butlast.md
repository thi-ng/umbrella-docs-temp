<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [ButLast](./api.butlast.md)

## ButLast type

Extracts everything except the last element from a tuple.

<b>Signature:</b>

```typescript
export declare type ButLast<T extends unknown[], C extends unknown[] = []> = {
    0: ButLast<Tail<T>, Prepend<Head<T>, C>>;
    1: Reverse<C>;
}[IsEmpty<Tail<T>>];
```