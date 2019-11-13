<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hiccup-css](./hiccup-css.md) &gt; [RuleFn](./hiccup-css.rulefn.md)

## RuleFn type

Function type used by `at_xxx()` functions or any other function in the head position of a rule scope array.

These fns have special behavior and are resonsible to append their results to the CSS output string accumulator directly.

<b>Signature:</b>

```typescript
export declare type RuleFn = (acc: string[], opts: CSSOpts) => string[];
```