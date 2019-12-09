<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [FromAtomOpts](./rstream.fromatomopts.md)

## FromAtomOpts interface

<b>Signature:</b>

```typescript
export interface FromAtomOpts<T> extends CommonOpts 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [changed](./rstream.fromatomopts.changed.md) | <code>Predicate2&lt;T&gt;</code> | User predicate to determine value changes in atom. New values are only emitted on stream if the predicate returns true. |
|  [emitFirst](./rstream.fromatomopts.emitfirst.md) | <code>boolean</code> | True, if the current atom value should be emitted when the stream activates. |
