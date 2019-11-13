<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/paths](./paths.md) &gt; [setIn](./paths.setin.md)

## setIn variable

Immediate use setter, i.e. same as: `setter(path)(state, val)`<!-- -->.

```ts
setIn({}, "a.b.c", 23);
// {a: {b: {c: 23}}}

```

<b>Signature:</b>

```typescript
setIn: (state: any, path: Path, val: any) => any
```