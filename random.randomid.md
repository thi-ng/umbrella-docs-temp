<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/random](./random.md) &gt; [randomID](./random.randomid.md)

## randomID variable

Generates and returns a random string of `len` characters (default 4), plus optional given `prefix` and using only provided `syms` characters (default lowercase a-z).

```ts
randomID()
"qgdt"

randomID(8, "id-", "0123456789ABCDEF")
"id-94EF6E1A"

```

<b>Signature:</b>

```typescript
randomID: (len?: number, prefix?: string, syms?: string, rnd?: IRandom) => string
```