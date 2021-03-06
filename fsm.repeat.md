<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [repeat](./fsm.repeat.md)

## repeat variable

Takes a matcher and `min` / `max` repeats. Returns new matcher which only returns `Match.FULL` if `match` succeeded at least `min` times or once `max` repetitions have been found.

<b>Signature:</b>

```typescript
repeat: <T, C, R>(match: Matcher<T, C, R>, min: number, max: number, success?: SeqCallback<T, C, R> | undefined, fail?: SeqCallback<T, C, R> | undefined) => Matcher<T, C, R>
```
