<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/paths](./paths.md) &gt; [getIn](./paths.getin.md)

## getIn variable

Immediate use getter, i.e. same as: `getter(path)(state)`<!-- -->.

```ts
getIn({a: {b: {c: 23}}}, "a.b.c");
// 23

```

<b>Signature:</b>

```typescript
getIn: (state: any, path: Path) => any
```