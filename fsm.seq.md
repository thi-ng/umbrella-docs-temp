<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [seq](./fsm.seq.md)

## seq variable

Takes an array of matchers and returns new matcher which applies them in sequence. If any of the given matchers fails, returns `Match.FAIL`<!-- -->.

<b>Signature:</b>

```typescript
seq: <T, C, R>(matches: Matcher<T, C, R>[], success?: SeqCallback<T, C, R> | undefined, fail?: SeqCallback<T, C, R> | undefined) => Matcher<T, C, R>
```
