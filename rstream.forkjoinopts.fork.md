<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [ForkJoinOpts](./rstream.forkjoinopts.md) &gt; [fork](./rstream.forkjoinopts.fork.md)

## ForkJoinOpts.fork property

Transformation function prepare (e.g. chunk) work for a single worker. Receives worker `id` \[0 .. numWorkers), `numWorkers` and current input value to be processed. Only the results of this function are sent to the worker and therefore the function must return a type compatible with the configured worker instance.

For example, such a function might extract slices from a large input array, one per worker. The given worker ID and worker count can be used to create non-overlapping chunks to evenly spread the workload...

Also see: [forkBuffer](./rstream.forkbuffer.md)

<b>Signature:</b>

```typescript
fork: Fn3<number, number, IN, MSG>;
```
