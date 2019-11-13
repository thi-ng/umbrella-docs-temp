<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [merge](./rstream.merge.md)

## merge variable

Returns a new `StreamMerge` instance, a subscription type consuming inputs from multiple inputs and passing received values on to any subscribers. Input streams can be added and removed dynamically. By default, `StreamMerge` calls `done()` when the last active input is done, but this behavior can be overridden via the `close` option.

```ts
merge({
    // input streams w/ different frequencies
    src: [
        fromIterable([1, 2, 3], 10),
        fromIterable([10, 20, 30], 21),
        fromIterable([100, 200, 300], 7)
    ]
}).subscribe(trace());
// 100
// 1
// 200
// 10
// 2
// 300
// 3
// 20
// 30

```
Use the `labeled()` transducer for each input to create a stream of labeled values and track their provenance:

```ts
merge({
    src: [
        fromIterable([1, 2, 3]).transform(labeled("a")),
        fromIterable([10, 20, 30]).transform(labeled("b")),
    ]
}).subscribe(trace());
// ["a", 1]
// ["b", 10]
// ["a", 2]
// ["b", 20]
// ["a", 3]
// ["b", 30]

```
 StreamMergeOpts

<b>Signature:</b>

```typescript
merge: <A, B>(opts?: Partial<StreamMergeOpts<A, B>> | undefined) => StreamMerge<A, B>
```