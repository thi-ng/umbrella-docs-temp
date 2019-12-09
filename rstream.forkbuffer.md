<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [forkBuffer](./rstream.forkbuffer.md)

## forkBuffer variable

Higher-order fork function for scenarios involving the split-parallel processing of a large buffer.

<b>Signature:</b>

```typescript
forkBuffer: (minChunkSize?: number) => <T extends Sliceable<any>>(id: number, numWorkers: number, buf: T) => T
```

## Remarks

The returned function is meant to be used as `fork` function in a [ForkJoinOpts](./rstream.forkjoinopts.md) config and extracts a workload slice of the original buffer for a single worker. The HOF itself takes a minimum chunk size as optional parameter (default: 1).

\*\*Note:\*\* Depending on the configured `minChunkSize` and the size of the input buffer to be partitioned, the returned fork function might produce empty sub-arrays for some workers, iff the configured number of workers exceeds the resulting number of chunks / input values. E.g. If the number of workers = 8, buffer size = 10 and min chunk size = 2, then the last 3 (i.e. 8 - 10 / 2) workers will only receive empty workloads.

More generally, if the input buffer size is not equally distributable over the given number of workers, the last worker(s) might receive a larger, smaller or empty chunk.

Also see [forkJoin](./rstream.forkjoin.md) and [joinBuffer](./rstream.joinbuffer.md)<!-- -->.

## Example


```ts
forkJoin<number[], number[], number[], number[]>({
    src,
    // job definition / split buffer into chunks (min size 256 values)
    fork: forkBuffer(256),
    // re-join partial results
    join: joinBuffer(),
    worker: "./worker.js",
})

```
