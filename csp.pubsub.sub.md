<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/csp](./csp.md) &gt; [PubSub](./csp.pubsub.md) &gt; [sub](./csp.pubsub.sub.md)

## PubSub.sub() method

Creates a new topic subscription channel and returns it. Each topic is managed by its own `Mult` and can have arbitrary number of subscribers. If the optional transducer is given, it will only be applied to the new subscription channel.

The special "\*" topic can be used to subscribe to all messages and acts as multiplexed pass-through of the source channel.

<b>Signature:</b>

```typescript
sub(id: string, tx?: Transducer<T, any>): Channel<any> | undefined;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  id | <code>string</code> | topic id |
|  tx | <code>Transducer&lt;T, any&gt;</code> | transducer for new subscription |

<b>Returns:</b>

`Channel<any> | undefined`
