<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [ITransformable](./rstream.itransformable.md) &gt; [transform](./rstream.itransformable.transform_2.md)

## ITransformable.transform() method

<b>Signature:</b>

```typescript
transform<C, D, E>(a: Transducer<B, C>, b: Transducer<C, D>, c: Transducer<D, E>, opts?: Partial<CommonOpts>): Subscription<B, E>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  a | <code>Transducer&lt;B, C&gt;</code> |  |
|  b | <code>Transducer&lt;C, D&gt;</code> |  |
|  c | <code>Transducer&lt;D, E&gt;</code> |  |
|  opts | <code>Partial&lt;CommonOpts&gt;</code> |  |

<b>Returns:</b>

`Subscription<B, E>`
