<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [ISubscribable](./rstream.isubscribable.md) &gt; [subscribe](./rstream.isubscribable.subscribe_1.md)

## ISubscribable.subscribe() method

<b>Signature:</b>

```typescript
subscribe<C>(sub: Partial<ISubscriber<T>>, xform: Transducer<T, C>, opts?: Partial<CommonOpts>): Subscription<T, C>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  sub | <code>Partial&lt;ISubscriber&lt;T&gt;&gt;</code> |  |
|  xform | <code>Transducer&lt;T, C&gt;</code> |  |
|  opts | <code>Partial&lt;CommonOpts&gt;</code> |  |

<b>Returns:</b>

`Subscription<T, C>`

