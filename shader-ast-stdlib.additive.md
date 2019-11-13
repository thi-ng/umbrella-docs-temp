<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-stdlib](./shader-ast-stdlib.md) &gt; [additive](./shader-ast-stdlib.additive.md)

## additive variable

Higher order function. Takes an AST type ID, a single-arg scalar function `fn`<!-- -->, number of octaves (default: 4) and an optional function name. Returns a new function which computes the summed value of `fn` over the given number octaves and accepts 3 args:

- position (float) - octave shift (float) - octave decay (usually 0.5)

For each octave `i` \[0..oct), the function is (in principle) evaluated as:

n += decay / exp2(i) \* fn(pos \* exp2(i) + i \* shift)

<b>Signature:</b>

```typescript
additive: <T extends Prim>(type: T, fn: Fn<Term<T>, Term<"float">>, oct?: number, name?: string) => import("@thi.ng/shader-ast").TaggedFn3<T, T, "float", "float">
```