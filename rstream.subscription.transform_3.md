<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [Subscription](./rstream.subscription.md) &gt; [transform](./rstream.subscription.transform_3.md)

## Subscription.transform() method

<b>Signature:</b>

```typescript
transform<C, D, E, F>(a: Transducer<B, C>, b: Transducer<C, D>, c: Transducer<D, E>, d: Transducer<E, F>, opts?: Partial<CommonOpts>): Subscription<B, F>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  a | <code>Transducer&lt;B, C&gt;</code> |  |
|  b | <code>Transducer&lt;C, D&gt;</code> |  |
|  c | <code>Transducer&lt;D, E&gt;</code> |  |
|  d | <code>Transducer&lt;E, F&gt;</code> |  |
|  opts | <code>Partial&lt;CommonOpts&gt;</code> |  |

<b>Returns:</b>

`Subscription<B, F>`

