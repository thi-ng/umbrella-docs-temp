<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [fromViewUnsafe](./rstream.fromviewunsafe.md)

## fromViewUnsafe variable

Unchecked version of . Paths can be given as string or tuple.

<b>Signature:</b>

```typescript
fromViewUnsafe: <T>(atom: ReadonlyAtom<any>, opts: FromViewUnsafeOpts<T>) => Stream<T extends undefined ? any : T>
```

## Example


```ts
const db = defAtom<any>({ a: 1, b: { c: 2 }});

// create stream of `c` value changes
fromViewUnsafe(
  db,
  {
    path: "b.c",
    tx: (x) => x != null ? String(x) : "n/a"
  }
).subscribe(trace("view:"))
// view: 2

// update `c` in state
db.swapInUnsafe("b.c", (x: number) => x + 1);
// view: 3

db.reset({ a: 10 });
// view: n/a

```

