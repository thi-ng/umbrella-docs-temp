<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Without7](./api.without7.md)

## Without7 type

<b>Signature:</b>

```typescript
export declare type Without7<T, A extends Keys<T>, B extends Keys1<T, A>, C extends Keys2<T, A, B>, D extends Keys3<T, A, B, C>, E extends Keys4<T, A, B, C, D>, F extends Keys5<T, A, B, C, D, E>, G extends Keys6<T, A, B, C, D, E, F>> = Without<T, A> & {
    [id in A]: Without6<Val1<T, A>, B, C, D, E, F, G>;
};
```