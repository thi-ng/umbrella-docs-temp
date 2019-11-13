<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/pointfree-lang](./pointfree-lang.md) &gt; [run](./pointfree-lang.run.md)

## run variable

Main user function. Takes a string w/ DSL source code and optional env and stack. Prepares env using `ensureEnv()`<!-- -->, parses, compiles and executes source, then returns resulting `StackContext` tuple.

<b>Signature:</b>

```typescript
run: (src: string, env?: any, stack?: any[]) => pf.StackContext
```