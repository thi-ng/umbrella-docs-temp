<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/atom](./atom.md) &gt; [History](./atom.history.md) &gt; [reset](./atom.history.reset.md)

## History.reset() method

`IReset.reset()` implementation. Delegates to wrapped atom/cursor, but too applies `changed` predicate to determine if there was a change and if the previous value should be recorded.

<b>Signature:</b>

```typescript
reset(val: T): T;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  val | <code>T</code> | replacement value |

<b>Returns:</b>

`T`

