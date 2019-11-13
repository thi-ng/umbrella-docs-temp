<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [cat](./transducers.cat.md)

## cat variable

Transducer to concatenate iterable values. Iterates over each input and emits individual values down stream, therefore removing one level of nesting from the input. If, during processing, the transducer is given a wrapped `reduced()` input iterable, it will still be processed as normal, but then immediately triggers early termination by wrapping its own result in `reduced()`<!-- -->. E.g. this behavior allows a `mapcat()` user functions to benefit from `reduced` results.

```
[...iterator(comp(map((x) => [x, x]), cat()), [1, 2, 3, 4])]
// [ 1, 1, 2, 2, 3, 3, 4, 4 ]

[...iterator(
  comp(
    mapIndexed((i, x) => [[i], [x, x]]),
    cat(),
    cat()
  ),
  "abc"
)]
// [ 0, 'a', 'a', 1, 'b', 'b', 2, 'c', 'c' ]

[...mapcat((x)=>(x > 1 ? reduced([x, x]) : [x, x]), [1, 2, 3, 4])]
// [ 1, 1, 2, 2 ]

```
 thi.ng/transducers/iter/concat  thi.ng/transducers/xform/mapcat

<b>Signature:</b>

```typescript
cat: <T>() => Transducer<Iterable<T> | null | undefined, T>
```