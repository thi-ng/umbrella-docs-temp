<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast](./shader-ast.md) &gt; [buildCallGraph](./shader-ast.buildcallgraph.md)

## buildCallGraph variable

Builds dependency graph of given function, by recursively adding all function dependencies. Returns graph.

<b>Signature:</b>

```typescript
buildCallGraph: (fn: Func<any>, graph?: DGraph<Func<any>>) => DGraph<Func<any>>
```
