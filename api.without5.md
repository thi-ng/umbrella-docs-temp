<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Without5](./api.without5.md)

## Without5 type

<b>Signature:</b>

```typescript
export declare type Without5<T, A extends Keys<T>, B extends Keys1<T, A>, C extends Keys2<T, A, B>, D extends Keys3<T, A, B, C>, E extends Keys4<T, A, B, C, D>> = Without<T, A> & {
    [id in A]: Without4<Val1<T, A>, B, C, D, E>;
};
```
