<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Path8](./api.path8.md)

## Path8 type

Type checked lookup path (depth 8)

<b>Signature:</b>

```typescript
export declare type Path8<T, A, B, C, D, E, F, G, H> = A extends Keys<T> ? B extends Keys1<T, A> ? C extends Keys2<T, A, B> ? D extends Keys3<T, A, B, C> ? E extends Keys4<T, A, B, C, D> ? F extends Keys5<T, A, B, C, D, E> ? G extends Keys6<T, A, B, C, D, E, F> ? H extends Keys7<T, A, B, C, D, E, F, G> ? readonly [A, B, C, D, E, F, G, H] : never : never : never : never : never : never : never : never;
```