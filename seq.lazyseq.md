<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/seq](./seq.md) &gt; [lazyseq](./seq.lazyseq.md)

## lazyseq variable

Returns a new lazily evaluated `ISeq` produced by given function `fn`<!-- -->, which is only realized when values are requested. The function is only called once (if at all) and its result cached.

<b>Signature:</b>

```typescript
lazyseq: <T>(fn: Fn0<ISeq<T> | undefined>) => ISeq<T>
```

## Example


```ts
const rnd = () => lazyseq(() => cons(Math.random(), rnd()));
const a = rnd();

a.first();
// 0.4421468479982633
a.next().first();
// 0.29578903713266524

```

