<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-js](./shader-ast-js.md) &gt; [JSTarget](./shader-ast-js.jstarget.md)

## JSTarget interface

<b>Signature:</b>

```typescript
export interface JSTarget extends Fn<Term<any>, string> 
```

## Methods

|  Method | Description |
|  --- | --- |
|  [compile(tree, env)](./shader-ast-js.jstarget.compile.md) | Compiles given AST to JavaScript, using optional <code>env</code> as backend for various operators / builtins. If <code>env</code> is not given the bundled [JS\_DEFAULT\_ENV](./shader-ast-js.js_default_env.md) is used (based on [@thi.ng/vectors](./vectors.md) and [@thi.ng/matrices](./matrices.md) packages).<!-- -->Any functions defined in the given AST will be exported using their defined name via the returned object.
```
const js = targetJS();
const module = js.compile(
  defn("float", "foo", [["float"]], (x)=> [ret(mul(x, float(10)))])
);

module.foo(42)
// 420

module.foo.toString()
// function foo(_sym0) {
// return (_sym0 * 10);
// }

```
 |

