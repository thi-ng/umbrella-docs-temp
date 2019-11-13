<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/resolve-map](./resolve-map.md)

## resolve-map package

## Variables

|  Variable | Description |
|  --- | --- |
|  [absPath](./resolve-map.abspath.md) | Takes the path for the current key and a lookup path string. Converts the possibly relative lookup path into its absolute form. |
|  [resolve](./resolve-map.resolve.md) | Visits all key-value pairs or array items in depth-first order, expands any reference values, mutates the original object and returns it. Cyclic references are not allowed and will throw an error. However, refs pointing to other refs are recursively resolved (again, provided there are no cycles).<!-- -->Reference values are special strings representing lookup paths of other values in the object and are prefixed with <code>@</code> for relative refs or <code>@/</code> for absolute refs and both using <code>/</code> as path separator (Note: trailing slashes are NOT allowed!). Relative refs are resolved from the currently visited object and support "../" prefixes to access any parent levels. Absolute refs are always resolved from the root level (the original object passed to this function).
```ts
// `c` references sibling `d`
// `d` references parent `a`
resolve({a: 1, b: {c: "@d", d: "@/a"} })
// { a: 1, b: { c: 1, d: 1 } }

```
Any function values are called using two possible conventions:<!-- -->1) If the user function uses ES6 object destructuring for its first argument, the given object keys are resolved prior to calling the function and the resolved values provided as first argument (object) and a general <code>resolve</code> function as second argument. 2) If no de-structure form is found in the function's arguments, the function is only called with <code>resolve</code> as argument.<!-- -->\*\*Important:\*\* Since ES6 var names can't contain special characters, destructured keys can ALWAYS only be looked up as siblings of the currently processed key.<!-- -->The <code>resolve</code> function provided as arg to the user function accepts a path (\*\*without <code>@</code> prefix\*\*) to look up any other values in the root object.
```
// `c` uses ES6 destructuring form to look up `a` & `b` values
// `d` uses provided resolve fn arg `$` to look up `c`
resolve({a: 1, b: 2, c: ({a,b}) => a + b, d: ($) => $("c") })
// { a: 1, b: 2, c: 3, d: 3 }

// last item references item @ index = 2
resolve([1,2, ($) => $("0") + $("1"), "@2"])
// [1, 2, 3, 3]

```
The return value of the user provided function is used as final value for that key in the object. This mechanism can be used to compute derived values of other values stored anywhere in the root object. \*\*Function values will always be called only once.\*\* Therefore, in order to associate a function as final value to a key, it MUST be wrapped with an additional function, as shown for the <code>e</code> key in the example below. Similarly, if an actual string value should happen to start with <code>@</code>, it needs to be wrapped in a function (see <code>f</code> key below).
```
// `a` is derived from 1st array element in `b.d`
// `b.c` is looked up from `b.d[0]`
// `b.d[1]` is derived from calling `e(2)`
// `e` is a wrapped function
res = resolve({
  a: ($) => $("b/c") * 100,
  b: { c: "@d/0", d: [2, ($) => $("../../e")(2) ] },
  e: () => (x) => x * 10,
  f: () => "@foo",
})
// { a: 200, b: { c: 2, d: [ 2, 20 ] }, e: [Function], f: "@foo" }

res.e(2);
// 20

```
 |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [LookupPath](./resolve-map.lookuppath.md) |  |
|  [ResolveFn](./resolve-map.resolvefn.md) |  |
