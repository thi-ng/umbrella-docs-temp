<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/defmulti](./defmulti.md) &gt; [defmultiN](./defmulti.defmultin.md)

## defmultiN variable

Returns a multi-dispatch function which delegates to one of the provided implementations, based on the arity (number of args) when the function is called.

<b>Signature:</b>

```typescript
defmultiN: <T>(impls: {
    [id: number]: import("@thi.ng/api").FnAny<T>;
}, fallback?: import("@thi.ng/api").FnAny<T> | undefined) => import("./api").MultiFn<T>
```

## Remarks

Internally uses [defmulti()](./defmulti.defmulti.md)<!-- -->, so new arities can be dynamically added (or removed) at a later time. If no `fallback` is provided, `defmultiN` also registers a [DEFAULT](./defmulti.default.md) implementation which simply throws an [IllegalArityError](./errors.illegalarityerror.md) when invoked.

\*\*Note:\*\* Unlike [defmulti()](./defmulti.defmulti.md) no argument type checking is supported, however you can specify the return type for the generated function.

## Example


```ts
const foo = defmultiN<string>({
  0: () => "zero",
  1: (x) => `one: ${x}`,
  3: (x, y, z) => `three: ${x}, ${y}, ${z}`
});

foo();
// zero
foo(23);
// one: 23
foo(1, 2, 3);
// three: 1, 2, 3
foo(1, 2);
// Error: illegal arity: 2

foo.add(2, (x, y) => `two: ${x}, ${y}`);
foo(1, 2);
// two: 1, 2

```

