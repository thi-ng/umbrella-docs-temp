<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [tweenNumber](./rstream.tweennumber.md)

## tweenNumber variable

Convenience version of [tween](./rstream.tween.md) for its most common use case, tweening of numeric streams.

<b>Signature:</b>

```typescript
tweenNumber: (src: ISubscribable<number>, init?: number, speed?: number, eps?: number, clock?: number | ISubscribable<any> | undefined) => import("./subscription").Subscription<{
    src: number;
}, number>
```
