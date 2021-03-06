<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/compose](./compose.md) &gt; [threadLast](./compose.threadlast.md)

## threadLast variable

Takes an `init` value and a number of functions and/or function tuples, consisting of: `[fn, ...args]`<!-- -->. Executes each function (or tuple) with the return value of the previous expression inserted as last argument, using `init` for the first expression.

<b>Signature:</b>

```typescript
threadLast: (init: any, ...fns: (FnAny<any> | [FnAny<any>, ...any[]])[]) => any
```

## Example


```ts
const neg = (x) => -x;
const sub = (a, b) => a - b;
const div = (a, b) => a / b;

threadLast(
  5,
  neg,       // -5
  [sub, 10], // 20 - (-5) = 25
  [div, 10]  // 10 / 25 = 0.4
);

// 0.4

```
[threadFirst](./compose.threadfirst.md)

