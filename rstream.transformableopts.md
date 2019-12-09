<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [TransformableOpts](./rstream.transformableopts.md)

## TransformableOpts interface

<b>Signature:</b>

```typescript
export interface TransformableOpts<A, B> extends CommonOpts 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [xform](./rstream.transformableopts.xform.md) | <code>Transducer&lt;A, B&gt;</code> | Transducer to transform incoming stream values. If given, all child subscriptions will only receive the transformed result values. |
