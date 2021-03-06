<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [fromIterableSync](./rstream.fromiterablesync.md)

## fromIterableSync variable

Creates a new [Stream](./rstream.stream.md) of given iterable which synchronously calls `.next()` for each item of the iterable when the first (and in this case the only one) subscriber becomes available. Once the iterable is exhausted (MUST be finite!), then calls `.done()` by default, but can be avoided by passing `false` as last argument.

<b>Signature:</b>

```typescript
fromIterableSync: <T>(src: Iterable<T>, opts?: Partial<CommonOpts> | undefined) => Stream<T>
```
