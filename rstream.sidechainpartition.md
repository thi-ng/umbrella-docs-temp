<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [sidechainPartition](./rstream.sidechainpartition.md)

## sidechainPartition variable

Returns a [Subscription](./rstream.subscription.md) which buffers values from `src` until side chain fires, then emits buffer (unless empty) and repeats process until either input is done.

<b>Signature:</b>

```typescript
sidechainPartition: <A, B>(side: ISubscribable<B>, opts?: Partial<SidechainPartitionOpts<B>> | undefined) => Subscription<A, A[]>
```

## Remarks

By default, the values read from the side chain are ignored (i.e. only their timing is used), however the `pred`<!-- -->icate option can be used to only trigger for specific values / conditions.

## Example


```t
// merge various event streams
events = merge([
    fromEvent(document,"mousemove"),
    fromEvent(document,"mousedown"),
    fromEvent(document,"mouseup")
]);

// queue event processing to only execute during the
// requestAnimationFrame cycle (RAF)
events.subscribe(sidechainPartition(fromRAF())).subscribe(trace())

```

