<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast](./shader-ast.md) &gt; [defTarget](./shader-ast.deftarget.md)

## defTarget variable

Takes an object of code generator functions and returns a new code generator / compile target function which serializes a given AST using the provided node type implementations.

<b>Signature:</b>

```typescript
defTarget: <T>(impls: TargetImpl<T>) => Fn<Term<any>, T>
```