<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Path3](./api.path3.md)

## Path3 type

Type checked lookup path (depth 3)

<b>Signature:</b>

```typescript
export declare type Path3<T, A, B, C> = A extends Keys<T> ? B extends Keys1<T, A> ? C extends Keys2<T, A, B> ? readonly [A, B, C] : never : never : never;
```
