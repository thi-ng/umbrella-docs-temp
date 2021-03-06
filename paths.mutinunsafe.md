<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/paths](./paths.md) &gt; [mutInUnsafe](./paths.mutinunsafe.md)

## mutInUnsafe variable

Unchecked version of .

<b>Signature:</b>

```typescript
mutInUnsafe: <T = any>(state: any, path: Path, val: T) => any
```

## Remarks

The type parameter `T` can be used to indicate the type of the nested value to be mutated (default: `any`<!-- -->).

## Example


```ts
mutIn({ a: { b: [10, 20] } }, "a.b.1", 23);
// { a: { b: [ 10, 23 ] } }

// fails (see `mutator` docs)
mutIn({}, "a.b.c", 23);
// undefined

```

