<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Replace2](./api.replace2.md)

## Replace2 type

<b>Signature:</b>

```typescript
export declare type Replace2<T, A extends Keys<T>, B extends Keys1<T, A>, V> = Without<T, A> & {
    [id in A]: Replace<Val1<T, A>, B, V>;
};
```