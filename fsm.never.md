<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [never](./fsm.never.md)

## never variable

Returns a matcher which always fails (produces a `Match.FAIL` result) for any given input. Use `always()` for the opposite effect.

<b>Signature:</b>

```typescript
never: <T, C, R>(callback?: LitCallback<T, C, R> | undefined) => Matcher<T, C, R>
```