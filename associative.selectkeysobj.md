<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/associative](./associative.md) &gt; [selectKeysObj](./associative.selectkeysobj.md)

## selectKeysObj variable

Returns a new object only containing given keys (and only if they existed in the original).

<b>Signature:</b>

```typescript
selectKeysObj: <T extends any>(src: T, ks: Iterable<string | number | symbol>) => { [id in keyof T]?: T[id] | undefined; }
```
