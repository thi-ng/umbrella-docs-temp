<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Tail](./api.tail.md)

## Tail type

Extracts everything except the first element from a tuple.

<b>Signature:</b>

```typescript
export declare type Tail<T extends unknown[]> = ((...a: T) => void) extends (v: any, ...args: infer R) => void ? R : never;
```
