<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [fromInterval](./rstream.frominterval.md)

## fromInterval variable

Returns a new `Stream` which emits a monotonically increasing counter value at given `delay` interval, up to an optionally defined max value (default: ∞), after which the stream is closed. The stream only starts when the first subscriber becomes available.

<b>Signature:</b>

```typescript
fromInterval: (delay: number, count?: number) => Stream<number>
```