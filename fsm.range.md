<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [range](./fsm.range.md)

## range variable

Returns a single input matcher which returns `Match.FULL` if the input is within the closed interval given by \[`min`<!-- -->,`max`<!-- -->\].

<b>Signature:</b>

```typescript
range: <T extends string | number, C, R>(min: T, max: T, success?: LitCallback<T, C, R> | undefined, fail?: LitCallback<T, C, R> | undefined) => Matcher<T, C, R>
```
