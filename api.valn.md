<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [ValN](./api.valn.md)

## ValN type

Generalised version of Val1-Val7

<b>Signature:</b>

```typescript
export declare type ValN<T, L extends unknown[]> = L extends [] ? T : ValNReducer<T, Head<L>, Tail<L>>;
```
