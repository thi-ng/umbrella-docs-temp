<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/atom](./atom.md) &gt; [View](./atom.view.md) &gt; [view](./atom.view.view.md)

## View.view() method

Like [IDeref.deref()](./api.ideref.deref.md)<!-- -->, but doesn't update view's cached state and dirty flag if value has changed.

<b>Signature:</b>

```typescript
view(): T | undefined;
```
<b>Returns:</b>

`T | undefined`

## Remarks

If there's an unprocessed value change, returns result of this sub's transformer or else the cached value.

\*\*Important:\*\* Use this function only if the view has none or or a stateless transformer. Else might cause undefined/inconsistent behavior when calling `view` or [IDeref.deref()](./api.ideref.deref.md) subsequently.

