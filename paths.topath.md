<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/paths](./paths.md) &gt; [toPath](./paths.topath.md)

## toPath variable

Converts the given key path to canonical form (array).

```
toPath("a.b.c");
// ["a", "b", "c"]

toPath(0)
// [0]

toPath(["a", "b", "c"])
// ["a", "b", "c"]

```

<b>Signature:</b>

```typescript
toPath: (path: Path) => (string | number)[]
```
