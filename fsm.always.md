<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [always](./fsm.always.md)

## always variable

Returns a matcher which always succeeds (produces a `Match.FULL` result) for any given input. Use `never()` for the opposite effect.

<b>Signature:</b>

```typescript
always: <T, C, R>(callback?: LitCallback<T, C, R> | undefined) => Matcher<T, C, R>
```