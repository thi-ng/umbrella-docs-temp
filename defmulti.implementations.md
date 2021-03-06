<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/defmulti](./defmulti.md) &gt; [implementations](./defmulti.implementations.md)

## implementations variable

Syntax-sugar intended for sets of multi-methods sharing same dispatch values / logic. Takes a dispatch value, an object of "is-a" relationships and a number of multi-methods, each with an implementation for the given dispatch value.

<b>Signature:</b>

```typescript
implementations: (id: string | number | symbol, rels: IObjectOf<MultiFn<any>[]>, ...impls: (MultiFn<any> | import("@thi.ng/api").FnAny<any>)[]) => void
```

## Remarks

The relations object has dispatch values (parents) as keys and arrays of multi-methods as their values. For each multi-method associates the given `type` with the related parent dispatch value to delegate to its implementation.

The remaining implementations are associated with their related multi-method and the given `type` dispatch value.

## Example


```ts
foo = defmulti((x) => x.id);
bar = defmulti((x) => x.id);
bax = defmulti((x) => x.id);
baz = defmulti((x) => x.id);

// define impls for dispatch value `a`
implementations(
  "a",

  // delegate bax & baz impls to dispatch val `b`
  {
     b: [bax, baz]
  },

  // concrete multi-fn impls
  foo,
  (x) => `foo: ${x.val}`,

  bar,
  (x) => `bar: ${x.val.toUpperCase()}`
);

// add parent impls
bax.add("b", (x) => `bax: ${x.id}`);
baz.add("c", (x) => `baz: ${x.id}`);
// use "c" impl for "b"
baz.isa("b", "c");

foo({ id: "a", val: "alice" }); // "foo: alice"
bar({ id: "a", val: "alice" }); // "bar: ALICE"
bax({ id: "a", val: "alice" }); // "bax: a"
baz({ id: "a", val: "alice" }); // "baz: a"

baz.impls(); // Set { "c", "a", "b" }

```

