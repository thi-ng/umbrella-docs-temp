<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Head](./api.head.md)

## Head type

Extracts the first element of a tuple.

<b>Signature:</b>

```typescript
export declare type Head<T extends unknown[]> = T extends Parameters<(v: infer R, ...args: any[]) => any> ? R : never;
```
